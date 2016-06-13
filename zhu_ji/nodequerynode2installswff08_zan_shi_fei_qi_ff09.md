## node/queryNode2InstallSw（暂时废弃） {#node-querynode2installsw}

**基本信息：**

| 方法描述 | 查询可安装软件的节点列表 |
| --- | --- |
| 请求方法 | POST |
| API | node/queryNode2InstallSw |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 用户 | 是 |
| 多语 | 中文名称 | 查询可安装软件的节点列表 |
|  | 英文名称 |  |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/node/queryNode2InstallSw?_=1410924373474

**参数：**SoftwareVO svo

**返回值：**List< ComputerVO>

**说明：**ComputerVO 见node/list