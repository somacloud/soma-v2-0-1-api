## servicecatalog/get/{name} {#servicecatalog-get-name}

**基本信息：**

| 方法描述 | 根据名称查询服务类型 |
| --- | --- |
| 请求方法 | GET |
| API | servicecatalog/get/{name} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据名称查询服务类型 |
|  | 英文名称 | Listservice type by name |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/servicecatalog/get/{name}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | name | ServiceTypeVObasic name | true | path variable |

**返回值：**Collection&lt;ServiceTypeVO&gt;

**说明：**ServiceTypeVO见servicecatalog/list