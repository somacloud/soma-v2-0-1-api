## node/update {#node-update}

**基本信息：**

| 方法描述 | 更新主机信息 |
| --- | --- |
| 请求方法 | POST |
| API | node/update |
| 权限 | 系统管理员 | 是，更新所有节点 |
|  | 租户管理员 | 是，只能更新租户下的节点 |
|  | 系统用户 | 否 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 更新主机信息 |
|  | 英文名称 | Update hostinformation |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/node/update?_=1410924373474

参数：**ComputerVO vo**

返回值：

说明：**ComputerVO** 见node/list