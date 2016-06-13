## account/lock/{code} {#account-lock-code}

**基本信息：**

| 方法描述 | 锁定租户 |
| --- | --- |
| 请求方法 | GET |
| API | account/lock/{code} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 否 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 锁定租户 |
|  | 英文名称 | **Lock the tenant** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/user/lock/0001AA100000000050NT?_=1410921917577

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | code | AdminVO code | true | path variable |

**返回值：**

**说明：**AdminVO的数据结构:

{ String code;

String name;

String password;

String oldPassword;

Int type;

String email;

String accountCode;

String accountName;

Boolean logined;

String dataType = “user”;

String apikey;

String secretKey;

String state;

String pConfig;

UFDateTime lockedDate;

}

AdminVO的数据实例:

| { |
| --- |