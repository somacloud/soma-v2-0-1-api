## catalog/download/{type}/{fileName} {#catalog-download-type-filename}

**基本信息：**

| 方法描述 | 下载目录中的软件、服务、应用 |
| --- | --- |
| 请求方法 | GET |
| API | catalog/download/{type}/{fileName} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 下载目录中的软件、服务、应用 |
|  | 英文名称 | Download software type,service type, application type |
| 是否记入事件 | 是 |

**Request URL:**

[http://127.0.0.1:7681/soma/rest/catalog/download/applicationType/APP_UAP65](http://127.0.0.1:7681/appcloud/rest/catalog/download/applicationType/APP_UAP65)? sessionid=

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | type | applicationTypeserviceType | true | path variable |
| String | name | 应用类型 | true | path variable |

**返回值：**

**说明：**type取值为”applicationType”和”serviceType”