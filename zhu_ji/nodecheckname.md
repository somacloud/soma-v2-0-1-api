## node/checkname {#node-checkname}

**基本信息：**

| 方法描述 | 查询主机名称是否存在 |
| --- | --- |
| 请求方法 | POST |
| API | node/checkname |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 否 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 查询主机名称是否存在 |
|  | 英文名称 | Check the name of node |
| 是否记入事件 | 否 |

**Request URL:**

[http://localhost/soma/rest/node/checkname?_=1445331142563](http://localhost/soma/rest/node/checkname?_=1445331142563)

**参数：**String name

**返回值：**boolean

| true | 名称可用 |
| --- | --- |
| false | 名称已经存在 |