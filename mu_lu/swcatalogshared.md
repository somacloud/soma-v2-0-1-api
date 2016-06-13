## swcatalog/shared {#swcatalog-shared}

**基本信息：**

| 方法描述 | 分享软件类型 |
| --- | --- |
| 请求方法 | POST |
| API | swcatalog/shared |
| 权限 | 系统管理员 | 是，分享非系统预置的资源 |
|  | 租户管理员 | 是，分享自己上传的资源 |
|  | 系统用户 | 是，分享非系统预置的资源 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 分享软件类型 |
|  | 英文名称 | Share software type to others |
| 是否记入事件 | 是 |

**Request URL:**

[http://127.0.0.1:7681/soma/rest/swcatalog/shared?_=1415867638043](http://127.0.0.1:7681/appcloud/rest/appcatalog/shared?_=1415867638043)

**参数：**String

例1："{\"catalogName\":\"UAP63_TEST\",\"users\":\"0001AA10000000003YV6\"}"

分享名称为：UAP63_TEST的软件类型给用户“{用户编码}”

例2："{\"catalogName\":\"UAP63_TEST\",\"users\":\" shared\"}"

分享名称为：UAP63_TEST的软件类型给所有用户

例3："{\"catalogName\":\"UAP63_TEST\",\"users\":\"private\"}"

设置UAP63_TEST的软件类型为私有型

**返回值：**无