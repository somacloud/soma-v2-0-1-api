## node/installService {#node-installservice}

**基本信息：**

| 方法描述 | 选择可以安装服务的主机 |
| --- | --- |
| 请求方法 | POST |
| API | node/installService |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 用户 | 是 |
| 多语 | 中文名称 | 选择可以安装服务的主机 |
|  | 英文名称 |  |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/node/installService?_=1410924373474

**参数：**Json String {“name”:”XXX”,”outNodes”:[ xxx,xxx]}

**返回值：**List< ComputerVO>

**说明：**ComputerVO 见node/list