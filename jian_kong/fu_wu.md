## 服务

### monitorService/list {#monitorservice-list}

**基本信息：**

| 方法描述 | 分页条件查询服务监控 |
| --- | --- |
| 请求方法 | POST |
| API | monitorService/list |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 分页条件查询服务监控 |
|  | 英文名称 | Query service monitors by page and condition |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/monitorService/list?_=1410921917577

**参数：**QueryClause qc详细见node/listbypage

**返回值：**Response r详细见node/listbypage

**说明：**r.data是Collection&lt;AppMonitorStatistic&gt;

### monitorEnv/query {#monitorenv-query}

**基本信息：**

| 方法描述 | 查询服务监控的配置信息 |
| --- | --- |
| 请求方法 | POST |
| API | monitorEnv/query |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询服务监控的配置信息 |
|  | 英文名称 | Query service monitor configuration |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/monitorEnv/query?_=1410921917577

**参数：**Stringjson

**返回值：**AppMonitorStatistic avo

**说明：**r.data是Collection&lt;AppMonitorStatistic&gt;