## appIication/allocAppToTenant {#appiication-allocapptotenant}

**基本信息：**

| 方法描述 | 分配应用给租户 |
| --- | --- |
| 请求方法 | POST |
| API | application/allocAppToTenant |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 否 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 分配应用给租户 |
|  | 英文名称 | **Allocate application to tenant** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/allocAppToTenant?_=1410924373474

**参数：**String json

**返回值：**

**说明：**VirtualSystemVO见application/list

Json的格式：{“vcCode”:vcCode;”accCode”:accCode}

vcCode为VirtualSystemVO code

accCode为AccountVO code