## node/allocateService {#node-allocateservice}

**基本信息：**

| 方法描述 | 拓扑结构中为新建的服务查询节点列表 |
| --- | --- |
| 请求方法 | POST |
| API | node/allocateService |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 用户 | 是 |
| 多语 | 中文名称 | 拓扑结构中为新建的服务查询节点列表 |
|  | 英文名称 |  |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/node/allocateService?_=1410924373474

**参数：**Json String

| **类型** | **参数名称** | **描述** |
| --- | --- | --- |
| String | appCode | 应用编码 |
| String | stype | 服务类型 |
| String | machineName | 用于过滤的节点名称 |

**返回值：**List< ComputerVO>

**说明：**ComputerVO 见node/list