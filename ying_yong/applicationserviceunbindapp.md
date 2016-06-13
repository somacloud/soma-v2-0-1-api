## application/serviceUnbindApp {#application-serviceunbindapp}

**基本信息：**

| 方法描述 | 共享服务查询已经绑定的应用列表 |
| --- | --- |
| 请求方法 | POST |
| API | application/serviceUnbindApp |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 共享服务查询已经绑定的应用列表 |
|  | 英文名称 | **Query application for services binded** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/ serviceUnbindApp?_=1410924373474

**参数：**AVMachineVO avm

**返回值：**Response r

r.data= List< VirtualSystemVO> vsvos