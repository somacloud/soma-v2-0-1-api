## 模板

### monitorPresent/listPresent {#monitorPresent-listPresent}

**基本信息：**

| 方法描述 | 查询所有模板列表 |
| --- | --- |
| 请求方法 | POST |
| API | monitorPresent/listPresent |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询所有模板列表 |
|  | 英文名称 | List all presents |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/monitorPresent/listPresent?_=1410921917577

**参数：**null

**返回值：**Response r详细见node/listbypage

**说明：**r.HashMap&lt;String, List&lt;PresentVO&gt;&gt;

### monitorPresent/listInstancePresent {#monitorPresent-listInstancePresent}

**基本信息：**

| 方法描述 | 查询该实例的所有模板列表 |
| --- | --- |
| 请求方法 | POST |
| API | monitorPresent/listInstancePresent |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询该实例的所有模板列表 |
|  | 英文名称 | List all presents by instanceCode |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/monitorPresent/listInstancePresent?_=1410921917577

**参数：**String code

**返回值：**Collection&lt;PresentTmplVO&gt;

### monitorPresent/getDfDashboard {#monitorPresent-getDfDashboard}

**基本信息：**

| 方法描述 | 查询某实例的首页看板配置|
| --- | --- |
| 请求方法 | POST |
| API | monitorPresent/getDfDashboard |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询某实例的首页看板配置 |
|  | 英文名称 | Query dashboard config by request |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/monitorPresent/getDfDashboard?_=1410921917577

**参数：**MonitorConfigRequest

"MonitorConfigRequest request"

| 参数名 | 类型 | 描述 |
| --- | --- | --- |
| resCode | String | 实例code |
| resType | String | 实例类型 |
| fillData | Boolean | 是否对配置进行模板填充，若要读取配置生成页面则为true,若为编辑查看则false |

**返回值：**DashboardVO

**说明：**

MonitorConfigRequest的数据结构:

{ int operation = QUERY; **QUERY = 0,EDIT = 1,CHECKEXITS = 2

String resCode;

String resType;

Env env;

PresentVO present;

PerformanceVO performance;

DashboardVO dashboard;

boolean fillData = true;

TemplateVO tmpl;

String presentCode;

boolean all;

boolean shared = false;

String monitorType;

String downloadCode;

String downloadName;

}

PresentVO的数据结构：
{ String code;

String name;

String desc;

Performance dashboard;

Snapshot snapshot;

Performance performance;

Analysis analysis;

String ts;

}

PresentVO的数据结构：
{ String resType;

String resCode;

String type;

String command;

List&lt;Metric&gt;  metrics

}
