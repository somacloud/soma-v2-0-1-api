## node/hostsmgr {#node-hostsmgr}

**基本信息：**

| 方法描述 | 主机分配管理：查询可以分配给租户的主机和租户已经分配了的主机列表 |
| --- | --- |
| 请求方法 | POST |
| API | node/hostmgr |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 否 |
|  | 用户 | 否 |
| 多语 | 中文名称 | 主机分配管理：查询可以分配给租户的主机和租户已经分配了的主机列表 |
|  | 英文名称 |  |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/node/hostmgr?_=1410924373474

**参数：**Json String

{“tenantCode”:”XXX”,”keyword”:”XXX”}

查询可以分配给租户的主机和租户已经分配了的主机列表。

**返回值：**Collection < ComputerVO>

**说明：**ComputerVO 见node/list