## swcatalog/list {#swcatalog-list}

**基本信息：**

| 方法描述 | 查询软件类型列表 |
| --- | --- |
| 请求方法 | GET |
| API | swcatalog/list |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询软件类型列表 |
|  | 英文名称 | List all software types |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/swcatalog/list?_=1410924373474

**参数：**无

**返回值：**Collection&lt;SoftwareVO&gt;

**说明：**SoftwareVO的数据结构：

{ String code;

String name;

String repoType;

Integer datatype;

String srcpath;

String collectioncode;

String swType;

String roleType;

String swVersion;

String pkgName;

String swPath;

String winDefaultPath;

String nonWinDefaultPath;

Map<String,String> env;

String es;

String machineCode;

String machineName;

String lastModifyTime;

String length;

Boolean auto;

String install_args;

String swModules;

String taskID;

String softwareRepoCode;

RepoConfigVO belongRepo;

RepoConfigVO[] repos;

SoftwareInBasicVO basic;

List&lt;ConfigOptionVO&gt; configOptions;

CatelogAccVO authVO;

SystemTypesVO[] systemTypes;

}

RepoConfigVO的数据结构:

{ String code;

String name;

String type;

String url;

Boolean isready;

String description;

String protocol = null;

String host = null;

Int port = -1;

String path = null;

String username = null;

String password = null;

Boolean defaultRepo;

Boolean isenable;

String accountCode = null;

String system;

}

SoftwareInBasicVO的数据结构:

{ String type;

String node;

String machineCode;

String machineName;

}

ConfigOptionVO的数据结构:

{ String category;

String name;

String key;

String initValue;

String value;

String layout;

String defaultValue;

String optype;

}

CatelogAccVO的数据结构:

{ String code;

String typeCode;

String typeName;

String creatorCode;

String creatorName;

String creatorAccountCode;

String creatorAccountName;

Int accType;

String cateLogType;

}

SystemTypesVO的数据结构:

{ String systemType;

String pachageName;

}

SoftwareVO的数据实例：

| [{ |
| --- |