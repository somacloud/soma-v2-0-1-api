## appcatalog/list {#appcatalog-list}

| 方法描述 | 查询所有应用类型 |
| --- | --- |
| 请求方法 | GET |
| API | appcatalog/list |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询所有应用类型 |
|  | 英文名称 | List all application types |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/appcatalog/list?_=1410924373474

**参数：**无

**返回值：**Collection&lt;ApplicationTypeVO&gt;

**说明：**ApplicationTypeVO的数据结构:

{ AppTypeBasicVO basic;

SoftwareTypeVO software;

List&lt;TypePluginVO&gt; plugins;

CatelogAccVO authVO;

List&lt;ServiceTypeVO&gt; services;

}

AppTypeBasicVO的数据结构:

{ String basePath;

String detailBasePath = “”;

List&lt;String&gt; acceptServiceTypes;

List&lt;String&gt; acceptSoftwareTypes;

String userName;

Boolean placeholder;

String appSource;

}

SoftwareTypeVO的数据结构:见swcatalog/list

TypePluginVO的数据结构:见swcatalog/list

CatelogAccVO的数据结构:见swcatalog/list

ApplicationTypeVO的数据实例:

| { |
| --- |