## service/bind {#service-bind}

**基本信息：**

| 方法描述 | 将服务绑定到应用 |
| --- | --- |
| 请求方法 | POST |
| API | service/bind |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 将服务绑定到应用 |
|  | 英文名称 | **Bind service to application** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/service/bind?_=1410924373474

**参数：**ServiceBindParam param

**返回值：**

**说明：**

ServiceBindParam的数据结构:

{ String appCode;

String[] servicesCode;

}

ServiceBindParam的数据实例:

| { |
| --- |