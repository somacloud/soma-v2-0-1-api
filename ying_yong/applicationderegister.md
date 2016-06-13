## application/deregister {#application-deregister}

**基本信息：**

| 方法描述 | 反注册应用 |
| --- | --- |
| 请求方法 | POST |
| API | application/deregister |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 反注册应用 |
|  | 英文名称 | **Deregister Application** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/deregister?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | id | Application code | true | path variable |

**返回值：code**

**说明：**Application 见application/update