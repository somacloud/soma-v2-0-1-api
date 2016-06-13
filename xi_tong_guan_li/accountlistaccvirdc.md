## account/listAccVirDC {#account-listaccvirdc}

**基本信息：**

| 方法描述 | 查询用户的虚拟数据中心 |
| --- | --- |
| 请求方法 | GET |
| API | account/listAccVirDC |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询用户的虚拟数据中心 |
|  | 英文名称 | **Query the vm data center of the tenant** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/account/listAccVirDC?_=1410924373474

**参数：**

**返回值：** AccountDCVO[]

**说明：**AccountDCVO见account/modifyVirDc