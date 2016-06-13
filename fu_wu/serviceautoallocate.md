## service/autoAllocate {#service-autoallocate}

**基本信息：**

| 方法描述 | 服务自动分配到主机 |
| --- | --- |
| 请求方法 | POST |
| API | service/autoAllocate |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 否 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 服务自动分配到主机 |
|  | 英文名称 | **Allocate service to machine** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/service/autoAllocate?_=1410924373474

**参数：**List&lt;Service&gt; svos

**返回值：** List&lt;Service&gt; svos