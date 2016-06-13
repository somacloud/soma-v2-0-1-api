## application/materialize/{id} {#application-materialize-id}

**基本信息：**

| 方法描述 | 物化应用 |
| --- | --- |
| 请求方法 | GET |
| API | application/materialize/{id} |
| 权限 | 系统管理员 | 是，编辑所有非注册应用 |
|  | 租户管理员 | 是，编辑租户下的所有非注册应用 |
|  | 系统用户 | 是，编辑所有非注册应用 |
|  | 租户用户 | 是，编辑用户创建的所有非注册应用 |
| 多语 | 中文名称 | 物化应用 |
|  | 英文名称 | **Materializeapplication** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/materialize /{id}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | id | Application code | true | path variable |

**返回值：**

**说明：**Application 见application/update