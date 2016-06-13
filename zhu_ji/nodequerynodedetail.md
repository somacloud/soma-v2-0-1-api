## node/queryNodeDetail {#node-querynodedetail}

**基本信息：**

| 方法描述 | 根据编码查询节点信息 |
| --- | --- |
| 请求方法 | POST |
| API | node/queryNodeDetail |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据编码查询节点信息 |
|  | 英文名称 | Queryhost by code |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/node/queryNodeDetail?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | id | ComputerVOcode | true | path variable |

**返回值：**ComputerVO

**说明：**ComputerVO见node/list