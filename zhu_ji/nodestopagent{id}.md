## node/stopagent/{id} {#node-stopagent-id}

**基本信息：**

| 方法描述 | 主机停止Agent |
| --- | --- |
| 请求方法 | GET |
| API | node/stopagent/{id} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 否(只有重启功能) |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 停止Agent |
|  | 英文名称 | Stop Agent |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/node/stopagent/{id}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | id | ComputerVO code | true | path variable |

**返回值：**

**说明：**ComputerVOcode见node/list