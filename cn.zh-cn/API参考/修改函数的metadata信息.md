# 修改函数的metadata信息<a name="functiongraph_06_0111"></a>

## 功能介绍<a name="section14487165524413"></a>

修改指定的函数的metadata信息。

## URI<a name="section19488125564417"></a>

URL：/v2/\{project\_id\}/fgs/functions/\{function\_urn\}/config

Method：PUT

参数说明如[表1](#table14489155144411)所示。

**表 1**  参数说明

<a name="table14489155144411"></a>
<table><thead align="left"><tr id="row7740355154412"><th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.1"><p id="p97401559442"><a name="p97401559442"></a><a name="p97401559442"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885711%" id="mcps1.2.5.1.2"><p id="p18740855114411"><a name="p18740855114411"></a><a name="p18740855114411"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.5.1.3"><p id="p11740105515447"><a name="p11740105515447"></a><a name="p11740105515447"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="52.03479652034796%" id="mcps1.2.5.1.4"><p id="p2740125518442"><a name="p2740125518442"></a><a name="p2740125518442"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row5740175574412"><td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.1 "><p id="p17409554448"><a name="p17409554448"></a><a name="p17409554448"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.5.1.2 "><p id="p127401355154420"><a name="p127401355154420"></a><a name="p127401355154420"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p11740145513446"><a name="p11740145513446"></a><a name="p11740145513446"></a>必选</p>
</td>
<td class="cellrowborder" valign="top" width="52.03479652034796%" headers="mcps1.2.5.1.4 "><p id="p15740175515447"><a name="p15740175515447"></a><a name="p15740175515447"></a>Project Id。</p>
</td>
</tr>
<tr id="row12740195519440"><td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.1 "><p id="p37401855134414"><a name="p37401855134414"></a><a name="p37401855134414"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.5.1.2 "><p id="p37402055184410"><a name="p37402055184410"></a><a name="p37402055184410"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.5.1.3 "><p id="p774075564418"><a name="p774075564418"></a><a name="p774075564418"></a>必选</p>
</td>
<td class="cellrowborder" valign="top" width="52.03479652034796%" headers="mcps1.2.5.1.4 "><p id="p187401555194410"><a name="p187401555194410"></a><a name="p187401555194410"></a>函数的URN，详细解释见<a href="FunctionGraph函数模型.md">FunctionGraph函数模型</a>。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section6503155554416"></a>

**请求参数**

参数说明如[表2](#table5506155144418)所示。

**表 2**  参数说明表

<a name="table5506155144418"></a>
<table><thead align="left"><tr id="row127401255104416"><th class="cellrowborder" valign="top" width="17.171717171717173%" id="mcps1.2.5.1.1"><p id="p1974075594416"><a name="p1974075594416"></a><a name="p1974075594416"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16.161616161616163%" id="mcps1.2.5.1.2"><p id="p174014556446"><a name="p174014556446"></a><a name="p174014556446"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="12.121212121212121%" id="mcps1.2.5.1.3"><p id="p8740455154417"><a name="p8740455154417"></a><a name="p8740455154417"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="54.545454545454554%" id="mcps1.2.5.1.4"><p id="p1274075519446"><a name="p1274075519446"></a><a name="p1274075519446"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row774115514417"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p07412555445"><a name="p07412555445"></a><a name="p07412555445"></a>Runtime</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p27411855154416"><a name="p27411855154416"></a><a name="p27411855154416"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p13741175512449"><a name="p13741175512449"></a><a name="p13741175512449"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p1494811074514"><a name="p1494811074514"></a><a name="p1494811074514"></a>FunctionGraph函数的执行环境，取值：Node.js6.10、Node.js8.10、Python2.7、Python3.6、Java8、Go1.8、C#.NET Core 2.0、C#.NET Core 2.1。</p>
</td>
</tr>
<tr id="row133668354389"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p833044815384"><a name="p833044815384"></a><a name="p833044815384"></a>code_type</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p1633024863810"><a name="p1633024863810"></a><a name="p1633024863810"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p2033016486385"><a name="p2033016486385"></a><a name="p2033016486385"></a>必选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p83301348143814"><a name="p83301348143814"></a><a name="p83301348143814"></a>函数代码类型，请参考<a href="FunctionGraph函数模型.md#table357132064218">表1</a>。</p>
</td>
</tr>
<tr id="row344573219388"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p103301848103818"><a name="p103301848103818"></a><a name="p103301848103818"></a>code_url</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p12330114818381"><a name="p12330114818381"></a><a name="p12330114818381"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p4330148103818"><a name="p4330148103818"></a><a name="p4330148103818"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p11330648103815"><a name="p11330648103815"></a><a name="p11330648103815"></a>函数代码包在OBS上的地址，当CodeType为obs时必选。</p>
</td>
</tr>
<tr id="row1574111556448"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p1574135517441"><a name="p1574135517441"></a><a name="p1574135517441"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p5741655184415"><a name="p5741655184415"></a><a name="p5741655184415"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p167412555449"><a name="p167412555449"></a><a name="p167412555449"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p16741205514417"><a name="p16741205514417"></a><a name="p16741205514417"></a>函数的描述。</p>
</td>
</tr>
<tr id="row1741175524419"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p137411559442"><a name="p137411559442"></a><a name="p137411559442"></a>handler</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p9741125511443"><a name="p9741125511443"></a><a name="p9741125511443"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p17741255134419"><a name="p17741255134419"></a><a name="p17741255134419"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p1374118556446"><a name="p1374118556446"></a><a name="p1374118556446"></a>函数执行入口，请参考<a href="FunctionGraph函数模型.md#table357132064218">表1</a>。</p>
</td>
</tr>
<tr id="row1741105517449"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p1774114559446"><a name="p1774114559446"></a><a name="p1774114559446"></a>memory_size</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p13742155544414"><a name="p13742155544414"></a><a name="p13742155544414"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p10742555124414"><a name="p10742555124414"></a><a name="p10742555124414"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p1074245514442"><a name="p1074245514442"></a><a name="p1074245514442"></a>函数消耗的内存，单位M，取值范围为：128、256、512、768、1024、1280、1536、1792、2048、2560、3072、3584、4096。最小值为128，最大值为4096。</p>
</td>
</tr>
<tr id="row18742155519442"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p1474285554419"><a name="p1474285554419"></a><a name="p1474285554419"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p874205516445"><a name="p874205516445"></a><a name="p874205516445"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p1174255516448"><a name="p1174255516448"></a><a name="p1174255516448"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p157421355114414"><a name="p157421355114414"></a><a name="p157421355114414"></a>函数的超时时间。</p>
</td>
</tr>
<tr id="row8742355104420"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p9742175515447"><a name="p9742175515447"></a><a name="p9742175515447"></a>user_data</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p274235554415"><a name="p274235554415"></a><a name="p274235554415"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p15742205515443"><a name="p15742205515443"></a><a name="p15742205515443"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p1774215524416"><a name="p1774215524416"></a><a name="p1774215524416"></a>用户自定义的name/value参数。</p>
</td>
</tr>
<tr id="row188511757114411"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p98519572447"><a name="p98519572447"></a><a name="p98519572447"></a>dependency_pkg</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p985112575448"><a name="p985112575448"></a><a name="p985112575448"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p1685165744418"><a name="p1685165744418"></a><a name="p1685165744418"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p12816329164214"><a name="p12816329164214"></a><a name="p12816329164214"></a>函数使用的第三方软件zip包在obs上的url地址。</p>
</td>
</tr>
<tr id="row0742155584410"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p4742115518447"><a name="p4742115518447"></a><a name="p4742115518447"></a>xrole</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p57425559449"><a name="p57425559449"></a><a name="p57425559449"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p774225511448"><a name="p774225511448"></a><a name="p774225511448"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p1674245594418"><a name="p1674245594418"></a><a name="p1674245594418"></a>如函数需要访问其他云服务，则必填。</p>
</td>
</tr>
<tr id="row4465731163315"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p1796105543714"><a name="p1796105543714"></a><a name="p1796105543714"></a>app_xrole</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p13961055143716"><a name="p13961055143716"></a><a name="p13961055143716"></a>*string</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p1096175510373"><a name="p1096175510373"></a><a name="p1096175510373"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p149655583711"><a name="p149655583711"></a><a name="p149655583711"></a>如函数需要访问其他云服务app，则必填。</p>
</td>
</tr>
<tr id="row753033483320"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p096195563711"><a name="p096195563711"></a><a name="p096195563711"></a>initializer_handler</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p12961055143713"><a name="p12961055143713"></a><a name="p12961055143713"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p09610551371"><a name="p09610551371"></a><a name="p09610551371"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p696455113716"><a name="p696455113716"></a><a name="p696455113716"></a>函数初始化入口。</p>
</td>
</tr>
<tr id="row11923135519349"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p139617552371"><a name="p139617552371"></a><a name="p139617552371"></a>initializer_timeout</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p1996165518371"><a name="p1996165518371"></a><a name="p1996165518371"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p496175573717"><a name="p496175573717"></a><a name="p496175573717"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p7961355133715"><a name="p7961355133715"></a><a name="p7961355133715"></a>函数的初始化时间，范围1~300秒。</p>
</td>
</tr>
<tr id="row812074163518"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p11961455113712"><a name="p11961455113712"></a><a name="p11961455113712"></a>func_vpc. subnet_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p179616554378"><a name="p179616554378"></a><a name="p179616554378"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p1596125543711"><a name="p1596125543711"></a><a name="p1596125543711"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p2961955113715"><a name="p2961955113715"></a><a name="p2961955113715"></a>虚拟私有云子网编号。</p>
</td>
</tr>
<tr id="row48462183512"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p2961455203714"><a name="p2961455203714"></a><a name="p2961455203714"></a>func_vpc.vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p1196135583715"><a name="p1196135583715"></a><a name="p1196135583715"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p1396145519371"><a name="p1396145519371"></a><a name="p1396145519371"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p10961155153719"><a name="p10961155153719"></a><a name="p10961155153719"></a>虚拟私有云唯一标识。</p>
</td>
</tr>
</tbody>
</table>

**请求示例**

```
PUT  
/v2/7aad83af3e8d42e99ac194e8419e2c9b/fgs/functions/urn:fss:cn-north-1:7aad83af3e8d42e99ac194e8419e2c9b:function:default:test:latest/config HTTP/1.1 
{ 
  "description": "", 
  "handler": "test.handler", 
  "memory_size": 128, 
  "timeout": 3, 
  "runtime": "Python", 
  "user_data": "", 
  "code_type": "inline", 
  "func_code": { 
    "file": "aW1wb3J0IGpzb24KZGVmIGhhbmRsZXIgKGV2ZW50LCBjb250ZXh0KToKICAgIG91dHB1dCA9ICdIZWxsbyBtZXNzYWdlOiAnICsganNvbi5kdW1wcyhldmVudCkKICAgIHJldHVybiBvdXRwdXQ=" 
  }, 
  "xrole": "cffservice" 
}
```

## 响应消息<a name="section7552125518446"></a>

**响应参数**

响应参数如[表3](#table394445163918)所示。    

**表 3**  响应参数

<a name="table394445163918"></a>
<table><thead align="left"><tr id="row5944851163912"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.4.1.1"><p id="p7944165193912"><a name="p7944165193912"></a><a name="p7944165193912"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.112511251125113%" id="mcps1.2.4.1.2"><p id="p494413519391"><a name="p494413519391"></a><a name="p494413519391"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.68546854685468%" id="mcps1.2.4.1.3"><p id="p159441351193918"><a name="p159441351193918"></a><a name="p159441351193918"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row898316393534"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p60439610"><a name="p60439610"></a><a name="p60439610"></a>func_urn</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p159832399530"><a name="p159832399530"></a><a name="p159832399530"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p63770254"><a name="p63770254"></a><a name="p63770254"></a>函数的URN（Uniform Resource Name），唯一标识函数。</p>
</td>
</tr>
<tr id="row42001372535"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p49181313"><a name="p49181313"></a><a name="p49181313"></a>func_name</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p5201173725318"><a name="p5201173725318"></a><a name="p5201173725318"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p24263425"><a name="p24263425"></a><a name="p24263425"></a>函数名称。</p>
</td>
</tr>
<tr id="row18461113155312"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p38405776"><a name="p38405776"></a><a name="p38405776"></a>user_domain</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p02891635145919"><a name="p02891635145919"></a><a name="p02891635145919"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p23860166"><a name="p23860166"></a><a name="p23860166"></a>租户名称。</p>
</td>
</tr>
<tr id="row12325311185316"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p12865660"><a name="p12865660"></a><a name="p12865660"></a>namespace</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p830113515915"><a name="p830113515915"></a><a name="p830113515915"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p35485571"><a name="p35485571"></a><a name="p35485571"></a>租户的project id。</p>
</td>
</tr>
<tr id="row42345816531"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p32068643"><a name="p32068643"></a><a name="p32068643"></a>project_name</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p73101735165919"><a name="p73101735165919"></a><a name="p73101735165919"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p47423267"><a name="p47423267"></a><a name="p47423267"></a>租户的project name。</p>
</td>
</tr>
<tr id="row71958611537"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p10497128"><a name="p10497128"></a><a name="p10497128"></a>package</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p10319103585917"><a name="p10319103585917"></a><a name="p10319103585917"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p44961053"><a name="p44961053"></a><a name="p44961053"></a>函数所属的分组Package，用于用户针对函数的自定义分组。</p>
</td>
</tr>
<tr id="row1121313416531"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p27482234"><a name="p27482234"></a><a name="p27482234"></a>runtime</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p143291358595"><a name="p143291358595"></a><a name="p143291358595"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p652094462816"><a name="p652094462816"></a><a name="p652094462816"></a>FunctionGraph函数的执行环境，支持Node.js6.10、Python2.7、Python3.6、Java8、Go1.8、Node.js 8.10、C#.NET Core 2.0、C#.NET Core 2.1。</p>
</td>
</tr>
<tr id="row16165192105318"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p39009036"><a name="p39009036"></a><a name="p39009036"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p9339035135910"><a name="p9339035135910"></a><a name="p9339035135910"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p5615384"><a name="p5615384"></a><a name="p5615384"></a>函数执行超时时间，超时函数将被强行停止，范围3～900秒。</p>
</td>
</tr>
<tr id="row12238205710522"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p67083165"><a name="p67083165"></a><a name="p67083165"></a>handler</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p535063516598"><a name="p535063516598"></a><a name="p535063516598"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p65027307"><a name="p65027307"></a><a name="p65027307"></a>函数执行入口，规则：xx.xx，必须包含“. ”，举例：对于node.js函数：myfunction.handler，则表示函数的文件名为myfunction.js，执行的入口函数名为handler。</p>
</td>
</tr>
<tr id="row1229205512521"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p26048945"><a name="p26048945"></a><a name="p26048945"></a>memory_size</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p6360153545914"><a name="p6360153545914"></a><a name="p6360153545914"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p29589819"><a name="p29589819"></a><a name="p29589819"></a>函数消耗的内存，单位M，取值范围为：128、256、512、768、1024、1280、1536、1792、2048、2560、3072、3584、4096。最小值为128，最大值为4096。</p>
</td>
</tr>
<tr id="row192981153205213"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p29032981"><a name="p29032981"></a><a name="p29032981"></a>cpu</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p168801912184317"><a name="p168801912184317"></a><a name="p168801912184317"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p2861285"><a name="p2861285"></a><a name="p2861285"></a>函数占用的cpu资源，单位为millicore（1 core=1000 millicores），取值与MemorySize成比例，默认是128M内存占0.1个核（100 millicores），函数占用的CPU为基础CPU：200 millicores，再加上内存按比例占用的CPU，计算方法：内存/128 *100 + 200。</p>
</td>
</tr>
<tr id="row618615514526"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p5502495"><a name="p5502495"></a><a name="p5502495"></a>code_type</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p1738033513599"><a name="p1738033513599"></a><a name="p1738033513599"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p43048911"><a name="p43048911"></a><a name="p43048911"></a>函数代码类型，取值有4种：</p>
<p id="p51895880"><a name="p51895880"></a><a name="p51895880"></a>inline：UI在线编辑代码</p>
<p id="p64409739"><a name="p64409739"></a><a name="p64409739"></a>zip：函数代码为zip包</p>
<p id="p42816746"><a name="p42816746"></a><a name="p42816746"></a>jar：函数代码为jar包，主要针对Java函数</p>
<p id="p49806396"><a name="p49806396"></a><a name="p49806396"></a>obs：函数代码来源于obs存储</p>
</td>
</tr>
<tr id="row1854324825113"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p2967967"><a name="p2967967"></a><a name="p2967967"></a>code_url</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p38271640155912"><a name="p38271640155912"></a><a name="p38271640155912"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p11470128149"><a name="p11470128149"></a><a name="p11470128149"></a>当CodeType为obs时，该值为函数代码包在OBS上的地址，CodeType为其他值时，该字段为空。</p>
</td>
</tr>
<tr id="row761414555118"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p34277422"><a name="p34277422"></a><a name="p34277422"></a>code_filename</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p3839240115913"><a name="p3839240115913"></a><a name="p3839240115913"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p25007806"><a name="p25007806"></a><a name="p25007806"></a>函数的文件名，当CodeType为jar/zip时必须提供该字段，inline和obs不需要提供。</p>
</td>
</tr>
<tr id="row45128232510"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p44188613"><a name="p44188613"></a><a name="p44188613"></a>code_size</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p485417296439"><a name="p485417296439"></a><a name="p485417296439"></a>int64</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p22507915"><a name="p22507915"></a><a name="p22507915"></a>函数大小，单位：字节。</p>
</td>
</tr>
<tr id="row112081421205117"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p33707641"><a name="p33707641"></a><a name="p33707641"></a>user_data</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p1861440185912"><a name="p1861440185912"></a><a name="p1861440185912"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p45964432"><a name="p45964432"></a><a name="p45964432"></a>用户自定义的name/value信息，在函数中使用的参数，举例：如函数要访问某个主机，可以设置自定义参数：Host={host_ip}，最多定义20个，总长度不超过4KB。</p>
</td>
</tr>
<tr id="row12112101985115"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p20747816"><a name="p20747816"></a><a name="p20747816"></a>digest</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p1687714404594"><a name="p1687714404594"></a><a name="p1687714404594"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p2851512"><a name="p2851512"></a><a name="p2851512"></a>函数代码SHA512 hash值，用于判断函数是否变化。</p>
</td>
</tr>
<tr id="row134021765117"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p65486773"><a name="p65486773"></a><a name="p65486773"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p388920409598"><a name="p388920409598"></a><a name="p388920409598"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p2828410"><a name="p2828410"></a><a name="p2828410"></a>函数版本号，由系统自动生成，规则：vYYYYMMDD-HHMMSS（v+年月日-时分秒）。</p>
</td>
</tr>
<tr id="row162071015105114"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p48645199"><a name="p48645199"></a><a name="p48645199"></a>image_name</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p189011840195919"><a name="p189011840195919"></a><a name="p189011840195919"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p47947026"><a name="p47947026"></a><a name="p47947026"></a>函数版本的内部标识。</p>
</td>
</tr>
<tr id="row1251115812517"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p56772777"><a name="p56772777"></a><a name="p56772777"></a>xrole</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p139143403598"><a name="p139143403598"></a><a name="p139143403598"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p35192261"><a name="p35192261"></a><a name="p35192261"></a>函数使用的权限委托名称，需要IAM支持，并在IAM界面创建委托，当函数需要访问其他服务时，必须提供该字段。</p>
</td>
</tr>
<tr id="row354514614513"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p15157838201310"><a name="p15157838201310"></a><a name="p15157838201310"></a>app_xrole</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p944454618436"><a name="p944454618436"></a><a name="p944454618436"></a>*string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p215783891315"><a name="p215783891315"></a><a name="p215783891315"></a>函数app使用的权限委托名称，需要IAM支持，并在IAM界面创建委托，当函数需要访问其他服务时，必须提供该字段。</p>
</td>
</tr>
<tr id="row1937154145711"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p1947817508576"><a name="p1947817508576"></a><a name="p1947817508576"></a>dependency_pkg</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p13478750125716"><a name="p13478750125716"></a><a name="p13478750125716"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p129371741195717"><a name="p129371741195717"></a><a name="p129371741195717"></a>函数依赖的第三方软件zip包在obs上的地址，多个第三方软件要打包到一个zip文件中，如果未使用第三方软件，此处不填。</p>
</td>
</tr>
<tr id="row848184115116"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p19572290"><a name="p19572290"></a><a name="p19572290"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p17880477596"><a name="p17880477596"></a><a name="p17880477596"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p41851680"><a name="p41851680"></a><a name="p41851680"></a>函数描述。</p>
</td>
</tr>
<tr id="row722816218514"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p42450590"><a name="p42450590"></a><a name="p42450590"></a>version_description</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p7991247145910"><a name="p7991247145910"></a><a name="p7991247145910"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p15945784"><a name="p15945784"></a><a name="p15945784"></a>函数版本描述。</p>
</td>
</tr>
<tr id="row19286204517"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p14643338"><a name="p14643338"></a><a name="p14643338"></a>last_modified</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p20110547185915"><a name="p20110547185915"></a><a name="p20110547185915"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p45259754"><a name="p45259754"></a><a name="p45259754"></a>函数最后一次更新时间。</p>
</td>
</tr>
<tr id="row196151954414"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p136151911443"><a name="p136151911443"></a><a name="p136151911443"></a>func_code</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p13611819124413"><a name="p13611819124413"></a><a name="p13611819124413"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p186114196443"><a name="p186114196443"></a><a name="p186114196443"></a>函数代码，请参考<a href="获取函数列表.md#table535915353505">表4</a>。</p>
</td>
</tr>
<tr id="row188192822711"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p78812287273"><a name="p78812287273"></a><a name="p78812287273"></a>depend_list</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p1120815202451"><a name="p1120815202451"></a><a name="p1120815202451"></a>[]string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p18881182842710"><a name="p18881182842710"></a><a name="p18881182842710"></a>依赖包列表。</p>
</td>
</tr>
<tr id="row1732519315277"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p163252312270"><a name="p163252312270"></a><a name="p163252312270"></a>strategy_config</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p1832518315276"><a name="p1832518315276"></a><a name="p1832518315276"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p18325531142712"><a name="p18325531142712"></a><a name="p18325531142712"></a>函数策略配置，请参考<a href="#table1654695031117">表4</a>。</p>
</td>
</tr>
<tr id="row1576510114465"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p212451417468"><a name="p212451417468"></a><a name="p212451417468"></a>dependencies</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p612410148467"><a name="p612410148467"></a><a name="p612410148467"></a>[]*string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p3124514134619"><a name="p3124514134619"></a><a name="p3124514134619"></a>依赖代码包。</p>
</td>
</tr>
<tr id="row16431056468"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p2124111418467"><a name="p2124111418467"></a><a name="p2124111418467"></a>initializer_handler</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p17124121413461"><a name="p17124121413461"></a><a name="p17124121413461"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p2012419143463"><a name="p2012419143463"></a><a name="p2012419143463"></a>函数初始化入口，规则：xx.xx，必须包含“. ”，举例：对于node.js函数：myfunction.initializer，则表示函数的文件名为myfunction.js，初始化的入口函数名为initializer。</p>
</td>
</tr>
<tr id="row15632571461"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p6124181412461"><a name="p6124181412461"></a><a name="p6124181412461"></a>initializer_timeout</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p18124714154615"><a name="p18124714154615"></a><a name="p18124714154615"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p1412451494619"><a name="p1412451494619"></a><a name="p1412451494619"></a>初始化超时时间，超时函数将被强行停止，范围1～300秒。</p>
</td>
</tr>
<tr id="row535113129465"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p712461414612"><a name="p712461414612"></a><a name="p712461414612"></a>func_vpc</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p412411417460"><a name="p412411417460"></a><a name="p412411417460"></a>*string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p17126171454619"><a name="p17126171454619"></a><a name="p17126171454619"></a>vpc配置，请参考<a href="获取函数列表.md#table11522131317013">表6 func_vpc参数说明</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  strategy\_config参数说明

<a name="table1654695031117"></a>
<table><thead align="left"><tr id="row175461750151117"><th class="cellrowborder" valign="top" width="18%" id="mcps1.2.5.1.1"><p id="p054605019114"><a name="p054605019114"></a><a name="p054605019114"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p1854695001111"><a name="p1854695001111"></a><a name="p1854695001111"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.3"><p id="p105472050141110"><a name="p105472050141110"></a><a name="p105472050141110"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="53%" id="mcps1.2.5.1.4"><p id="p254755018117"><a name="p254755018117"></a><a name="p254755018117"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1354725017111"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.1 "><p id="p2547105010118"><a name="p2547105010118"></a><a name="p2547105010118"></a>concurrency</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p1554795091117"><a name="p1554795091117"></a><a name="p1554795091117"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.3 "><p id="p195479501116"><a name="p195479501116"></a><a name="p195479501116"></a>必选</p>
</td>
<td class="cellrowborder" valign="top" width="53%" headers="mcps1.2.5.1.4 "><p id="p20547150111114"><a name="p20547150111114"></a><a name="p20547150111114"></a>0：函数被禁用。</p>
<p id="p155471650141112"><a name="p155471650141112"></a><a name="p155471650141112"></a>-1：函数被启用。</p>
</td>
</tr>
</tbody>
</table>

**响应示例**

成功时的返回格式：

```
HTTP/1.1 200 
{       
    "func_urn": "urn:fss:cn-north-1:7aad83af3e8d42e99ac194e8419e2c9b:function:default:test",      
    "func_name": "test",      
    "user_domain": "cff01_hk",      
    "namespace": "7aad83af3e8d42e99ac194e8419e2c9b",      
    "project_name": "cn-north-1",       
    "package": "default",      
    "runtime": "Node.js6.10",       
    "timeout": 3,       
    "handler": "test.handler",      
    "memory_size": 128,      
    "cpu": 300,      
    "code_type": "inline",      
    "code_url": "",      
    "code_filename": "index.js",      
    "code_size": 272,       
    "user_data": "",      
    "digest": "decbce6939297b0b5ec6d1a23bf9c725870f5e69fc338a89a6a4029264688dc26338f56d08b6535de47f15ad538e22ca66613b9a46f807d50b687bb53fded1c6",  
    "version": "latest",                                   
    "image_name": "latest-5qe8e",      
    "xrole": "cff", 
 "app_xrole": null   
    "dependency_pkg": "",      
    "description": "111",     
    "version_description": "",     
    "last_modified": "2018-03-28T11:30:32+08:00", 
 "func_code": {    
   "file": "",    
   "link": "" 
 }, 
   "func_vpc":null   
   "depend_list": null,  
   "strategy_config": {      
      "concurrency": -1
 },  
   "extend_config": "",   
   "dependencies": null,
  "initializer_handler": "index.initializer",
  "initializer_timeout": 3 
    }
```

失败时的返回格式（示例）：

```
HTTP/1.1 404 Not Found 
{ 
  "error_code": "FSS.1051", 
  "error_msg": "Not found the function" 
 }
```

## 状态码<a name="section05863551442"></a>

状态码说明如[表5](#table1458815564417)所示。

**表 5**  状态码说明

<a name="table1458815564417"></a>
<table><thead align="left"><tr id="row13744195564411"><th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.3.1.1"><p id="p107441055204411"><a name="p107441055204411"></a><a name="p107441055204411"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="86.87%" id="mcps1.2.3.1.2"><p id="p17744355174417"><a name="p17744355174417"></a><a name="p17744355174417"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row674485512444"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p274414554449"><a name="p274414554449"></a><a name="p274414554449"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p11744955194412"><a name="p11744955194412"></a><a name="p11744955194412"></a>InvalidParameterValueException：输入参数错误。</p>
</td>
</tr>
<tr id="row874485584413"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p1674414553444"><a name="p1674414553444"></a><a name="p1674414553444"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p274415554443"><a name="p274415554443"></a><a name="p274415554443"></a>UnauthorizedAccess：未授权的访问。</p>
</td>
</tr>
<tr id="row1877711344401"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p277743415407"><a name="p277743415407"></a><a name="p277743415407"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p9777133412404"><a name="p9777133412404"></a><a name="p9777133412404"></a>Forbidden：禁止访问。</p>
</td>
</tr>
<tr id="row774545534412"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p18745135515448"><a name="p18745135515448"></a><a name="p18745135515448"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p20745155510440"><a name="p20745155510440"></a><a name="p20745155510440"></a>ResourceNotFoundException：要修改的函数没有找到。</p>
</td>
</tr>
<tr id="row20932171092117"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p14179142824616"><a name="p14179142824616"></a><a name="p14179142824616"></a>409</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p517912813469"><a name="p517912813469"></a><a name="p517912813469"></a>ResourceConflictException：函数已存在。</p>
</td>
</tr>
<tr id="row18745105512445"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p8745185584416"><a name="p8745185584416"></a><a name="p8745185584416"></a>429</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p207451155134415"><a name="p207451155134415"></a><a name="p207451155134415"></a>TooManyRequestsException：并发请求数太多。</p>
</td>
</tr>
<tr id="row074595519442"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p20745655124414"><a name="p20745655124414"></a><a name="p20745655124414"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p074575534411"><a name="p074575534411"></a><a name="p074575534411"></a>InternalServerError：服务内部出错。</p>
</td>
</tr>
</tbody>
</table>

