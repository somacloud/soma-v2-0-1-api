## somaconfig/list {#somaconfig-list}

**基本信息：**

| 方法描述 | 查询全局变量 |
| --- | --- |
| 请求方法 | GET |
| API | somaconfig/list |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询全局变量 |
|  | 英文名称 | **Query variables** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/somaconfig/list?_=1410924373474

**参数：**

**返回值：**Map<String, String> map

**说明：**

map的结构为{ NODE_ALLOCATE_POLICY: preempt, APPLICATION_ALLOCATE_POLICY: nodeaffinity}其中，NODE_ALLOCATE_POLICY代表应用自动伸缩策略，取值有两种，preempt和virtualfirst，代表水平优先和垂直优先。APPLICATION_ALLOCATE_POLICY代表应用分配节点策略，取值有两种，nodeaffinity和widedistribution，代表节点亲和策略和水平分配策略。