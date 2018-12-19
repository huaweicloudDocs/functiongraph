# 修改函数的metadata信息<a name="functiongraph_06_0111"></a>

## 功能介绍<a name="section14487165524413"></a>

修改指定的函数的metadata信息。

## URI<a name="section19488125564417"></a>

URL：/v1.0/\{project\_id\}/fss/functions/\{function\_urn\}/config

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

>![](public_sys-resources/icon-note.gif) **说明：**   
>各字段的详细解释请见[表1](FunctionGraph函数模型.md#table4539774994724)。  

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
<tr id="row1574111556448"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p1574135517441"><a name="p1574135517441"></a><a name="p1574135517441"></a>Description</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p5741655184415"><a name="p5741655184415"></a><a name="p5741655184415"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p167412555449"><a name="p167412555449"></a><a name="p167412555449"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p16741205514417"><a name="p16741205514417"></a><a name="p16741205514417"></a>函数的描述。</p>
</td>
</tr>
<tr id="row1741175524419"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p137411559442"><a name="p137411559442"></a><a name="p137411559442"></a>Handler</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p9741125511443"><a name="p9741125511443"></a><a name="p9741125511443"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p17741255134419"><a name="p17741255134419"></a><a name="p17741255134419"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p1374118556446"><a name="p1374118556446"></a><a name="p1374118556446"></a>函数执行入口，请参考<a href="FunctionGraph函数模型.md#table4539774994724">表1</a>。</p>
</td>
</tr>
<tr id="row1741105517449"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p1774114559446"><a name="p1774114559446"></a><a name="p1774114559446"></a>MemorySize</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p13742155544414"><a name="p13742155544414"></a><a name="p13742155544414"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p10742555124414"><a name="p10742555124414"></a><a name="p10742555124414"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p1074245514442"><a name="p1074245514442"></a><a name="p1074245514442"></a>函数消耗的内存，单位M，取值为128的整数倍，最小值为128，最大值为1536。</p>
</td>
</tr>
<tr id="row18742155519442"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p1474285554419"><a name="p1474285554419"></a><a name="p1474285554419"></a>Timeout</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p874205516445"><a name="p874205516445"></a><a name="p874205516445"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p1174255516448"><a name="p1174255516448"></a><a name="p1174255516448"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p157421355114414"><a name="p157421355114414"></a><a name="p157421355114414"></a>函数的超时时间。</p>
</td>
</tr>
<tr id="row8742355104420"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p9742175515447"><a name="p9742175515447"></a><a name="p9742175515447"></a>UserData</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p274235554415"><a name="p274235554415"></a><a name="p274235554415"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p15742205515443"><a name="p15742205515443"></a><a name="p15742205515443"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p1774215524416"><a name="p1774215524416"></a><a name="p1774215524416"></a>用户自定义的name/value参数。</p>
</td>
</tr>
<tr id="row188511757114411"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p98519572447"><a name="p98519572447"></a><a name="p98519572447"></a>DependencyPkg</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p985112575448"><a name="p985112575448"></a><a name="p985112575448"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p1685165744418"><a name="p1685165744418"></a><a name="p1685165744418"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p12816329164214"><a name="p12816329164214"></a><a name="p12816329164214"></a>函数使用的第三方软件zip包在obs上的url地址。</p>
</td>
</tr>
<tr id="row67135710118"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p135221211191211"><a name="p135221211191211"></a><a name="p135221211191211"></a>StrategyConfig</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p56896254128"><a name="p56896254128"></a><a name="p56896254128"></a>StrategyConfig</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p39195715112"><a name="p39195715112"></a><a name="p39195715112"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p191757161119"><a name="p191757161119"></a><a name="p191757161119"></a>函数策略配置，请参考<a href="#table4775818446">表3</a>。</p>
</td>
</tr>
<tr id="row0742155584410"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.2.5.1.1 "><p id="p4742115518447"><a name="p4742115518447"></a><a name="p4742115518447"></a>Xrole</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.5.1.2 "><p id="p57425559449"><a name="p57425559449"></a><a name="p57425559449"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="12.121212121212121%" headers="mcps1.2.5.1.3 "><p id="p774225511448"><a name="p774225511448"></a><a name="p774225511448"></a>可选</p>
</td>
<td class="cellrowborder" valign="top" width="54.545454545454554%" headers="mcps1.2.5.1.4 "><p id="p1674245594418"><a name="p1674245594418"></a><a name="p1674245594418"></a>如函数需要访问其他云服务，则必填。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  StrategyConfig参数说明

<a name="table4775818446"></a>
<table><thead align="left"><tr id="row17785844414"><th class="cellrowborder" valign="top" width="18%" id="mcps1.2.5.1.1"><p id="p771581446"><a name="p771581446"></a><a name="p771581446"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.2"><p id="p1773582447"><a name="p1773582447"></a><a name="p1773582447"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.3"><p id="p107115884415"><a name="p107115884415"></a><a name="p107115884415"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="53%" id="mcps1.2.5.1.4"><p id="p974580442"><a name="p974580442"></a><a name="p974580442"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row47195819446"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.1 "><p id="p17775834410"><a name="p17775834410"></a><a name="p17775834410"></a>Concurrency</p>
</td>
<td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.2 "><p id="p9285359487"><a name="p9285359487"></a><a name="p9285359487"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.3 "><p id="p13745811441"><a name="p13745811441"></a><a name="p13745811441"></a>必选</p>
</td>
<td class="cellrowborder" valign="top" width="53%" headers="mcps1.2.5.1.4 "><p id="p13755817443"><a name="p13755817443"></a><a name="p13755817443"></a>0：函数被禁用。</p>
<p id="p1411826144918"><a name="p1411826144918"></a><a name="p1411826144918"></a>-1：函数被启用。</p>
</td>
</tr>
</tbody>
</table>

**请求示例**

```
PUT /v1.0/7aad83af3e8d42e99ac194e8419e2c9b/fss/functions/urn:fss:cn-north-1:7aad83af3e8d42e99ac194e8419e2c9b:function:default:test:latest/config HTTP/1.1{  
"Description": "",  
"Handler": "test.handler",  
"MemorySize": 128,  
"Timeout": 3,  
"Runtime": "Python",  
"UserData": "",  
"CodeType": "inline",  
"FuncCode": {"File":"aW1wb3J0IGpzb24KZGVmIGhhbmRsZXIgKGV2ZW50LCBjb250ZXh0KToKICAgIG91dHB1dCA9ICdIZWxsbyBtZXNzYWdlOiAnICsganNvbi5kdW1wcyhldmVudCkKICAgIHJldHVybiBvdXRwdXQ="  },
"StrategyConfig":{
	"Concurrency":0
}
"Xrole": "cffservice"
}
```

## 响应消息<a name="section7552125518446"></a>

**响应参数**

函数的metadata信息：JSON对象，表示指定函数的metadata信息。

**响应示例**

成功时的返回格式：

```
HTTP/1.1 200
{
  "CodeFileName": "index.js",
  "CodeSize": 173,
  "CodeType": "inline",
  "CodeUrl": "",
  "Cpu": 300,
  "DependencyPkg": "",
  "Description": "",
  "Digest": "fe3d5f53536af46985e59332ece1a2dca785309937af90502745a565cf0c9ba8ebec45d70d2f31a83bd13cbf618a0ffb4e60470389da494a214213e15e4049fb",
  "FuncName": "HelloWorld",
  "FuncUrn": "urn:fss:cn-hk1:284f722ca42d465397ada4d9381c5eac:function:default:HelloWorld:latest",
  "Handler": "index.handler",
  "ImageName": "latest-fhzsf",
  "LastModified": "2018-08-23T14:17:17+08:00",
  "MemorySize": 128,
  "Namespace": "284f722ca42d465397ada4d9381c5eac",
  "Package": "default",
  "ProjectName": "cn-hk1",
  "Runtime": "Node.js6.10",
  "StrategyConfig": {
   "Concurrency": 0
  },
  "Subnet": "",
  "SubnetId": "",
  "Timeout": 3,
  "UserData": "",
  "UserDomain": "ecmuseryy",
  "Version": "latest",
  "VersionDescription": "",
  "Vpc": "",
  "VpcId": "",
  "Xrole": ""
 }
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

状态码说明如[表4](#table1458815564417)所示。

**表 4**  状态码说明

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

