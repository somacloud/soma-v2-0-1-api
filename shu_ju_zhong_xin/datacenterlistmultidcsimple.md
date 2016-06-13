## datacenter/listMultiDCSimple {#datacenter-listmultidcsimple}

**基本信息：**

| 方法描述 | 查询用户的多租户数据中心名称 |
| --- | --- |
| 请求方法 | POST |
| API | datacenter/listMultiDCSimple |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 否 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 查询用户的多租户数据中心名称 |
|  | 英文名称 | Query the simple information of user’s multi-tenant data center |
| 是否记入事件 | 否 |

**Request URL:**

[http://localhost/soma/rest/datacenter/listMultiDCSimple?_=1445331142563](http://localhost/soma/rest/datacenter/listMultiDCSimple?_=1445331142563)

**参数：**无

**返回值：**Response r

r.data的类型Collection< DCSimpleVO >

DCSimpleVO对象定义：

| 字段 | 类型 | 描述 |
| --- | --- | --- |
| code | String |  |
| name | String |  |
| dcType | String |  |
| mgtMode | String |  |