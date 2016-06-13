## node/list {#node-list}

**基本信息：**

| 方法描述 | 查询所有主机信息 |
| --- | --- |
| 请求方法 | GET |
| API | node/list |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询所有主机信息 |
|  | 英文名称 | Query all hosts |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/node/list?_=1410924373474

**参数：**无

**返回值：**ComputerVO[]

**说明：**ComputerVO的数据结构

{ String code;

String name;

String username;

String password;

String systemType;

String osType;

String osName;

String vmSystemType;

String vm_type;

String hostComputerCode;

String agentIP;

String privateIP;

Integer agentPort;

String agentCode;

String agentPath;

Boolean agentAlive;

String agentInsatllStatus;

String agentVersion;

String agentNewVersion;

Boolean isLan;

String oldPassword;

HealthReport report;

AgentMonitorStatistic statistic;

String selinux;

String firewall;

String sshd;

String ulimitOpenfile;

String ulimitMaxPro;

List&lt;SoftwareVO&gt; softwares;

String hostname;

String domainName;

String rack;

String dcCode;

String dcName;

String vncHost;

String vncPort;

String vncPassword;

Integer maxVncPort = 5905;

String memModel;

String memSize;

String memSpeed;

String cpuModel;

String spuFrq;

Integer cpuCount;

Integer cpuKernel;

Long diskSize;

List&lt;PartitionVO&gt; partitions;

List&lt;VMDiskVO&gt; vmdisks;

List&lt;MachineDatastorageVO&gt; datastorage;

String datastoragecode;

List&lt;SwapVO&gt; swaps;

List&lt;NicVO&gt; nics;

Long memUsed;

Integer memFree;

Double cpuRatio;

Integer readIO;

Integer writeIO;

String vmStatus;

String allocationTs;

Long allocationTotalTime=0l;

UFDateTime created;

String organizeCode;

String organizeName;

String adminAccountCode;

String adminAccountName;

String userAccountCode;

String userAccountName;

}

HealthReport的数据结构:

{ int score;

String level;

String description;

String advise;

List&lt;HealthData&gt; detail;

}

HealthData的数据结构：

{ String prop;

String displayProp;

Double avgVal;

List&lt;String&gt; datas;

List&lt;Integer&gt; scores;

List&lt;String&gt; times;

Int rusultScore;

}

AgentMonitorStatistic的数据结构:

{ String code;

String name;

String agentIP;

String startTs;

HealthReport report;

Int score;

String status;

String osType;

String agentPath;

AgentMonitorVO monitorVO;

Boolean monitorFlag;

Long interval;

List&lt;MonitorRule&gt; rules;

String AlarmResponse alarm;

}

SoftwareVO的数据结构:见swcatalog/list

PartitionVO的数据结构:

{ String name;

Integer partitionSize;

Integer uesdSize;

Integer usableSize;

Double usedRatio;

String reference;

String code;

String machineCode;

}

VMDiskVO的数据结构:

{ String code;

String machinename;

String datastoragecode;

String datastoragename;

String machinecode;

String disk_path;

String disk_size;

String disk_type;

}

MachineDatastorageVO的数据结构:

{ String code;

String name;

String datastoragecode;

String machinecode;

String dir;

String size_all;

String size_used;

String ds_type;

}

SwapVO的数据结构:

{ String name;

Integer swapSize;

Integer usedSize;

String code;

String machineCode;

String type;

Integer priority;

}

NicVO的数据结构:

{ String code;

String ip;

String mac;

String machineCode;

String model;

String name;

}

ComputerVO的数据实例：

| { |
| --- |