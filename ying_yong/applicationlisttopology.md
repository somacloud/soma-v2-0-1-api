## application/listTopology {#application-listtopology}

**基本信息：**

| 方法描述 | 根据应用编码查询应用服务及实例信息 |
| --- | --- |
| 请求方法 | POST |
| API | application/listTopology |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 分页查询应用列表 |
|  | 英文名称 | **Query applications by page** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/listTopology?_=1415951479462

**参数：**String code

**返回值：**Response r详细见node/listbypage

r.data= List&lt;VirtualSystemVO&gt; vos

vos.size()=1

vos.get(0).appInst = Application app