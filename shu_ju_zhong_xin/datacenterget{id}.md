## datacenter/get/{id} {#datacenter-get-id}

**基本信息：**

| 方法描述 | 查询id查询数据中心 |
| --- | --- |
| 请求方法 | GET |
| API | datacenter /get/{id} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据编码查询数据中心 |
|  | 英文名称 | List data center by code |
| 是否记入事件 | 否 |

**Request URL:** http://127.0.0.1:7681/soma/rest/datacenter /get/{id}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | id | DataCenterVO code | true | path variable |

**返回值：**DataCenterVO

**说明：**DataCenterVO见space/list