## patchhistory/listbypage {#patchhistory-listbypage}

**基本信息：**

| 方法描述 | 分页查询补丁历史列表 |
| --- | --- |
| 请求方法 | GET |
| API | patchhistory/listbypage |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 分页查询补丁历史列表 |
|  | 英文名称 | **Query history patchs by page** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/ patchhistory /listbypage?_=1410924373474

**参数：**QueryClause qc例：{pageSize:18, pageIndex:1, queryCount:true, params:{keyword:aa, pagi:true}}。“keyword”的值是输入值

**返回值：**Response

**说明：**Response对象参考node/listbypage