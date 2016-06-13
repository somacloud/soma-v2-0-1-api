## node/validateResources {#node-validateresources}

**基本信息：**

| 方法描述 | 校验多个节点是否可以指定给租户 |
| --- | --- |
| 请求方法 | POST |
| API | node/validateResources |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 否 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 校验多个节点是否可以指定给租户 |
|  | 英文名称 | Validate nodes for allocate to user |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/node/ validateResources?_=1410924373474

**参数：**String json

**返回值：**String message

**说明：**ComputerVO见node/list

Json为List&lt;ComputerVO&gt; cvos转换而成。