## 任务

### task/listbypage {#task-listbypage}

**基本信息：**

| 方法描述 | 分页条件查询任务 |
| --- | --- |
| 请求方法 | POST |
| API | task/listbypage |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 分页条件查询任务 |
|  | 英文名称 | Query task by page and condition |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/task/listbypage?_=1410921917577

**参数：**QueryClause qc详细见node/listbypage

**返回值：**Response r详细见node/listbypage

**说明：**r.data是Collection&lt;TaskVO&gt;