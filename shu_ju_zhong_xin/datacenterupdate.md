## datacenter/update {#datacenter-update}

**基本信息：**

| 方法描述 | 更新数据中心信息 |
| --- | --- |
| 请求方法 | POST |
| API | datacenter /update |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 否 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 更新数据中心信息 |
|  | 英文名称 | Update data center |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/datacenter/update?_=1410924373474

**参数：**Representation entity

**返回值：**无

**说明：**entity的格式为<key,value>，包含(code,code) (name,name)，其中code为DataCenterVO的字段code，Name 为DataCenterVO的字段name。DataCenterVO见space/list