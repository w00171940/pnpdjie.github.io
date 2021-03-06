## Service ProvisionService
provisioning is a process where the orchestrator coordinates resources on the entire network, computes the optimal service trail, and provisions and activates service in a one-stop manner.

CloudOpera Orchestrator SDN provides the following functions to implement rapid E2E service provisioning across vendors.
- Supports various service types. Supports the provisioning of various composite services including the layer 2 EPL or EVPL private line, layer 2 E-LAN private network, VLL, L3VPN, and SDH services.
- Quickly provisions services.
    - Identifies the service templates released during service design and automatically adds them to the service provisioning GUI.
    - Automatically simplifies the service provisioning operations by service type.
    - Provides a service topology that shows resource information such as links between domains, NEs within domains, VLAN IDs, and ports after the optimal service route is computed.
    
### Prerequisites
- You have permission to perform operations on **Service Design Management** and **VPN Policy Management**. For details see [![](../image/open_soft.png)Users and Permission](/hedex/hedex.do?lib=ies_control_en&id=hlp_security_p_hlp_usermanage&locale=en-us).
- You have collected NE, port, and link data from controllers. [![](../image/open_soft.png)More details](/hedex/hedex.do?lib=ies_control_en&id=base_resource&locale=en-us)。
- A service profile has been created in the [![](../image/open_soft.png)“Service design”](/vpndesignwebsite/manage/index.html?action=create)

### Note
- A protection group is not required for provisioning the L2VPN service.
- A protection group and route constraints are not required for provisioning the SDH service.

[![](../image/open_soft.png)More details](/hedex/hedex.do?lib=ies_control_en&id=ipwan_serviceprovision).

### Follow-up Procedure
 Perform service maintenance such as service topology query, connectivity check, service activation, and service deactivation in the [![](../image/open_soft.png)service view](/ui/wansolution/v1/pages/servicemgrlist/servicemgrlist.html). [![](../image/open_soft.png)More details](/hedex/hedex.do?lib=ies_control_en&id=IPWAN_serviceMgr&locale=en-us).
