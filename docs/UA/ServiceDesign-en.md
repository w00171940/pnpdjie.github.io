# Service Design
CloudOpera Orchestrator SDN allows a carrier to preset service parameters, allocate resources, and release various service profiles based on a network plan to meet diverse tenant requirements. 

Service profiles apply to two types of services:
- Customer facing services (CFSs): tenant-oriented services. Service parameters that tenants concern include the service access point and SLA. Specific network details are not involved, such as the networking modes, protocols, and configurations of networks that carry the services.
- Resource facing services (RFSs): network-oriented connections. The design includes the selection and configuration of a network protocol for intra-domain connections, and configuration and policy creation for inter-domain connections.

The service design supports the service profiles in two service scenarios:
- Single-domain services: The source and sink nodes of VPN services are in the management domain of a single atomic VPN service. The traversed management domain refers to one domain under the management of a controller, in the same way as an enterprise and its branches are in the same city.
- Cross-domain services: The source and sink nodes of VPN services cross more than one management domains of single-domain VPN services. It is similar to the condition that an enterprise and its branches are in different cities. Between the domains, the service must cross the convergence domain and core domain to achieve the creation of VPN services.

## Prerequisites[]
- You have permission to perform operations on **Service Design Management** and **VPN Policy Management**. For details see [Users and Permission](/hedex/hedex.do?lib=ies_control_zh&id=AdminConsoleHome_002&locale=zh-cn).
- 已完成基础资源的准备，[了解更多信息](/hedex/hedex.do?lib=ies_control_zh&id=AdminConsoleHome_002&locale=zh-cn)。

## 后续操作
- [业务模板维护](/vpndesignwebsite/manage/index.html?agencyId=1&locale=zh-cn)：业务模板创建后可以执行发布、停止发布、复制、修改业务模板名称操作，对于未发布或去发布的业务模板可以执行修改、删除等操作。
- [业务发放](/ui/wansolution/v1/pages/provision.html?showMenu=false&agencyId=1&locale=zh-cn)：选择已设计好的业务模板发放业务。
