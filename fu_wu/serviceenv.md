## service/env {#service-env}

**基本信息：**

| 方法描述 | 查询服务环境变量 |
| --- | --- |
| 请求方法 | POST |
| API | service/env |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询服务环境变量 |
|  | 英文名称 | **Queryservice environment** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/service/env?_=1410924373474

**参数：**String code

**返回值：**List&lt;ConfigOptionVO&gt;

**说明：**Service code 见service/get/{code}