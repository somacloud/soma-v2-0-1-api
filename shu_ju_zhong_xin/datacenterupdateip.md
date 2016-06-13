## datacenter/updateip {#datacenter-updateip}

**基本信息：**

| 方法描述 | 更新数据中心的控制端IP |
| --- | --- |
| 请求方法 | POST |
| API | datacenter/updatetag |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 否 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 更新数据中心的控制端IP |
|  | 英文名称 | Update the controller and redis ip of the datacenter |
| 是否记入事件 | 是 |

**Request URL:**

**http://127.0.0.1/soma/rest/datacenter/updateip?_=1415846379453**

**参数：**List&lt;DCDetailVO&gt; dcdvos

| 字段名称 | 字段类型 | 描述 |
| --- | --- | --- |
| code | String |  |
| dcCode | String |  |
| key | String |  |
| value | String |  |

参数例子：

| [{ |
| --- |

**返回值：无**