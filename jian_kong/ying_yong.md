## 应用

### monitorApplication/list {#monitorapplication-list}

**基本信息：**

| 方法描述 | 分页条件查询应用监控 |
| --- | --- |
| 请求方法 | POST |
| API | monitorApplication/list |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 分页条件查询应用监控 |
|  | 英文名称 | Query application monitors by page and condition |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/monitorApplication/list?_=1410921917577

**参数：**QueryClause qc详细见node/listbypage

**返回值：**Response r详细见node/listbypage

**说明：**r.data是Collection&lt;AppMonitorSystemStatistic&gt;

### monitorApplication/get/{id} {#monitorapplication-get-id}

**基本信息：**

| 方法描述 | 根据编码查询应用监控 |
| --- | --- |
| 请求方法 | GET |
| API | monitorApplication/get/{id} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据编码查询应用监控 |
|  | 英文名称 | Query application monitor by code |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/monitorApplication/get/{id}?_=1410921917577

**参数：**String code

**返回值：**Response r详细见node/listbypage

**说明：**r.data是AppMonitorSystemStatistic

### monitorApplication/startReal/{id} {#monitorapplication-startreal-id}

**基本信息：**

| 方法描述 | 启动实时监控 |
| --- | --- |
| 请求方法 | GET |
| API | monitorApplication/startReal/{id} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 启动实时监控 |
|  | 英文名称 | Start real time monitor |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/monitorApplication/startReal/{id}?_=1410921917577

**参数：**String code

**返回值：**Response r详细见node/listbypage

**说明：**r.data是BooleanstartFlag

### monitorApplication/stopReal/{id} {#monitorapplication-stopreal-id}

**基本信息：**

| 方法描述 | 停止实时监控 |
| --- | --- |
| 请求方法 | GET |
| API | monitorApplication/stopReal/{id} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 停止实时监控 |
|  | 英文名称 | Stop real time monitor |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/monitorApplication/stopReal/{id}?_=1410921917577

**参数：**String code

**返回值：**Response r详细见node/listbypage

**说明：**r.data是BooleanstartFlag