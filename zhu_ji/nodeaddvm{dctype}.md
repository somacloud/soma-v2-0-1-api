## node/addvm/{dcType} {#node-addvm-dctype}

**基本信息：**

| 方法描述 | 新增虚机 |
| --- | --- |
| 请求方法 | POST |
| API | node/addvm/{dcType} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 用户 | 否 |
| 多语 | 中文名称 | 新增虚机 |
|  | 英文名称 |  |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/node/allocateHosts?_=1410924373474

**参数：**dcType：支持的数据中心类型：UAPCloud，阿里云，华为云，vcenter

String json：json为各个数据中心的虚机创建时需要的参数。

UAPCloud

| 属性 | 类型 | 描述 |
| --- | --- | --- |
| vmname | String |  |
| agentPort | String |  |
| vmpolicycode | String |  |
| dccode | String |  |
| ostype | String |  |
| memSize | String |  |
| cpuFrq | String |  |
| cpuCount | String |  |
| hypervisor | String |  |
| templateid | String |  |
| tmplname | String |  |
| networkid | String |  |
| serviceofferingid | String |  |
| username | String |  |
| password | String |  |

阿里云

| 属性 | 类型 | 描述 |
| --- | --- | --- |
| vmname | String |  |
| agentPort | String |  |
| dccode | String |  |
| RegionId | String |  |
| IoOptimized | String |  |
| SecurityGroupId | String |  |
| memSize | String |  |
| cpuFrq | String |  |
| cpuCount | String |  |
| InternetChargeType | String |  |
| InternetMaxBandwidthOut | String |  |
| templateid | String |  |
| tmplname | String |  |
| ostype | String |  |
| InstanceType | String |  |
| SystemDiskCategory | String |  |
| username | String |  |
| DataDisk | String |  |
| password | String |  |

华为云

| 属性 | 类型 | 描述 |
| --- | --- | --- |
| vmname | String |  |
| dccode | String |  |
| memSize | String |  |
| cpuCount | String |  |
| password | String |  |

VCenter

| 属性 | 类型 | 描述 |
| --- | --- | --- |
| vmname | String |  |
| agentPort | String |  |
| dccode | String |  |
| ostype | String |  |
| memSize | String |  |
| cpuFrq | String |  |
| cpuCount | String |  |
| hypervisor | String |  |
| templateid | String |  |
| tmplname | String |  |
| networkid | String |  |
| serviceofferingid | String |  |
| username | String |  |
| password | String |  |

**返回值：**Response r; r.data=tasked; 返回任务的id，创建虚机是远程耗时任务。

**说明：**