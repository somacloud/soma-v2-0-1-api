## node/validateResource {#node-validateresource}

**基本信息：**

| 方法描述 | 校验单个节点资源 |
| --- | --- |
| 请求方法 | POST |
| API | node/validateResource |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 否 |
|  | 系统用户 | 否 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 校验单个节点资源 |
|  | 英文名称 | Validate node for limit resource |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/node/ validateResource?_=1410924373474

**参数：**String json

**返回值：**String message

**说明：**ComputerVO见node/list

Json的结构：{“code”:machineCode,”actionType”:actionType}