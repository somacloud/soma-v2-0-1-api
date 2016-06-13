## node/connectTest/{nodeid} {#node-connecttest-nodeid}

**基本信息：**

| 方法描述 | 测试节点是否联通 |
| --- | --- |
| 请求方法 | GET |
| API | node/connectTest/{nodeid} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 用户 | 是 |
| 多语 | 中文名称 | 测试节点是否联通 |
|  | 英文名称 |  |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/node/ connectTest/{nodeid}?_=1410924373474

**参数：**Nodeid：节点的编码

**返回值：**Response r; r.data=computerVO cvo。

Cvo中有主机的最新的链接状态。

**说明：**