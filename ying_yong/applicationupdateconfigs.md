## application/updateConfigs {#application-updateconfigs}

**基本信息：**

| 方法描述 | 升级应用实例（与应用类型的配置信息对比变化） |
| --- | --- |
| 请求方法 | POST |
| API | application/updateConfigs |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 升级应用实例（与应用类型的配置信息对比变化） |
|  | 英文名称 | **Update application configurations** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/updateConfigs?_=1410924373474

**参数：**List&lt;SimpleVO&gt; svos

**返回值：**List&lt;String&gt; appNames

| SimpleVO对象 |
| --- |