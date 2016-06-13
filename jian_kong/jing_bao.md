## 警报

### alarm/list {#alarm-list}

**基本信息：**

| 方法描述 | 查询警报信息 |
| --- | --- |
| 请求方法 | POST |
| API | alarm/list |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询警报信息 |
|  | 英文名称 | Query alrams by condition |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/alarm/list?_=1410921917577

**参数：**AlarmRequestaq

**返回值：**Response r详细见node/listbypage

**说明：**r.data是List&lt;AlarmResponse&gt;