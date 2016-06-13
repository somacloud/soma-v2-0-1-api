## node/addvmbypolicy/{dcType} {#node-addvmbypolicy-dctype}

**基本信息：**

| 方法描述 | 根据虚机模板创建虚机 |
| --- | --- |
| 请求方法 | POST |
| API | node/addvmbypolicy/{dcType} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 用户 | 否 |
| 多语 | 中文名称 | 根据虚机模板创建虚机 |
|  | 英文名称 |  |
| 是否记入事件 |  |

**Request URL:**

http://127.0.0.1:7681/soma/rest/node/ addvmbypolicy/{dcType}?_=1410924373474

**参数：**

dcType：支持的数据中心类型：UAPCloud，阿里云，华为云，vcenter

String json：{“vmname”:”XXX”}。

**返回值：**Response r; r.data=tasked; 返回任务的id，创建虚机是远程耗时任务。

**说明：**