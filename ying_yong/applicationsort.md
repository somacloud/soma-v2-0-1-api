## application/sort {#application-sort}

**基本信息：**

| 方法描述 | 查询应用评分较低的几个实例 |
| --- | --- |
| 请求方法 | POST |
| API | application/sort |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 查询应用评分较低的几个实例 |
|  | 英文名称 | **Query application srcore desc for top n** |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/application/sort?_=1410924373474

**参数：**String topn(数字)

**返回值：**List< ResourceHealthVO> rhvo

| ResourceHealthVO对象 |
| --- |