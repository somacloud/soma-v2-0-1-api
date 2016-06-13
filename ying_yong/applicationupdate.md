## application/update {#application-update}

**基本信息：**

| 方法描述 | 更新应用信息 |
| --- | --- |
| 请求方法 | POST |
| API | application/update |
| 权限 | 系统管理员 | 是，编辑所有非注册应用 |
|  | 租户管理员 | 是，编辑租户下的所有非注册应用 |
|  | 系统用户 | 是，编辑所有非注册应用 |
|  | 租户用户 | 是，编辑用户自己创建的所有非注册应用 |
| 多语 | 中文名称 | 更新应用信息 |
|  | 英文名称 | **Update application** |
| 是否记入事件 | 是 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/update?_=1410924373474

**参数：**Application app

**返回值：**

**说明：**

Application的数据结构:

{ AppInstanceBasicVO basic;

Software software;

List&lt;Service&gt; services;

List&lt;ServiceGroup&gt; serviceGroups;

List&lt;TypePluginVO&gt; plugins;

}

AppInstanceBasicVO basic的数据结构:

{ String node;

String httpPort;

}

Software的数据结构:

{ SoftwareInBasicVO basic;

SystemTypeVO[] systemTypes;

}

Service的数据结构:

{ ServiceInBasicVO basic;

Software software;

List&lt;TypePluginVO&gt; plugins;

}

ServiceGroup的数据结构:

{ String name;

List&lt;String&gt; urls;

List&lt;String&gt; servers;

}

TypePluginVO的数据结构:

{ PluginBasicVO basic;

List&lt;ConfigOptionVO&gt; configOptions;

String data;

}

Application的数据实例:

| { |
| --- |