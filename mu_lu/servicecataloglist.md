## servicecatalog/list {#servicecatalog-list}

**基本信息：**

| 方法描述 | 查询所有服务类型 |
| --- | --- |
| 请求方法 | GET |
| API | servicecatalog/list |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询所有服务类型 |
|  | 英文名称 | Listall service types |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/servicecatalog/list?_=1410924373474

**参数：**无

**返回值：**Collection&lt;ServiceTypeVO&gt;

**说明：**ServiceTypeVO的数据结构：

{ ServiceTypeBasicVO basic;

SoftwareTypeVO software;

List&lt;TypePluginVO&gt; plugins;

CatelogAccVO authVO;

}

ServiceTypeBasicVO的数据结构:

{ String basePath = “”;

String detailBasePath = “”;

Boolean placeholder;

String serviceName;

String userName;

List&lt;String&gt; acceptLbServices;

}

SoftwareTypeVO的数据结构:

{ SoftwareTypeBasicVO basic;

SystemTypesVO[] systemTypes;

CatelogAccVO authVO;

}

SoftwareTypeBasicVO的数据结构:

{ String repoType;

String code;

String name;

Boolean placeholder;

String swType;

String roleType;

String swVersion;

List&lt;String&gt; hisVersion;

String srcpath;

String defaultPath;

String swPath;

String system;

String description;

String icon;

String tag;

}

SystemTypesVO的数据结构:

{ String systemType;

String packageName;

}

TypePluginVO的数据结构:

{ PluginBasicVO basic;

List&lt;ConfigOptionVO&gt; configOptions;

String data;

}

CatelogAccVO的数据结构:见swcatalog/list

ServiceTypeVO的数据实例：

| [{ |
| --- |