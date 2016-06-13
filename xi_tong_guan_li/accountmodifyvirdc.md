## account/modifyVirDC {#account-modifyvirdc}

**基本信息：**

| 方法描述 | 修改用户的虚拟数据中心 |
| --- | --- |
| 请求方法 | POST |
| API | account/modifyVirDC |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 否 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 修改用户的虚拟数据中心 |
|  | 英文名称 | **Update the vm data center of the tenant** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/account/modifyVirDC?_=1410924373474

**参数：**Collection&lt;AccountDCVO&gt; list

**返回值：**

**说明：**

AccountDCVO的数据结构

{ String code;

String accountCode;

String dcCode;

String dcName;

}