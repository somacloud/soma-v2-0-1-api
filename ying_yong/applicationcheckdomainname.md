## application/checkDomainName {#application-checkdomainname}

**基本信息：**

| 方法描述 | 检查域名是否合法 |
| --- | --- |
| 请求方法 | POST |
| API | application/checkDomainName |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 检查域名是否合法 |
|  | 英文名称 | **Validate domainName** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/checkDomainName?_=1410924373474

**参数：**code是应用编码，domainName是应用的域名

| {“code”:”XXXXXXAppcodeXXXX” |
| --- |

**返回值：** Boolean