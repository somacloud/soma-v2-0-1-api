## node/allocateHosts {#node-allocatehosts}

**基本信息：**

| 方法描述 | 系统管理员给租户分配主机 |
| --- | --- |
| 请求方法 | POST |
| API | node/allocateHosts |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 否 |
|  | 用户 | 否 |
| 多语 | 中文名称 | 系统管理员给租户分配主机 |
|  | 英文名称 |  |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/node/allocateHosts?_=1410924373474

**参数：**List&lt;String&gt; codes

系统管理员收回编码在codes列表中的的所有主机

**返回值：**无

**说明：**