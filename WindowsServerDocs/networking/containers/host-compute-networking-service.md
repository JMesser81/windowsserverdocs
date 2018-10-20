# Host Compute Networking Service

## What is the HCN?
The Host Compute Networking (HCN) Service provides the control-path functionality to create and manage (CRUD) virtual networks, endpoints, and associated network policies that together provide connectivity and security for virtual machines and containers running on a Windows host. It is designed to be used in conjunction with the Host Compute Service (HCS) (which provides functionality to start and control VMs and containers) and should not be used in isolation. 

The HCN Service API is aimed at developers who need to manage networking for VMs and containers in their application workflows. End-users are not expected to directly interact with these APIs, rather applications (e.g. CNI plugins) are expected to build on top of these platform APIs to provide the end-user workflows. HCN runs as a Win32 service with an RPC server which exports a low-level, "RESTful-like" API for managing network resources on the host. The APIs are schema-based such that most functions of the API define input and output parameters as strings formatted in a JSON document. A subscription/callback API is provided to enable clients to register for notifications of service-wide events such as network creations and deleions.  HCN then programs the Windows network data-path to enforce network policies. HCN is also a stateless service; network settings and resources are non-persistent across service or system reboots and consumers of the API will need to clean up all resources created. 

A host compute network represents a Hyper-V virtual switch, a host virtual network adapter (acts as the default gateway for the network), along with IP subnets, DNS information, and routes. IPAM can be handled by the HCN service directly in the case of some networking modes (e.g. NAT) or managed externally. Network-wide policies can also be assigned to this resource.

A host compute network endpoint represents a host virtual network adapter and IP endpoint along with any endpoint-speific policies. 

A host compute network namespace represents an isolated network environment where each namespace has its own set of network interfaces and routing tables, separated from other namespaces. (This was formally described as a TCPIP Network Compartment).

A host compute network load balancer represents a network policy to load balance connections across multiple endpoints. 

## API References

For a list of the HCN functions, please see [References](host-networking-service-api.md)

For a reference to HCN JSON document schema, please see [HCN JSON Schema](hcn-json-schema.md)