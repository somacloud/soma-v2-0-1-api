## service/queryService/{code} {#service-queryservice-code}

**基本信息：**

| 方法描述 | 根据编码查询服务和服务实例信息 |
| --- | --- |
| 请求方法 | GET |
| API | service/queryService/{code} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据编码查询服务和服务实例信息 |
|  | 英文名称 | query all service information by code |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/service/queryService/{code}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | code | Service code | true | path variable |

**返回值：**AVMachineVO avm

**说明：**avm.serviceInstanceVO=Service svo