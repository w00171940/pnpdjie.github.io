# 业务设计
运营商可以根据网络规划，预置业务参数、分配资源，发布多种业务模板，用于匹配不同的租户诉求。用户完成一次业务设计后，其业务模板可以用于多次业务发放，提升运营商发放业务的效率。

业务模板包括如下两个视角的配置：
- CFS（Customer Face Service）：即面向租户的业务形态，包括租户关心的业务参数，比如业务接入点、SLA等。不涉及具体的网络细节，如承接业务的网络组网、协议和配置等。
- RFS（Resource Face Service）：即面向网络的连接设计，包括域内连接网络标准协议的选择和配置、域间的网络连接创建策略和配置等。可以选择原子组件（即普通域）或自定义组件（即将已定义的业务模板作为域）。

业务设计支持创建如下两大场景的业务模板：
- 单域业务：即业务专线的源宿节点在一个单原子VPN业务的管理域。经过的管理域指一个控制器的管理域，比如某企业与分企业在同一个城市里。
- 跨域业务：即业务专线的源宿节点跨过两个及以上单域VPN业务管理域。比如某企业与另个企业分别在不同的两个城市，中间需要经过汇聚域、核心域实现业务专线的创建。

## 前提条件
- 用户具备“IP WAN业务管理”的“配置IP WAN网络设计”和“查看IP WAN网络设计”的权限。更多信息可参见[了解用户与权限](/hedex/hedex.do?lib=ies_control_zh&id=AdminConsoleHome_002&locale=zh-cn)。
- 已在[“一站式资源准备”](/basereswebsite/navigation.html?navg=accessSystem)中完成基础资源的准备，[了解更多信息](/hedex/hedex.do?lib=ies_control_zh&id=AdminConsoleHome_002&locale=zh-cn)。

## 后续操作
- [业务模板维护](/vpndesignwebsite/manage/index.html?agencyId=1&locale=zh-cn)：业务模板创建后可以执行发布、停止发布、复制、修改业务模板名称操作，对于未发布或去发布的业务模板可以执行修改、删除等操作。
- [业务发放](/ui/wansolution/v1/pages/provision.html?showMenu=false&agencyId=1&locale=zh-cn)：选择已设计好的业务模板发放业务。
