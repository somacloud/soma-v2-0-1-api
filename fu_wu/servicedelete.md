## service/delete {#service-delete}

**基本信息：**

| 方法描述 | 根据id删除服务 |
| --- | --- |
| 请求方法 | POST |
| API | service/delete |
| 权限 | 系统管理员 | 是, |
|  | 租户管理员 | 是,（租户的服务） |
|  | 系统用户 | 是 |
|  | 租户用户 | 是，（租户用户自己创建的服务） |
| 多语 | 中文名称 | 删除服务 |
|  | 英文名称 | Delete service |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/service/delete?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | code | Service code | true | path variable |

**返回值：**

**说明：**Service vo 见service/get/{code}