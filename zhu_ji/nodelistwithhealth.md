## node/listwithhealth {#node-listwithhealth}

**基本信息：**

| 方法描述 | 根据条件查询主机信息和其监控信息 |
| --- | --- |
| 请求方法 | POST |
| API | node/listwithhealth |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据条件查询主机信息和其监控信息 |
|  | 英文名称 | List hosts by condition |
| 是否记入事件 | 否 |

**Request URL:**

http:// 127.0.0.1/soma/rest/node/listwithhealth?_=1415860384829

**参数：**String json

例：{“code”:”XXX”,”dccode”:”XXX”}

**返回值：**Collection&lt;ComputerVO&gt; vos

**说明：**ComputerVO见node/list