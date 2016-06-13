## servicecatalog/getRoleTypes {#servicecatalog-getroletypes}

**基本信息：**

| 方法描述 | 查询服务的角色类型 |
| --- | --- |
| 请求方法 | POST |
| API | servicecatalog/getRoleTypes |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询服务的角色类型 |
|  | 英文名称 | List service role types by names |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/servicecatalog/getRoleTypes?_=1415865575694

**参数：**String 类型的数组String[] serTypes

例：["APACHE2","UAP65","ORACLE11G","REDIS289","ACTIVEMQ510"]

**返回值：**String[] rtypes

例：["WEB Server","Middleware","Database Server","Cache","Queue"]