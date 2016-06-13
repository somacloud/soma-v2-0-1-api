## user/ setUser/{code} {#user-setuser-code}

**基本信息：**

| 方法描述 | 将管理员设为系统用户 |
| --- | --- |
| 请求方法 | GET |
| API | user/setUser/{code} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 否 |
|  | 系统用户 | 否 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 将管理员设为系统用户 |
|  | 英文名称 | **Set the admin user to normal user** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/user/setUser/{code}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | code | AdminVO code | true | path variable |

**返回值：**

**说明：**AdminVO 见 account/lock/{code}