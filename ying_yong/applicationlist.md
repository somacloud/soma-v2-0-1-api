## application/list {#application-list}

**基本信息：**

| 方法描述 | 查询所有应用 |
| --- | --- |
| 请求方法 | GET |
| API | application/list |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询所有应用 |
|  | 英文名称 | **Query all application** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/list?_=1410924373474

**参数：**

**返回值：**Collection&lt;VirtualSystemVO&gt;

**说明：**

VirtualSystemVO的数据结构:

{ String code;

String name;

String systemStatus;

AppMonitorSystemStatistic statistic;

List&lt;AVMachineVO&gt; avms;

List&lt;ApplicationVO&gt; apps;

String masterCode;

String type;

String basicTypeIcon;

String appHome;

ApplicationTypeVO appType;

Application appInst;

List<VSAllocationVO allocations;

String console;

Boolean regist;

String allocationTs;

Long allocationTotalTime;

String appTemplateCode;

HealthReport healthReport;

UFDateTime createTime;

UFDateTime startTime;

}

AppMonitorSystemStatistic的数据结构:

{ String systemCode;

String systemName;

Int score;

String status;

Int onlineuser;

String runtime=”0”;

Collection&lt;AooMonitorServiceStatistic&gt; results;

HealthReport report;

DiagnoseReport diagnose;

Int loadPeak;

AlarmResponse alarm;

}

AVMachineVO的数据结构:

{ String code;

String name;

String machineCode;

String machineName;

String softwareCode;

String vsCode;

String vsName;

String avmStatus;

String roleType;

String softwareName;

String profileCode;

String serviceType;

String swType;

String env;

String swHome;

String javaHome;

String profileHome;

String wasHome;

List&lt;ConnectorVO&gt; connectors;

Integer webMaxConn;

Integer webInitCoon;

Integer webPort;

Integer servicePort;

String jvmArgs;

Int weiht = 2;

Integer maxThread;

Integer initThread;

Integer maxWMThread;

Integer maxScheduleThread;

String dbType;

String dbVersion;

String dbUrl;

String dbConnHost;

String dbConnPort;

String dbConnSID;

Boolean userExits;

Bollean instanceExits;

Boolean scaleDown;

String dbUser;

String dbPassword;

Integer dbMaxConn;

Integer dbInitConn;

String domain;

String adminuser;

String adminpwd;

String keystoreFile;

String keystorePass;

Boolean httpsEnabled;

UFDateTime operationTime;

String appTemplateCode;

String appSoftwareCode;

HealthReport healthReport;

UFDateTime createTime;

UFDateTime startTime;

}

ApplicationVO的数据结构:

{ String coed;

String name;

String version;

String softwareCode;

String ncHome;

String earPath;

String appStatus;

String vsCode;

String vsName;

String softwareType;

String[] deployModules;

String machineCode;

String machineName;

String agentIP;

}

ApplicationTypeVO的数据结构:见appcatalog/list

Application的数据结构:见application/update

VSAllocationVO的数据结构:

{ String code;

String vsCode;

String userAccCode;

String createrCode;

AccountVO userAccvo;

String userCode;

AdminVO user;

AdminVO creater;

}

HealthReport的数据结构:见node/list

VirtualSystemVO的数据实例：

| [{ |
| --- |