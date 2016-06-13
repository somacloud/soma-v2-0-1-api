## node/listbypage {#node-listbypage}

**基本信息：**

| 方法描述 | 分页查询主机信息 |
| --- | --- |
| 请求方法 | POST |
| API | node/ listbypage |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 分页查询主机信息 |
|  | 英文名称 | List hosts by page |
| 是否记入事件 | 否 |

**Request URL:**

http:// 127.0.0.1/soma/rest/node/listbypage?_=1415861213191

**参数：**QueryClause qc

| { |
| --- |

QueryClause对象：

| 字段 | 类型 | 描述 |
| --- | --- | --- |
| pageSize | int | 每页显示条数 |
| pageIndex | int | 第几页 |
| queryCount | boolean | 是否分页 |
| matchCriterias | List&lt;MatchCriteria&gt; | 多条件查询条件对象 |
| orders | List&lt;Order&gt; | 排序对象 |

MatchCriteria对象、

| 字段 | 类型 | 描述 |
| --- | --- | --- |
| value | String | 值 |
| column | String | 列名称 |
| matchType | String | 匹配类型 |
| display | String |  |
| dataType | String | 数据类型 |
| caseSensitive | Boolean | 是否大小写敏感 |

Order对象、

| 字段 | 类型 | 描述 |
| --- | --- | --- |
| column | String | 总页数 |
| ascending | String | 当前页 |

**返回值：**Response

Response对象：

| 字段 | 类型 | 描述 |
| --- | --- | --- |
| code | String | Pk |
| message | String | 描述信息 |
| data | Object | 返回数据列表 |
| dataCount | int | 满足条件的数据总条数 |
| taskId | String | 任务ID |
| showType | int | 前台展示形式0：alert；1：confirm |
| pageCount | int | 总页数 |
| pageIndex | int | 当前页 |
| pageSize | int | 总页数 |