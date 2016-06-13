## swcatalog/get/{id} {#swcatalog-get-id}

**基本信息：**

| 方法描述 | 查询软件目录列表 |
| --- | --- |
| 请求方法 | GET |
| API | swcatalog/get/{id} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据编码查询软件类型 |
|  | 英文名称 | List software type by code |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/swcatalog/get/{name}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | name | SoftwareVO basic name | true | path variable |

**返回值：**SoftwareVO

**说明：**SoftwareVO见swcatalog/list