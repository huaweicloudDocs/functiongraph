# FunctionGraph权限说明<a name="functiongraph_01_0140"></a>

## 帐户和子用户<a name="section227249155340"></a>

用户在注册华为云帐户后，进入"统一身份认证服务\>用户"界面，在帐户下创建用户，通过给用户组分配权限，设置用户所属用户组实现权限控制，如[图1](#fig11364911163819)所示。

**图 1**  权限控制<a name="fig11364911163819"></a>  
![](figures/权限控制.png "权限控制")

## 用户组权限说明<a name="section3360412155614"></a>

注册华为云帐户后，系统会自动生成admin用户组，进入"统一身份认证服务\>用户"界面，如[图2](#fig490852310713)所示。admin用户组具有所有区域所有服务的管理员权限，并且具有用户管理的权限，如[图3](#fig1119213115214)所示。

**图 2**  管理员<a name="fig490852310713"></a>  
![](figures/管理员.png "管理员")

**图 3**  admin用户组<a name="fig1119213115214"></a>  
![](figures/admin用户组.png "admin用户组")

除了admin用户组，登录账号进入"统一身份认证服务\>用户"界面，新建用户组，选择所属区域，修改权限集，如[图4](#fig17218162671016)所示。权限集说明如[表1](#table105311228172114)所示。

**图 4**  修改用户组权限<a name="fig17218162671016"></a>  
![](figures/修改用户组权限.png "修改用户组权限")

**表 1**  权限集说明

<a name="table105311228172114"></a>
<table><thead align="left"><tr id="row17532152812118"><th class="cellrowborder" valign="top" width="33.333333333333336%" id="mcps1.2.4.1.1"><p id="p175321328102113"><a name="p175321328102113"></a><a name="p175321328102113"></a>所属云服务</p>
</th>
<th class="cellrowborder" valign="top" width="33.333333333333336%" id="mcps1.2.4.1.2"><p id="p1353232812111"><a name="p1353232812111"></a><a name="p1353232812111"></a>权限集</p>
</th>
<th class="cellrowborder" valign="top" width="33.333333333333336%" id="mcps1.2.4.1.3"><p id="p1053332862110"><a name="p1053332862110"></a><a name="p1053332862110"></a>权限集描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row953322810211"><td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.1 "><p id="p16533122819217"><a name="p16533122819217"></a><a name="p16533122819217"></a>FGS</p>
</td>
<td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.2 "><p id="p353332812114"><a name="p353332812114"></a><a name="p353332812114"></a>FunctionGraph Administrator</p>
</td>
<td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.3 "><p id="p1159516587325"><a name="p1159516587325"></a><a name="p1159516587325"></a>可以控制函数、工作流和触发器的管理（增删改查）和触发。</p>
</td>
</tr>
<tr id="row45342028102113"><td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.1 "><p id="p1653492811212"><a name="p1653492811212"></a><a name="p1653492811212"></a>FGS</p>
</td>
<td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.2 "><p id="p17987651193015"><a name="p17987651193015"></a><a name="p17987651193015"></a>FunctionGraph Invoker</p>
</td>
<td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.3 "><p id="p105351328112110"><a name="p105351328112110"></a><a name="p105351328112110"></a>可以控制函数、工作流和触发器的查询，以及函数和工作流的触发。</p>
</td>
</tr>
<tr id="row153515284217"><td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.1 "><p id="p035911425222"><a name="p035911425222"></a><a name="p035911425222"></a>基本</p>
</td>
<td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.2 "><p id="p553632816210"><a name="p553632816210"></a><a name="p553632816210"></a>Tenant Administrator</p>
</td>
<td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.3 "><p id="p135361828122115"><a name="p135361828122115"></a><a name="p135361828122115"></a>具备该区域内所有服务的管理员权限。</p>
</td>
</tr>
<tr id="row15536102822114"><td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.1 "><p id="p165366281215"><a name="p165366281215"></a><a name="p165366281215"></a>基本</p>
</td>
<td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.2 "><p id="p1537202832117"><a name="p1537202832117"></a><a name="p1537202832117"></a>Server Administrator</p>
</td>
<td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.3 "><p id="p4537728102115"><a name="p4537728102115"></a><a name="p4537728102115"></a>具备该区域内所有Server服务（ECS、EVS、VPC）的管理员权限。</p>
</td>
</tr>
<tr id="row95371528102116"><td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.1 "><p id="p10537228162113"><a name="p10537228162113"></a><a name="p10537228162113"></a>基本</p>
</td>
<td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.2 "><p id="p8538202842120"><a name="p8538202842120"></a><a name="p8538202842120"></a>Tenant Guest</p>
</td>
<td class="cellrowborder" valign="top" width="33.333333333333336%" headers="mcps1.2.4.1.3 "><p id="p9538132802117"><a name="p9538132802117"></a><a name="p9538132802117"></a>具备该区域内所有服务的查看权限。</p>
</td>
</tr>
</tbody>
</table>

## 操作权限矩阵<a name="section24111253191131"></a>

**函数操作权限**

函数操作权限如[表2](#table2979182216211)所示。

**表 2**  函数操作权限

<a name="table2979182216211"></a>
<table><thead align="left"><tr id="row1798013220215"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.1"><p id="p179802229219"><a name="p179802229219"></a><a name="p179802229219"></a>操作</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.2"><p id="p398012220214"><a name="p398012220214"></a><a name="p398012220214"></a>本区域Tenant Administrator</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.3"><p id="p1698020225216"><a name="p1698020225216"></a><a name="p1698020225216"></a>本区域FunctionGraph Administrator</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.4"><p id="p7980522162115"><a name="p7980522162115"></a><a name="p7980522162115"></a>本区域FunctionGraph Invoker</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.6.1.5"><p id="p14980162211214"><a name="p14980162211214"></a><a name="p14980162211214"></a>本区域Tenant Guest</p>
</th>
</tr>
</thead>
<tbody><tr id="row89801522192116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p55341133132217"><a name="p55341133132217"></a><a name="p55341133132217"></a>创建函数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p89801225214"><a name="p89801225214"></a><a name="p89801225214"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p1298092210218"><a name="p1298092210218"></a><a name="p1298092210218"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p1998092211214"><a name="p1998092211214"></a><a name="p1998092211214"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p8980152202110"><a name="p8980152202110"></a><a name="p8980152202110"></a>×</p>
</td>
</tr>
<tr id="row1798018225216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p953463314220"><a name="p953463314220"></a><a name="p953463314220"></a>查询函数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p18980202220218"><a name="p18980202220218"></a><a name="p18980202220218"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p15980182216212"><a name="p15980182216212"></a><a name="p15980182216212"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p17980162292111"><a name="p17980162292111"></a><a name="p17980162292111"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p1198052212114"><a name="p1198052212114"></a><a name="p1198052212114"></a>√</p>
</td>
</tr>
<tr id="row13980132252113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p95341633122219"><a name="p95341633122219"></a><a name="p95341633122219"></a>修改函数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p198062211214"><a name="p198062211214"></a><a name="p198062211214"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p189801622182114"><a name="p189801622182114"></a><a name="p189801622182114"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p5980172212212"><a name="p5980172212212"></a><a name="p5980172212212"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p0980822162113"><a name="p0980822162113"></a><a name="p0980822162113"></a>×</p>
</td>
</tr>
<tr id="row398032262112"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p16534133311227"><a name="p16534133311227"></a><a name="p16534133311227"></a>删除函数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p1798112222120"><a name="p1798112222120"></a><a name="p1798112222120"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p298110229219"><a name="p298110229219"></a><a name="p298110229219"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p39812227216"><a name="p39812227216"></a><a name="p39812227216"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p12981122152118"><a name="p12981122152118"></a><a name="p12981122152118"></a>×</p>
</td>
</tr>
<tr id="row198110220215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p75354333225"><a name="p75354333225"></a><a name="p75354333225"></a>调用函数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p7981322172117"><a name="p7981322172117"></a><a name="p7981322172117"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p598112282113"><a name="p598112282113"></a><a name="p598112282113"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p17981172282120"><a name="p17981172282120"></a><a name="p17981172282120"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p89817223219"><a name="p89817223219"></a><a name="p89817223219"></a>×</p>
</td>
</tr>
<tr id="row11981122242119"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p1153515330224"><a name="p1153515330224"></a><a name="p1153515330224"></a>查看函数日志</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p898113228215"><a name="p898113228215"></a><a name="p898113228215"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p1298119222210"><a name="p1298119222210"></a><a name="p1298119222210"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p1298172218218"><a name="p1298172218218"></a><a name="p1298172218218"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p598182292116"><a name="p598182292116"></a><a name="p598182292116"></a>√</p>
</td>
</tr>
<tr id="row12981102212214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.1 "><p id="p14535933162213"><a name="p14535933162213"></a><a name="p14535933162213"></a>查看函数指标数据</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.2 "><p id="p179819223215"><a name="p179819223215"></a><a name="p179819223215"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.3 "><p id="p99818226217"><a name="p99818226217"></a><a name="p99818226217"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.4 "><p id="p2098172217218"><a name="p2098172217218"></a><a name="p2098172217218"></a>×</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.6.1.5 "><p id="p19981192214214"><a name="p19981192214214"></a><a name="p19981192214214"></a>√</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   “√”：子用户被赋予此权限可执行对应操作。  
>-   “×”：子用户被赋予此权限不可执行对应操作。  

**触发器使用权限**

-   DMS触发器
    1.  租户或拥有本区域Tenant Guest及以上权限的子用户。
    2.  创建委托（需要租户或者拥有“全局服务\>全局\>Security Administrator”权限的子用户），委托FunctionGraph访问DMS服务并配置到函数的委托配置中。

-   DIS触发器
    1.  租户或拥有本区域DIS Administrator及以上权限的子用户。
    2.  创建委托（需要租户或者拥有“全局服务\>全局\>Security Administrator”权限的子用户），委托FunctionGraph访问DIS服务并配置到函数的委托配置中。

-   OBS触发器

    租户或拥有“全局服务\>对象存储服务\>OBS Administrator”权限的子用户。

-   SMN触发器

    租户或拥有本区域SMN Administrator及以上权限的子用户。

-   APIG触发器

    租户或拥有本区域Tenant Administrator权限的子用户。

-   定时触发器

    租户或拥有本区域Tenant Administrator权限的子用户。


## 用户登录<a name="section120488316355"></a>

帐户登录界面如[图5](#fig1131013254515)所示。需要输入帐户名和密码。

**图 5**  帐户登录<a name="fig1131013254515"></a>  
![](figures/帐户登录.png "帐户登录")

子帐户登录界面如[图6](#fig99416427518)所示。需要输入帐户名、用户名和密码。

**图 6**  IAM用户登录<a name="fig99416427518"></a>  
![](figures/IAM用户登录.png "IAM用户登录")

