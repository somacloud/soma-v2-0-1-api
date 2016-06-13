## account/add {#account-add}

**基本信息：**

| 方法描述 | 新增租户 |
| --- | --- |
| 请求方法 | POST |
| API | account/add |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 否 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 新增租户 |
|  | 英文名称 | **Add tenant account** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/account/add?_=1410924373474

**参数：**AccountVO avo

**返回值：**AccountVO avo

**说明：**AccountVO对象

| 字段名称 | 类型 | 描述 |
| --- | --- | --- |
| code | String |  |
| name | String |  |
| type | Int | 类型 |
| renterMaxAppNum | int | 租户最大应用数目 |
| renterMaxCPUNum | int | 租户最大CPU数目 |
| renterMaxMemNum | long | 租户最大内存数目 |
| renterMaxNodeNum | int | 租户最大节点数目 |
| renterMaxPrimaryStorage | int | 租户最大存储 |
| contractCode | String |  |
| contractMakeTime | String |  |
| contractMakerName | String |  |
| contractMakerEmail | String |  |
| adminAccCode | String | 管理员编码 |
| adminAccName | String |  |
| state | String |  |
| logined | boolean |  |
| lockedDate | UFDateTime |  |
| dataType | String |  |
| hostTotalTime | long |  |
| appTotalTime | long |  |
| allocateMemSize | String |  |
| allocateCpuSize | String |  |
| allocateDiskSize | String |  |
| users | List&lt;AdminVO&gt; | 租户的用户列表 |
| computers | List&lt;ComputerVO&gt; | 租户的主机列表 |
| applications | Collection&lt;VirtualSystemVO&gt; | 租户的应用列表 |
| accountDcList | List&lt;AccountDCVO&gt; | 租户的可用数据中心列表 |