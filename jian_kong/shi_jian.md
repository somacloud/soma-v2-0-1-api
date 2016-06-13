## 事件

### event/list {#event-list}

**基本信息：**

| 方法描述 | 分页查询所有事件 |
| --- | --- |
| 请求方法 | POST |
| API | event/list |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询所有事件 |
|  | 英文名称 | **Query all events** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/event/list?_=1410921917577

**参数：**QueryClause qc详细见node/listbypage

**返回值：**Response r详细见node/listbypage

**说明：**r.data是 List&lt;OperationLogVO&gt;

OperationLogVO的数据结构:

{ String code;

String name;

String operationlog;

String ip;

Long cost;

String agent;

}

OperationLogVO的数据实例:

| [{ |
| --- |

### event/listbypage {#event-listbypage}

**基本信息：**

| 方法描述 | 分页条件查询事件 |
| --- | --- |
| 请求方法 | POST |
| API | event/listbypage |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 分页条件查询事件 |
|  | 英文名称 | **Query events by page and condition** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/event/listbypage?_=1410921917577

**参数：**QueryClause qc详细见node/listbypage

**返回值：**Response r详细见node/listbypage

**说明：**r.data是 List&lt;OperationLogVO&gt;