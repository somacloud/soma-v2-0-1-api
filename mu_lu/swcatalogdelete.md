## swcatalog/delete {#swcatalog-delete}

**基本信息：**

| 方法描述 | 根据编码删除软件类型 |
| --- | --- |
| 请求方法 | POST |
| API | swcatalog/delete |
| 权限 | 系统管理员 | 是，只能删除非系统预置的资源 |
|  | 租户管理员 | 是，只能删除自己上传的资源 |
|  | 系统用户 | 是，只能删除非系统预置的资源 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 根据编码删除软件类型 |
|  | 英文名称 | Delete software type by code |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/swcatalog/delete?_=1410924373474

**参数：**String

例如：“XXXXXXXXXX”

**返回值：**无

**说明：**SoftwareVO见swcatalog/list