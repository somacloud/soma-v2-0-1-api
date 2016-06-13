## node/queryuservmcount {#node-queryuservmcount}

**基本信息：**

| 方法描述 | 查询用户的主机数目 |
| --- | --- |
| 请求方法 | POST |
| API | node/queryuservmcount |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 用户 | 是 |
| 多语 | 中文名称 | 查询用户的所有主机的编码 |
|  | 英文名称 |  |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/node/queryuservmcount?_=1410924373474

**参数：**String usercode;

**返回值：**interger count;返回用户的主机数目。

**说明：**