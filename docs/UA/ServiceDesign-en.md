## Service Design
CloudOpera Orchestrator SDN allows a carrier to preset service parameters, allocate resources, and release various service templates based on a network plan to meet diverse tenant requirements.

Service templates apply to two types of services:
- Customer facing services (CFSs): tenant-oriented services. Service parameters that tenants concern include the service access point and SLA. Specific network details are not involved, such as the networking modes, protocols, and configurations of networks that carry the services.
- Resource facing services (RFSs): network-oriented connections. The design includes the selection and configuration of a network protocol for intra-domain connections, and configuration and policy creation for inter-domain connections.
The service design supports the service templates in two service scenarios:- Single-domain services: The source and sink nodes of VPN services are in the management domain of a single atomic VPN service. The traversed management domain refers to one domain under the management of a controller, in the same way as an enterprise and its branches are in the same city.- Cross-domain services: The source and sink nodes of VPN services cross more than one management domains of single-domain VPN services. It is similar to the condition that an enterprise and its branches are in different cities. Between the domains, the service must cross the convergence domain and core domain to achieve the creation of VPN services.

### Prerequisites
- You have permission to perform operations on **Service Design Management** and **VPN Policy Management**. [![](../image/open_soft.png)More details](/hedex/hedex.do?lib=ies_control_en&id=hlp_security_p_hlp_usermanage&locale=en-us).
- You have collected NE, port, and link data from controllers. [![](../image/open_soft.png)More details](/hedex/hedex.do?lib=ies_control_en&id=base_resource&locale=en-us).

### Follow-up Procedure
- [![](../image/open_soft.png)Service template maintenance](/vpndesignwebsite/manage/index.html): After a service template is created, you can release, revoke, copy, delete, export, or modify it. When a service template has not been released or has been revoked, you can also release, copy, delete, export, or modify it.
- [![](../image/open_soft.png)Service provisioning](/ui/wansolution/v1/pages/provision.html): Select the designed service template for service provisioning.

