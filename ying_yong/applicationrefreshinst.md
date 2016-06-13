## application/refreshInst {#application-refreshinst}

**基本信息：**

| 方法描述 | 刷新单个应用实例 |
| --- | --- |
| 请求方法 | POST |
| API | application/refreshInst |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 刷新单个应用实例 |
|  | 英文名称 | **Refresh one application** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/refreshInst?_=1410924373474

**参数：**String appCode

**返回值：**VirtualSystemVO vsvo（含有avms）