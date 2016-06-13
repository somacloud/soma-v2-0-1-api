## account/unlock/{code} {#account-unlock-code}

**基本信息：**

| 方法描述 | 解锁租户 |
| --- | --- |
| 请求方法 | GET |
| API | account/unlock/{code} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 否 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 解锁租户 |
|  | 英文名称 | **Unlock the tenant** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/user/unlock/0001AA100000000050NT?_=1410922620851

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | code | AdminVO code | true | path variable |

**返回值：**

**说明：**AdminVO 见 account/lock/{code}