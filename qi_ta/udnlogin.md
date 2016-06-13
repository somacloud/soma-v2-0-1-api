## udn/login {#udn-login}

**基本信息：**

| 方法描述 | UDN登陆 |
| --- | --- |
| 请求方法 | POST |
| API | udn/login |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | UDN登陆 |
|  | 英文名称 | **UDN login** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/udn/login?_=1410924373474

**参数：**SLI sli

SLI对象

| 名称 | 类型 | 描述 |
| --- | --- | --- |
| code | String |  |
| client_id | String |  |
| client_secret | String |  |
| redirect_uri | String |  |
| tokenurl | String |  |

**返回值：**Session svo

**说明：**Session对象

| 名称 | 类型 | 描述 |
| --- | --- | --- |
| sessionId | String |  |
| user | AdminVO | 对象详见account/lock/{code} |
| loginTime | Long |  |
| lastActivedTime | Long |  |