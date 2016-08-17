## 模板

### somalang/loadplugins {#somalang-loadplugins}

**基本信息：**

| 方法描述 | 加载插件多语文件 |
| --- | --- |
| 请求方法 | POST |
| API | somalang/loadplugins |
| 权限 | 系统管理员 | 是 |
|  | 租户管理员 | 是 |
|  | 系统用户 | 是 |
|  | 租户用户 | 是 |
| 多语 | 中文名称 | 加载插件多语文件 |
|  | 英文名称 | Load plugins lang |
| 是否记入事件 | 否 |

**Request URL:**

http://127.0.0.1:7681/soma/rest/somalang/loadplugins?_=1410921917577

**参数：**LangInfo 

"LangInfo langInfo"

| 参数名 | 类型 | 描述 |
| --- | --- | --- |
| langFileName | String | 多语目录名称 |
| langType | String | 多语类型CN("cn"), EN("en"); |
| moduleId | String | 模块id |
| menuId | String | 菜单id |

**返回值：**List&lt;LangInfo&gt;

**说明：

LangInfo:

{ String moduleId;

String menuId;

String langType;

String langFileName;

UTFProperties properties;
}
