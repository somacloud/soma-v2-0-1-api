## service/checkConfigs {#service-checkconfigs}

**基本信息：**

| 方法描述 | 检查服务实例的配置是否需要更新（与目录中的类型对比） |
| --- | --- |
| 请求方法 | POST |
| API | service/checkConfigs |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 否 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 检查服务实例的配置是否需要更新（与目录中的类型对比） |
|  | 英文名称 | **Check service configurations with catalogs** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/service/ checkConfigs?_=1410924373474

**参数：**String code

**返回值：**List&lt;SimpleVO&gt;

**说明：** 返回需要更新的服务列表。

| SimpleVO数据结构 |
| --- |