## datacenter/updaterepo/ {#datacenter-updaterepo}

**基本信息：**

| 方法描述 | 设置数据中心的软件源信息 |
| --- | --- |
| 请求方法 | POST |
| API | datacenter/updaterepo |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 否 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 设置数据中心的软件源 |
|  | 英文名称 | Setsoftware repo for data center |
| 是否记入事件 | 是 |

**Request URL:**

**http://127.0.0.1/soma/rest/datacenter/updaterepo?_=1415846379453**

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| DataCenterVO | dvo | DataCenterVO对象，在前台组织好数据，在后台直接保存 | true | path variable |

**返回值：无**

**说明：**DataCenterVO见space/list