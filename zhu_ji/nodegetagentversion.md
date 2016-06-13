## node/getAgentVersion {#node-getagentversion}

**基本信息：**

| 方法描述 | 查询Agent最新版本 |
| --- | --- |
| 请求方法 | GET |
| API | node/ getAgentVersion |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是（升级Agent使用） |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 查询Agent最新版本 |
|  | 英文名称 | Query newest version of Agent |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/node/getAgentVersion?_=1410924373474

**参数：**

**返回值：**String agentVersion

**说明：**ComputerVOagentVersion见node/list