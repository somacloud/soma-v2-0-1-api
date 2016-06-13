## datacenter/delete/{id} {#datacenter-delete-id}

**基本信息：**

| 方法描述 | 根据id删除数据中心 |
| --- | --- |
| 请求方法 | POST |
| API | datacenter /delete |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 否 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 删除数据中心 |
|  | 英文名称 | Delete data center |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/datacenter/delete/{id}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | id | DataCenterVO code | true | path variable |

**返回值：**

**说明：**DataCenterVO见space/list