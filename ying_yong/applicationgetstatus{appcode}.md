## application/getStatus/{appCode} {#application-getstatus-appcode}

**基本信息：**

| 方法描述 | 查询应用和服务的状态 |
| --- | --- |
| 请求方法 | POST |
| API | application/getStatus/{id} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询应用和服务的状态 |
|  | 英文名称 | **query the status of application and servers** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/ getStatus/XXXXXXXX?_=1410924373474

**参数：**String appCode

**返回值：** Map

{“appCode”：“appStatusXXXX”,

“Server1Code”:”Server1StatusXXX”, …}