## application/migrate {#application-migrate}

**基本信息：**

| 方法描述 | 迁移应用的中间件服务 |
| --- | --- |
| 请求方法 | POST |
| API | application/migrate |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 迁移应用的中间件服务 |
|  | 英文名称 | **Migrate middleware server to other node** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/migrate?_=1410924373474

**参数：**String json

| {“appCode”:”XXXXXXXXXXXX”, |
| --- |

**返回值：**Response r

r.taskId=taskCode