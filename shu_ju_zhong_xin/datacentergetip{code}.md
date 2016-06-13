## datacenter/getip/{code} {#datacenter-getip-code}

**基本信息：**

| 方法描述 | 根据数据中心编码获取对应的控制器ip信息 |
| --- | --- |
| 请求方法 | GET |
| API | datacenter/getip/{code} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 否 |
|  | 系统用户 | 否 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 根据数据中心编码获取对应的控制器ip信息 |
|  | 英文名称 | Get the controller and redis ip of the datacenter. |
| 是否记入事件 | 否 |

**Request URL:**

[http://localhost/soma/rest/datacenter/getip/{code}?_=1445331142563](http://localhost/soma/rest/datacenter/getip/%7bcode%7d?_=1445331142563)

**参数：**数据中心编码。

**返回值：**Collection&lt;DCDetailVO&gt;

DCDetailVO对象定义见datacenter/updateip。