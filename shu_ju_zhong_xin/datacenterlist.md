## datacenter/list {#datacenter-list}

**基本信息：**

**Request URL:**

| 方法描述 | 查询所有数据中心 |
| --- | --- |
| 请求方法 | GET |
| API | datacenter/list |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询数据中心 |
|  | 英文名称 | List data center |
| 是否记入事件 | 否 |

http://127.0.0.1:7681/soma/rest/datacenter /list?_=1410924373474

**参数：**无

**返回值：**DataCenterVO[]

**说明：**

DataCenterVO的数据结构

{ String code;

String name;

String netword;

Int dcType;

String description;

String imageLocation;

String cloudUserName;

String cloudPassword;

String cloudDomain;

String address;

String apiKey;

String secretKey;

String zoneId;

String memTotal;

String memUsed;

String cpuTotal;

String cpuUsed;

Int nodeTotal;

Int nodeAgentAlive;

String template;

String ts;

Integer dr;

List&lt;ComputerVO&gt; computers;

ComputerVO的数据结构：见node/list

DataCenterVO的数据实例：

| [{ |
| --- |