## service/stop/{code} {#service-stop-code}

**基本信息：**

| 方法描述 | 停止服务 |
| --- | --- |
| 请求方法 | GET |
| API | service/stop/{code} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是，（只能操作新增的启动的服务） |
|  | 系统用户 | 是 |
|  | 租户用户 | 是，（只能操作用户自己新增的启动的服务） |
| 多语 | 中文名称 | 停止服务 |
|  | 英文名称 | **Stopservice** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/service/stop/{code}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | code | Service code | true | String variable |

**返回值：**

**说明：**Service vo 见service/get/{code}