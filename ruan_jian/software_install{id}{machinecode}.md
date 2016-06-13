## software /install/{id}/{machineCode} {#software-install-id-machinecode}

**基本信息：**

| 方法描述 | 安装软件 |
| --- | --- |
| 请求方法 | GET |
| API | software/install/{id}/{machineCode} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 安装软件 |
|  | 英文名称 | Install software |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/software/install/{id}/{machineCode}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | id | SoftwareVO code | true | path variable |
| String | machineCode | ComputerVO code |  |  |

**返回值：**

**说明：**SoftwareVO对象定义见swcatalog/list，ComputerVO对象定义见node/list