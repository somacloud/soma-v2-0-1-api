## datacenter/listvirdc {#datacenter-listvirdc}

**基本信息：**

| 方法描述 | 查询用户的虚拟数据中心 |
| --- | --- |
| 请求方法 | GET |
| API | datacenter/listvirdc |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询用户的虚拟数据中心 |
|  | 英文名称 | Query the virtual data center |
| 是否记入事件 | 否 |

**Request URL:**

[http://localhost/soma/rest/datacenter/listvirdc?_=1445331142563](http://localhost/soma/rest/datacenter/listvirdc?_=1445331142563)

**参数：**无

**返回值：**Response r

r.data的类型Collection&lt;AccountDCVO&gt;

AccountDCVO对象定义：

| 字段 | 类型 | 描述 |
| --- | --- | --- |
| code | String |  |
| accountCode | String |  |
| dcCode | String |  |
| dcType | String |  |
| dcName | String |  |