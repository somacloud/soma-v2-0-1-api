## application/listServers {#application-listservers}

**基本信息：**

| 方法描述 | 根根据编码查询应用和服务的数据库存储的信息和及时状态 |
| --- | --- |
| 请求方法 | POST |
| API | application/listServers |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询应用和服务信息 |
|  | 英文名称 | **Query applications and servers by application code** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/ listServers?_=1415951479462

**参数：**String code

**返回值：**Response r详细见node/listbypage

r.data=List< VirtualSystemVO> vos

vos.size()=1