## application/get/{id} {#application-get-id}

**基本信息：**

| 方法描述 | 根据编码查询应用信息 |
| --- | --- |
| 请求方法 | GET |
| API | application/get/{id} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据编码查询应用信息 |
|  | 英文名称 | **Query application by code** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/get/{id}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | id | Application code | true | path variable |

**返回值：**Application

**说明：** Application 见application/update