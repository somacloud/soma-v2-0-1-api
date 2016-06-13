## application/listbycondition {#application-listbycondition}

**基本信息：**

| 方法描述 | 根据条件查询应用信息 |
| --- | --- |
| 请求方法 | POST |
| API | application/ listbycondition |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据条件查询应用信息 |
|  | 英文名称 | **Query applications by clause** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma /rest/application/listbycondition?_=1415951729697

**参数：**String json

"{\"isFillAvm\":true,\"isFillAuth\":true,\"pageInfo\":{\"pageSize\":10,\"pageIndex\":1}}"

| 参数名 | 类型 | 描述 |
| --- | --- | --- |
| vsvo | VirtualSystemVO对象 |  |
| pageInfo | QueryClause对象 | 需要分页时传入该参数 |
| isFullfill | Boolean | 返回的应用对象填充：应用的所有服务对象，应用的权限信息，应用的对应的实例对象，应用的类型对象，应用的监控信息 |
| isFillAuth | Boolean | 应用填充：应用的权限信息 |
| isFillAvm | Boolean | 应用填充：应用的所有服务对象 |
| isFillInst | Boolean | 应用填充：应用的对应的实例对象 |
| isFillType | Boolean | 应用填充：应用的类型对象 |
| isFillStatistic | Boolean | 应用填充：应用的监控信息 |

**返回值：**Response详细见node/listbypage