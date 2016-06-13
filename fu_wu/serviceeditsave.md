## service/editSave {#service-editsave}

**基本信息：**

| 方法描述 | 编辑服务 |
| --- | --- |
| 请求方法 | POST |
| API | service/editSave |
| 权限 | 系统管理员 | 是, |
|  | 租户管理员 | 是,（租户的服务） |
|  | 系统用户 | 是 |
|  | 租户用户 | 是，（租户用户自己创建的服务） |
| 多语 | 中文名称 | 编辑服务 |
|  | 英文名称 | Edit service |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/service/editSave?_=1410924373474

**参数：**Service vo

**返回值：无**

**说明：**Service vo 见service/get/{code}