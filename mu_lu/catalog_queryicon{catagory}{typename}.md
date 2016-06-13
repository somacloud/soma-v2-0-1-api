## catalog/ queryIcon/{catagory}/{typeName} {#catalog-queryicon-catagory-typename}

**基本信息：**

| 方法描述 | 加载服务、应用类型的图标 |
| --- | --- |
| 请求方法 | GET |
| API | catalog/ queryIcon/{catagory}/{typeName} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 加载服务、应用类型的图标 |
|  | 英文名称 | Load service, application icons |
| 是否记入事件 | 否 |

**Request URL:**

[http://127.0.0.1:7681/soma/rest/catalog/queryIcon/serviceType/IHS7](http://127.0.0.1:7681/appcloud/rest/catalog/download/applicationType/APP_UAP65)?sessionid=

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | catagory | applicationType serviceType | true | path variable |
| String | typeName | 应用类型名称 | true | path variable |

**返回值：**

**说明：**catagory取值为”applicationType”和”serviceType”