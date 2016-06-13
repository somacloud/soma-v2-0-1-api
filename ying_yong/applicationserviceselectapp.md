## application/serviceSelectApp {#application-serviceselectapp}

**基本信息：**

| 方法描述 | 查询服务可以绑定的应用 |
| --- | --- |
| 请求方法 | POST |
| API | application/serviceSelectApp |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询服务可以绑定的应用 |
|  | 英文名称 | **Search applications for service to bind** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/ serviceSelectApp?_=1410924373474

**参数：**AVMachineVO avm

**返回值：**Response r

r.data= List< VirtualSystemVO> vsvos