# 目录

版权 2

目录 3

1数据中心 8

1.1 datacenter/list 8

1.2 datacenter/listbypage 9

1.3 datacenter/get/{id} 10

1.4 datacenter/update 10

1.5 datacenter/add 11

1.6 datacenter/delete/{id} 11

1.7 datacenter/updaterepo/ 12

1.8 datacenter/updatetag 13

1.9 datacenter/updateip 14

1.10 datacenter/getip/{code} 15

1.11 datacenter/listvirdc 15

1.12 datacenter/querypdccount 16

1.13 datacenter/listallSimple 17

1.14 datacenter/listMultiDCSimple 17

1.15 datacenter /checkname 18

1.16 datacenter /upload 19

2主机 19

2.1 node/list 19

2.2 node/get/{id} 28

2.3 node/getsimple/{id} 29

2.4 node/update 30

2.5 node/regist 30

2.6 node/delete/{id} 31

2.7 node/installagent/{id} 31

2.8 node/startagent/{id} 32

2.9 node/stopagent/{id} 33

2.10 node/getAgentVersion 33

2.11 node/validateNode 34

2.12 node/validateResource 34

2.13 node/validateResources 35

2.14 node/listwithhealth 36

2.15 node/listbypage 36

2.16 node/refresh 38

2.17 node/checkname 38

2.18 node/queryCount 39

2.19 node/queryNodeDetail 39

2.20 node/allocateService 40

2.21 node/queryNode2InstallSw（暂时废弃） 41

2.22 node/installService 41

2.23 node/listMigrateNodes 42

2.24 node/hostsmgr 42

2.25 node/callbackHost 43

2.26 node/callbackHosts 44

2.27 node/allocateHosts 44

2.28 node/addvm/{dcType} 45

2.29 node/addvmbypolicy/{dcType} 47

2.30 node/connectTest/{nodeid} 48

2.31 node/listCodes 48

2.32 node/updatetag 49

2.33 node/queryuservmcount 49

3目录 50

3.1 swcatalog/list 50

3.2 swcatalog/get/{id} 54

3.3 swcatalog/delete 55

3.4 swcatalog/shared 56

3.5 servicecatalog/list 56

3.6 servicecatalog/get/{name} 61

3.7 servicecatalog/getRoleTypes 61

3.8 servicecatalog/shared 62

3.9 appcatalog/list 62

3.10 appcatalog/get/{name} 65

3.11 appcatalog/shared 66

3.12 catalog/download/{type}/{fileName} 66

3.13 catalog/ queryIcon/{catagory}/{typeName} 67

4软件 68

4.1 software/get/{id} 68

4.2 software /install/{id}/{machineCode} 68

5服务 69

5.1 service/list 69

5.2 service/listbypage 73

5.3 service/get/{code} 74

5.4 service/queryService/{code} 76

5.5 service/add 76

5.6 service/addAndInstall 77

5.7 service/editSave 78

5.8 service/editAndInstall 78

5.9 service/delete 79

5.10 service/syncConfig 79

5.11 service/ register 80

5.12 service/ deregister 80

5.13 service/materialize/{code} 81

5.14 service/bind 82

5.15 service/unbind/{code} 82

5.16 service/start/{code} 83

5.17 service/stop/{code} 84

5.18 service/env 84

5.19 service/checkConfigs 85

5.20 service/updateConfig 86

5.21 service/updateTag 86

5.22 service/autoAllocate 87

6应用 88

6.1 application/checkname 88

6.2 application/ getplugin/{appType} 88

6.3 application/list 89

6.4 application/get/{id} 98

6.5 application/getapp/{id} 98

6.6 application/listbypage 99

6.7 application/listServers 99

6.8 application/listTopology 100

6.9 application/listbycondition 101

6.10 application/add 101

6.11 application/addAndMaterialize 102

6.12 application/update 103

6.13 application/tupdate 110

6.14 application/updateAndMaterialize 111

6.15 application/delete/{id} 111

6.16 application/queryRegisterApp 112

6.17 application/register 112

6.18 application/deregister 113

6.19 application/materialize/{id} 114

6.20 application/start/{id} 114

6.21 application/stop/{id} 115

6.22 application/syncFiles 115

6.23 application/refresh 116

6.24 application/getAppReport 117

6.25 appIication/allocAppToTenant 117

6.26 application/callBackApp 118

6.27 application /queryAppEnv 118

6.28 application/updatePlugin 119

6.29 application/serviceSelectApp 119

6.30 application/serviceUnbindApp 120

6.31 application/getstypes/{appcode}/{srtype} 121

6.32 application/appstatistics 121

6.33 application/checkAppLimit 122

6.34 application/checkConfigs 122

6.35 application/updateConfigs 123

6.36 application/sort 124

6.37 application/refreshInst 125

6.38 application/updatetag 125

6.39 application/checkDomainName 126

6.40 application/getStatus/{appCode} 126

6.41 application/migrate 127

6.42 upload/jee 128

7补丁 128

7.1 patch/listbypage 128

7.2 patchhistory/listbypage 129

8模板 130

8.1 应用模板 130

8.1.1appflavor/list 130

8.1.2appflavor/listwithtype/{type} 133

8.1.3appflavor/get/{name} 134

8.1.4appflavor/update 135

8.1.5appflavor/add 135

8.1.6appflavor/delete/{name} 136

8.1.7appflavor/shared 136

8.2 服务模板 137

8.2.1serflavor/list 137

8.2.1serflavor/listbypage 148

8.2.2serflavor/add 149

8.2.3serflavor/update 149

8.2.4serflavor/delete 150

8.2.5serflavor/querybycode 150

8.2.6serflavor/shared 151

8.3 虚机模板 152

8.3.1vmpolicy/get/{id} 152

8.3.2vmpolicy/list 155

8.3.3vmpolicy/listbydctype/{type} 155

8.3.4vmpolicy/listbydccode/{code} 156

8.3.5vmpolicy/search 157

8.3.6vmpolicy/search/{json} 157

8.3.7vmpolicy/update 158

8.3.8vmpolicy/add 158

8.3.9vmpolicy/delete/{id} 159

8.3.10vmpolicy/shared 159

9监控 161

9.1 应用 161

9.1.1monitorApplication/list 161

9.1.2monitorApplication/get/{id} 161

9.1.3monitorApplication/startReal/{id} 162

9.1.4monitorApplication/stopReal/{id} 162

9.2 服务 163

9.2.1monitorService/list 163

9.2.2monitorEnv/query 164

9.3 主机 164

9.3.1monitorNode/list 164

9.4 警报 165

9.4.1alarm/list 165

9.5 任务 165

9.5.1task/listbypage 165

9.6 事件 166

9.6.1event/list 166

9.6.2event/listbypage 167

10系统管理 168

10.1 account/lock/{code} 168

10.2 account/unlock/{code} 170

10.3 account/removeVirDC/{code} 170

10.4 account/modifyVirDC 171

10.5 account/listAccVirDC 172

10.6 account/add 172

10.7 account/update 173

10.8 renter/list 174

10.9 renteruser/list 175

10.10 user/lock/{code} 175

10.11 user/ unlock/{code} 176

10.12 user/setAdmin/{code} 176

10.13 user/ setUser/{code} 177

10.14 user/changepw 178

10.15 user/add 178

10.16 user/update 179

10.17 somaconfig/list 179

10.18 somaconfig/get/{key} 180

10.19 somaconfig/set/{key}/{value} 180

11其他 181

11.1 udn/login 181