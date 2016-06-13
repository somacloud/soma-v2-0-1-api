## appcatalog/get/{name} {#appcatalog-get-name}

| 方法描述 | 根据名称查询应用类型 |
| --- | --- |
| 请求方法 | GET |
| API | appcatalog/get/{name} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据名称查询应用类型 |
|  | 英文名称 | List application type by name |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/appcatalog/get/{name}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | name | ApplicationTypeVO basic name | true | path variable |

**返回值：**Collection&lt;ApplicationTypeVO&gt;

**说明：**ApplicationTypeVO见appcatalog/list