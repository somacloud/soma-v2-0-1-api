## renter/list {#renter-list}

**基本信息：**

| 方法描述 | 查询所有租户 |
| --- | --- |
| 请求方法 | GET |
| API | rente/list |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是，（分享资源时使用） |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 查询所有租户 |
|  | 英文名称 | **Query all tenants** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/renter/list?_=1410924373474

**参数：**无

**返回值：**Collection&lt;AccountVO&gt;

**说明：**AdminVO 见 account/lock/{code}