## application/getstypes/{appcode}/{srtype} {#application-getstypes-appcode-srtype}

**基本信息：**

| 方法描述 | 根据应用查询应用某种服务角色支持的服务类型 |
| --- | --- |
| 请求方法 | POST |
| API | application/serviceUnbindApp |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据应用查询应用某种服务角色支持的服务类型 |
|  | 英文名称 | **Queryservice type by service role type for one application** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/ serviceUnbindApp?_=1410924373474

**参数：**AVMachineVO avm

**返回值：**Response r

r.data= List< VirtualSystemVO> vsvos