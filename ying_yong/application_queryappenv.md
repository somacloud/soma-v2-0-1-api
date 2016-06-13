## application /queryAppEnv {#application-queryappenv}

**基本信息：**

| 方法描述 | 查询应用环境变量 |
| --- | --- |
| 请求方法 | POST |
| API | application/queryAppEnv |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询应用环境变量 |
|  | 英文名称 | **Query application environmentvariables** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/queryAppEnv?_=1410924373474

**参数：**String code

**返回值：**List&lt;ConfigOptionVO&gt;

**说明：**VirtualSystemVO code见application/list