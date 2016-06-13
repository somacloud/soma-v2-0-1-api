## service/start/{code} {#service-start-code}

**基本信息：**

| 方法描述 | 启动服务 |
| --- | --- |
| 请求方法 | GET |
| API | service/start/{code} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是，（只能操作新增的停止的服务） |
|  | 系统用户 | 是 |
|  | 租户用户 | 是，（只能操作用户自己新增的停止的服务） |
| 多语 | 中文名称 | 启动服务 |
|  | 英文名称 | **Startservice** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/service/start/{code}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | code | Service code | true | path variable |

**返回值：**

**说明：**Service vo 见service/get/{code}