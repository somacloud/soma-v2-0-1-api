## 虚机模板

### vmpolicy/get/{id} {#vmpolicy-get-id}

**基本信息：**

| 方法描述 | 根据编码查询虚机模板 |
| --- | --- |
| 请求方法 | GET |
| API | vmpolicy/get/{id} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据编码查询虚机模板 |
|  | 英文名称 | **Query vm template by code** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/vmpolicy/get/{id}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | id | VMPolicy code | true | path variable |

**返回值：**VMPolicyVO

**说明：**VMPolicyVO的数据结构:

{ String code;

String name;

String hypervisor;

String dcCode;

String tmplCode;

String serviceCode;

String networkCode;

String systemCode;

String osName;

Int cpuCount;

String cpuFrq;

String memSize;

String memSpeed;

String networkName;

String description;

String accountCode;

String accountName;

String creatorCode;

String creatorName;

Int authType;

String serviceDescription;

String tmplName;

String dcName;

String username;

String password;

String oldPassword;

}

VMPolicyVO的数据实例:

| { |
| --- |

### vmpolicy/list {#vmpolicy-list}

**基本信息：**

| 方法描述 | 查询所有虚机模板 |
| --- | --- |
| 请求方法 | GET |
| API | vmpolicy/list |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询所有虚机模板 |
|  | 英文名称 | **Query all vm templates** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/vmpolicy/list?_=1410924373474

**参数：**

**返回值：**Collection&lt;VMPolicyVO&gt;

**说明：**VMPolocyVO见vmpolicy/get/{id}

### vmpolicy/listbydctype/{type} {#vmpolicy-listbydctype-type}

**基本信息：**

| 方法描述 | 根据数据中心类型查询所有虚机模板 |
| --- | --- |
| 请求方法 | GET |
| API | vmpolicy/listbydctype/{type} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据数据中心类型查询所有虚机模板 |
|  | 英文名称 | **Query vm templates by date center type** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/vmpolicy/listbydctype/{type}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | type | DataCenterVO dcType | true | path variable |

**返回值：**Collection&lt;VMPolicyVO&gt;

**说明：**VMPolocyVO见vmpolicy/get/{id} DataCenterVO见datacenter/list

### vmpolicy/listbydccode/{code} {#vmpolicy-listbydccode-code}

**基本信息：**

| 方法描述 | 根据数据中心id查询所有虚机模板 |
| --- | --- |
| 请求方法 | GET |
| API | vmpolicy/listbydccode/{code} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据数据中心id查询所有虚机模板 |
|  | 英文名称 | **Query vm templates by date center code** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/vmpolicy/listbydctype/{code}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | type | DataCenterVO code | true | path variable |

**返回值：**Collection&lt;VMPolicyVO&gt;

**说明：**VMPolocyVO见vmpolicy/get/{id} DataCenterVO参考datacenter/list

### vmpolicy/search {#vmpolicy-search}

**基本信息：**

| 方法描述 | 根据用户查询所有虚机模板 |
| --- | --- |
| 请求方法 | GET |
| API | vmpolicy/search |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据用户查询所有虚机模板 |
|  | 英文名称 | **Query all vm templates by user** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/vmpolicy/search?_=1410924373474

**参数：**

**返回值：**Collection&lt;VMPolicyVO&gt;

**说明：**VMPolocyVO见vmpolicy/get/{id}

### vmpolicy/search/{json} {#vmpolicy-search-json}

**基本信息：**

| 方法描述 | 根据关键字查询所有虚机模板 |
| --- | --- |
| 请求方法 | POST |
| API | vmpolicy/search/{json} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据关键字查询所有虚机模板 |
|  | 英文名称 | **Query vm templates by keyword** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/vmpolicy/search/{json}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | json | 关键字 | true | path variable |

**返回值：**Collection&lt;VMPolicyVO&gt;

**说明：**VMPolocyVO见vmpolicy/get/{id}

### vmpolicy/update {#vmpolicy-update}

**基本信息：**

| 方法描述 | 更新虚机模板 |
| --- | --- |
| 请求方法 | POST |
| API | vmpolicy/update |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是，自己创建的模板 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 更新虚机模板 |
|  | 英文名称 | **Update vm template** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/vmpolicy/update?_=1410924373474

**参数：**VMPolicyVO vo

**返回值：**VMPolicyVO vo

**说明：**VMPolocyVO见vmpolicy/get/{id}

### vmpolicy/add {#vmpolicy-add}

**基本信息：**

| 方法描述 | 创建虚机模板 |
| --- | --- |
| 请求方法 | POST |
| API | vmpolicy/add |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 创建虚机模板 |
|  | 英文名称 | **Create vm template** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/vmpolicy/add?_=1410924373474

**参数：**VMPolicyVO vo

**返回值：** VMPolicyVO

**说明：**VMPolocyVO见vmpolicy/get/{id}

### vmpolicy/delete/{id} {#vmpolicy-delete-id}

**基本信息：**

| 方法描述 | 删除虚机模板 |
| --- | --- |
| 请求方法 | GET |
| API | vmpolicy/delete/{id} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 删除虚机模板 |
|  | 英文名称 | **Delete vm template** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/vmpolicy/delete/{id}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | id | VMPolicyVO code | true | path variable |

**返回值：**

**说明：**VMPolocyVO见vmpolicy/get/{id}

### vmpolicy/shared {#vmpolicy-shared}

**基本信息：**

| 方法描述 | 分享虚机模板 |
| --- | --- |
| 请求方法 | POST |
| API | vmpolicy/shared |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是，只能分享自己新建的模板 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 分享虚机模板 |
|  | 英文名称 | **Share vm template** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/vmpolicy /shared?_=1410924373474

**参数：**String json

例："{\"tmplcode\":\"0001AA1000000000TFIX\",\"users\":\"0001AA10000000003YRF"}"

**返回值**：无

**说明：**参数json是一个由对象转换出来的字符串

{

"tmplcode": "0001AA1000000000TFIX",

"users": "0001AA10000000003YRF,0001AA10000000003YV6"

}

对象有两个属性：tmplcode和users

| 属性名称 | 描述 |
| --- | --- |
| tmplcode | 待分享模板的编码 |
| users | shared | 所有用户共享 |
|  | private | 租户自己私有 |
|  | "0001AA10000000003YRF,0001AA10000000003YV6" | 分享给某些租户，租户编码用逗号隔开 |