## node/updatetag {#node-updatetag}

**基本信息：**

| 方法描述 | 更新主机的标签 |
| --- | --- |
| 请求方法 | POST |
| API | node/updatetag |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 用户 | 是 |
| 多语 | 中文名称 | 查询用户的所有主机的编码 |
|  | 英文名称 |  |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/node/ updatetag?_=1410924373474

**参数：**ComputerVO vo

vo.code=nodeid;

vo.tag=newtag;

**返回值：**无

**说明：**