## application/appstatistics {#application-appstatistics}

**基本信息：**

| 方法描述 | 应用的状态汇总 |
| --- | --- |
| 请求方法 | POST |
| API | application/appstatistics |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 应用的状态汇总查询 |
|  | 英文名称 | **Query application status summry** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/ appstatistics?_=1410924373474

**参数：**AVMachineVO avm

**返回值：**NumberStatisticsVO mvo

| NumberStatisticsVO的数据结构: |
| --- |