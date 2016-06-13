## 应用模板

### appflavor/list {#appflavor-list}

**基本信息：**

| 方法描述 | 查询所有应用模板 |
| --- | --- |
| 请求方法 | GET |
| API | appflavor/list |
| 权限 | 系统管理员 | 是，查看所有模板 |
|  | 租户管理员 | 是，查看系统预置的，自己新增的，和别的租户分享给自己的 |
|  | 系统用户 | 是，查看所有模板 |
|  | 租户用户 | 是，查看系统预置的，自己新增的，和别的租户分享给自己的 |
| 多语 | 中文名称 | 查询所有应用模板 |
|  | 英文名称 | **Query all application template** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/appflavor/list?_=1410924373474

**参数：**

**返回值：**ApplicationTemplateVO[]

**说明：**ApplicationTemplateVO的数据结构:

{ AppTypeBasicVO basic;

SoftwareTypeVO software;

List&lt;TypePluginVO&gt; plugins;

TemplateAuthVO authVO;

List&lt;Service&gt; services;

}

AppTypeBasicVO的数据结构:

{ String basePath;

String detailBasePath;

List&lt;String&gt; acceptServiceTypes;

List&lt;String&gt; acceptSoftwareTypes;

String username;

Boolean placeholder;

String appSource;

}

SoftwareTypeVO的数据结构:见swcatalog/list

TypePluginVO的数据结构:见swcatalog/list

TemplateAuthVO的数据结构:

{ String code;

String templateCode;

String templateName;

String creatorCode;

String creatorName;

String creatorAccountCode;

String creatorAccountName;

Int authType;

String templateCate;

String userAccountCodes;

}

Service的数据结构:见service/get/{code}

ApplicationTemplateVO的数据实例:

| [{ |
| --- |

### appflavor/listwithtype/{type} {#appflavor-listwithtype-type}

**基本信息：**

| 方法描述 | 根据应用类型查询所有应用模板 |
| --- | --- |
| 请求方法 | GET |
| API | appflavor/listwithtype/{type} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据应用类型查询所有应用模板 |
|  | 英文名称 | **Query application templates by type** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/appflavor/listwithtype/{type}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | type | ApplicationTemplateVO.basic.type | true | path variable |

**返回值：**ApplicationTemplateVO[]

**说明：**ApplicationTemplateVO见appflavor/list

### appflavor/get/{name} {#appflavor-get-name}

**基本信息：**

| 方法描述 | 根据应用模板名称查询应用模板 |
| --- | --- |
| 请求方法 | GET |
| API | appflavor/get/{name} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据应用模板名称查询应用模板 |
|  | 英文名称 | **Query application template by name** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/appflavor/get/{name}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | name | ApplicationTemplateVO.basic.name | true | path variable |

**返回值：**ApplicationTemplateVO

**说明：**ApplicationTemplateVO见appflavor/list

### appflavor/update {#appflavor-update}

**基本信息：**

| 方法描述 | 更新应用模板信息 |
| --- | --- |
| 请求方法 | POST |
| API | appflavor/update |
| 权限 | 系统管理员 | 是，编辑所有非系统预置模板 |
|  | 租户管理员 | 是，编辑自己新增的模板 |
|  | 系统用户 | 是，编辑所有非系统预置模板 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 更新应用模板信息 |
|  | 英文名称 | **Update application template** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/appflavor/update?_=1410924373474

**参数：**ApplicationTemplateVO vo

**返回值：**

**说明：**ApplicationTemplateVO见appflavor/list

### appflavor/add {#appflavor-add}

**基本信息：**

| 方法描述 | 新增应用模板 |
| --- | --- |
| 请求方法 | POST |
| API | appflavor/add |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 新增应用模板 |
|  | 英文名称 | **Create application template** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/appflavor/add?_=1410924373474

**参数：**ApplicationTemplateVO vo

**返回值：**

**说明：**ApplicationTemplateVO见appflavor/list

### appflavor/delete/{name} {#appflavor-delete-name}

**基本信息：**

| 方法描述 | 根据名称删除应用模板 |
| --- | --- |
| 请求方法 | GET |
| API | appflavor/delete/{name} |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是，只能删除自己新建的模板 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 根据名称删除应用模板 |
|  | 英文名称 | **Delete application template by name** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/appflavor/delete/{name}?_=1410924373474

**参数：**

| **类型** | **参数名称** | **描述** | **Mandatory** | **Parameter type** |
| --- | --- | --- | --- | --- |
| String | name | ApplicationTemplateVO.basic.name | true | path variable |

**返回值：**

**说明：**ApplicationTemplateVO见appflavor/list

### appflavor/shared {#appflavor-shared}

**基本信息：**

| 方法描述 | 分享应用模板 |
| --- | --- |
| 请求方法 | POST |
| API | appflavor/shared |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是，只能分享自己新建的模板 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 分享应用模板 |
|  | 英文名称 | **Share application template** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/appflavor/shared?_=1410924373474

**参数：**String json

例："{\"tmplcode\":\"0001AA1000000000TFIX\",\"users\":\"0001AA10000000003YRF"}"

**返回值：**无

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