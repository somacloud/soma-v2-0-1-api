## service/list {#service-list}

**基本信息：**

| 方法描述 | 查询用户所有服务 |
| --- | --- |
| 请求方法 | GET |
| API | service/list |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询用户所有服务 |
|  | 英文名称 | List all services |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/service/list?_=1410924373474

**参数：**

**返回值：**AVMachineVO[]

**说明：**AVMachineVO的数据结构:

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

AVMachineVO的数据实例:

| [{ |
| --- |