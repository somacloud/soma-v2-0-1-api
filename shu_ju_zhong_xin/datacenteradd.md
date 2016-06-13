## datacenter/add {#datacenter-add}

**基本信息：**

| 方法描述 | 增加数据中心 |
| --- | --- |
| 请求方法 | POST |
| API | datacenter /add |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 否？（租户管理员可以新增物理数据中心，然后注册自己的主机过来） |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 新增数据中心 |
|  | 英文名称 | Add data center |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/datacenter/add?_=1410924373474

**参数：**Representation entity

**返回值：**

**说明：**entity为<key,value>，格式为(name,name)。其中，Name为DataCenterVO的字段name，DataCenterVO见space/list