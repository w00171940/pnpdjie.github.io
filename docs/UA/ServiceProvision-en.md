# Service Provision
Service provisioning is a process where the orchestrator coordinates resources on the entire network, computes the optimal service trail, and provisions and activates service in a one-stop manner.

CloudOpera Orchestrator SDN provides the following functions to implement rapid E2E service provisioning across vendors.
- Supports various service types. Supports the provisioning of various composite services including the layer 2 EPL or EVPL private line, layer 2 E-LAN private network, VLL, L3VPN, and SDH services.
- Quickly provisions services.
    - Identifies the service templates released during service design and automatically adds them to the service provisioning GUI.
    - Automatically simplifies the service provisioning operations by service type.
    - Provides a service topology that shows resource information such as links between domains, NEs within domains, VLAN IDs, and ports after the optimal service route is computed.

## Prerequisites
- You have permission to perform operations on **IP WAN Service Management**.
- 已在完成基础资源的准备，[了解更多信息](/hedex/hedex.do?lib=ies_control_zh&id=AdminConsoleHome_002&locale=zh-cn)。
- 已在[“业务设计”](/vpndesignwebsite/manage/index.html?action=create&agencyId=1&locale=zh-cn)中完成业务模板的创建。

## 注意事项
- L2VPN业务不支持设置保护组。
- SDH业务不需要设置保护组和路有约束。

[单击了解更多业务发放的信息](/hedex/hedex.do?lib=ies_control_zh&id=AdminConsoleHome_002&locale=zh-cn)。

## 后续操作
在[业务视图](/ui/underlayvpn/pages/servicemgrlist/servicemgrlist.html?showMenu=false&agencyId=1&locale=zh-cn)中进行业务维护，如查看业务拓扑、连通性检测、激活去激活业务等。[查看更多业务维护操作](/hedex/hedex.do?lib=ies_control_zh&id=AdminConsoleHome_002&locale=zh-cn)。
