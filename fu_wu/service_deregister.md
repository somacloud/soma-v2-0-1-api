## service/ deregister {#service-deregister}

**基本信息：**

| 方法描述 | 反注册服务 |
| --- | --- |
| 请求方法 | POST |
| API | service/deregister |
| 权限 | 系统管理员 | 是, |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 反注册服务 |
|  | 英文名称 | **Deregisterservice** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/service/deregister?_=1410924373474

**参数：**String code

**返回值：**

**说明：**Service code 见service/get/{code}