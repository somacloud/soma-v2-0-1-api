## 服务模板

### serflavor/list {#serflavor-list}

**基本信息：**

| 方法描述 | 查询所有服务模板 |
| --- | --- |
| 请求方法 | GET |
| API | serflavor/list |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询所有服务模板 |
|  | 英文名称 | **Query all service template** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/serflavor/listFlavor?_=1410924373474

**参数：**

**返回值：**Collection&lt;ServiceFlavorVO&gt;

**说明：**ServiceFlavorVO的数据结构:

{ ServiceTypeBasicVO basic;

SoftwareTypeVO software;

List&lt;TypePluginVO&gt; plugins;

TemplateAuthVO authVO;

}

ServiceTypeBasicVO的数据结构:

{ String basePath;

String detailBasePath;

Boolean placeholder;

String serviceName;

String username;

List&lt;String&gt; acceptLbServices;

}

SoftwareTypeVO的数据结构:见swcatalog/list

TypePluginVO的数据结构:见swcatalog/list

TemplateAuthVO的数据结构:见appflavor/list

ServiceFlavorVO的数据实例:

| { |
| --- |

### serflavor/listbypage {#serflavor-listbypage}

**基本信息：**

| 方法描述 | 根据关键字查询服务模板 |
| --- | --- |
| 请求方法 | GET |
| API | serflavor/listbypage |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据关键字查询服务模板 |
|  | 英文名称 | **Query service templates by condition** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/serflavor/listbypage?_=1410924373474

**参数：**String json

{pageSize:18, pageIndex:1, queryCount:true, params:{keyword:ab, pagi:true}}

“keyword”的值是输入值

**返回值：**Collection&lt;ServiceFlavorVO&gt;

**说明：**ServiceFlavorVO见serflavor/listFlavor

### serflavor/add {#serflavor-add}

**基本信息：**

| 方法描述 | 新增服务模板 |
| --- | --- |
| 请求方法 | POST |
| API | serflavor/add |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 新增服务模板 |
|  | 英文名称 | **Create service templates** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/serflavor/add?_=1410924373474

**参数：**ServiceFlavorVO svo

**返回值：**ServiceFlavorVO svo

**说明：**ServiceFlavorVO见serflavor/listFlavor

### serflavor/update {#serflavor-update}

**基本信息：**

| 方法描述 | 更新服务模板 |
| --- | --- |
| 请求方法 | POST |
| API | serflavor/update |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 更新服务模板 |
|  | 英文名称 | **Update service templates** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/serflavor/update?_=1410924373474

**参数：**String json

返回值：**ServiceFlavorVO**

**说明：**ServiceFlavorVO见serflavor/listFlavor

Json的格式为{“oldName”: oldName,” newObj”: newObj}

其中，newObj由ServiceFlavorVO转化而成

### serflavor/delete {#serflavor-delete}

**基本信息：**

| 方法描述 | 删除服务模板 |
| --- | --- |
| 请求方法 | POST |
| API | serflavor/delete |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 删除服务模板 |
|  | 英文名称 | **Delete service templates** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/serflavor/delete?_=1410924373474

**参数：**String json

返回值：

**说明：**ServiceFlavorVO见serflavor/listFlavor

Json由ServiceFlavorVO转化而成

### serflavor/querybycode {#serflavor-querybycode}

**基本信息：**

| 方法描述 | 根据模板编码查询模板 |
| --- | --- |
| 请求方法 | POST |
| API | serflavor/querybycode |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 根据模板编码查询模板 |
|  | 英文名称 | **Query service template by code** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/serflavor/querybycode?_=1410924373474

**参数：**String code

返回值：ServiceFlavorVO svo

**说明：**ServiceFlavorVO见serflavor/listFlavor

### serflavor/shared {#serflavor-shared}

**基本信息：**

| 方法描述 | 分享服务模板 |
| --- | --- |
| 请求方法 | POST |
| API | serflavor/shared |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是，只能分享自己新建的模板 |
|  | 系统用户 | 是 |
|  | 租户用户 | 否 |
| 多语 | 中文名称 | 分享服务模板 |
|  | 英文名称 | **Share service template** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/serflavor/shared?_=1410924373474

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