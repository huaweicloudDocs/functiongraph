# FunctionGraph函数模型<a name="ZH-CN_TOPIC_0115410472"></a>

## 函数模型<a name="section26908673"></a>

FunctionGraph函数模型如下。

```
{ 
  "functions": [ 
   { 
    "func_urn": "urn:fss:xxxxxxxxx:7aad83af3e8d42e99ac194e8419e2c9b:function:default:test", 
    "func_name": "test", 
    "domain_id": "cff01_hk", 
    "namespace": "7aad83af3e8d42e99ac194e8419e2c9b", 
    "project_name": "xxxxxxxxxx", 
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
    "app_xrole": null, 
    "description": "111", 
    "version_description": "", 
    "last_modified": "2018-03-28T11:30:32+08:00",
"func_code": {
  "file": "",
  "link": ""
 },
 "func_vpc":null,
 "mount_config":null,
 "depend_list": null,
 "strategy_config": {
     "concurrency": -1
 },
 "extend_config": "",
 "dependencies": null,
"initializer_handler": "index.initializer",
"initializer_timeout": 3  
   } 
  ], 
  "next_marker": 45 
 }
```

## 字段说明<a name="section40851470"></a>

FunctionGraph函数字段说明如[表1](#table357132064218)所示。

**表 1**  FunctionGraph函数字段说明表

<a name="table357132064218"></a>
<table><thead align="left"><tr id="row558102011425"><th class="cellrowborder" valign="top" width="29.9%" id="mcps1.2.3.1.1"><p id="p1273950184418"><a name="p1273950184418"></a><a name="p1273950184418"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="70.1%" id="mcps1.2.3.1.2"><p id="p273940124410"><a name="p273940124410"></a><a name="p273940124410"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2058142011422"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p1774017018446"><a name="p1774017018446"></a><a name="p1774017018446"></a>func_urn</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p874014034412"><a name="p874014034412"></a><a name="p874014034412"></a>函数的URN（Uniform Resource Name），唯一标识函数。</p>
</td>
</tr>
<tr id="row132313449427"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p474050194419"><a name="p474050194419"></a><a name="p474050194419"></a>func_name</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p974012024419"><a name="p974012024419"></a><a name="p974012024419"></a>函数名称。</p>
</td>
</tr>
<tr id="row19450204274311"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p107401703448"><a name="p107401703448"></a><a name="p107401703448"></a>domain_id</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p974015010440"><a name="p974015010440"></a><a name="p974015010440"></a>租户名称。</p>
</td>
</tr>
<tr id="row7467440154318"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p1074014024411"><a name="p1074014024411"></a><a name="p1074014024411"></a>namespace</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p19740603447"><a name="p19740603447"></a><a name="p19740603447"></a>租户的project id。</p>
</td>
</tr>
<tr id="row840763884314"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p1374018015443"><a name="p1374018015443"></a><a name="p1374018015443"></a>project_name</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p1374050114412"><a name="p1374050114412"></a><a name="p1374050114412"></a>租户的project name。</p>
</td>
</tr>
<tr id="row1621603614433"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p1874018019449"><a name="p1874018019449"></a><a name="p1874018019449"></a>package</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p77411044415"><a name="p77411044415"></a><a name="p77411044415"></a>函数所属的分组Package，用于用户针对函数的自定义分组。</p>
</td>
</tr>
<tr id="row821715346434"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p1741501443"><a name="p1741501443"></a><a name="p1741501443"></a>runtime</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p1274120064410"><a name="p1274120064410"></a><a name="p1274120064410"></a>FunctionGraph函数的执行环境，支持Node.js6.10、Python2.7、Python3.6、Java8、Go1.8、Node.js 8.10、C#.NET Core 2.0、C#.NET Core 2.1、PHP7.3。</p>
</td>
</tr>
<tr id="row145081418204316"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p47413017444"><a name="p47413017444"></a><a name="p47413017444"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p1674130144417"><a name="p1674130144417"></a><a name="p1674130144417"></a>函数执行超时时间，超时函数将被强行停止，范围3～900秒。</p>
</td>
</tr>
<tr id="row13357432164311"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p174119084415"><a name="p174119084415"></a><a name="p174119084415"></a>handler</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p67418010444"><a name="p67418010444"></a><a name="p67418010444"></a>函数执行入口，规则：xx.xx，必须包含“. ”，举例：对于node.js函数：myfunction.handler，则表示函数的文件名为myfunction.js，执行的入口函数名为handler。</p>
</td>
</tr>
<tr id="row162211430104319"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p197415018448"><a name="p197415018448"></a><a name="p197415018448"></a>memory_size</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p27416019446"><a name="p27416019446"></a><a name="p27416019446"></a>函数消耗的内存，单位M，取值范围为：128、256、512、768、1024、1280、1536、1792、2048、2560、3072、3584、4096。最小值为128，最大值为4096。</p>
</td>
</tr>
<tr id="row130522794317"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p207413016447"><a name="p207413016447"></a><a name="p207413016447"></a>cpu</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p9741160124417"><a name="p9741160124417"></a><a name="p9741160124417"></a>函数占用的cpu资源，单位为millicore（1 core=1000 millicores），取值与MemorySize成比例，默认是128M内存占0.1个核（100 millicores），函数占用的CPU为基础CPU：200 millicores，再加上内存按比例占用的CPU，计算方法：内存/128 *100 + 200。</p>
</td>
</tr>
<tr id="row18433112518437"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p77411002443"><a name="p77411002443"></a><a name="p77411002443"></a>code_type</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p1474110012449"><a name="p1474110012449"></a><a name="p1474110012449"></a>函数代码类型，取值有4种：</p>
<p id="p87411907446"><a name="p87411907446"></a><a name="p87411907446"></a>inline：UI在线编辑代码。</p>
<p id="p1374212017443"><a name="p1374212017443"></a><a name="p1374212017443"></a>zip：函数代码为zip包。</p>
<p id="p3742003445"><a name="p3742003445"></a><a name="p3742003445"></a>jar：函数代码为jar包，主要针对Java函数。</p>
<p id="p117427014440"><a name="p117427014440"></a><a name="p117427014440"></a>obs：函数代码来源于obs存储。</p>
</td>
</tr>
<tr id="row15521923124316"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p167429044411"><a name="p167429044411"></a><a name="p167429044411"></a>code_url</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p1274219019446"><a name="p1274219019446"></a><a name="p1274219019446"></a>当CodeType为obs时，该值为函数代码包在OBS上的地址，CodeType为其他值时，该字段为空。</p>
</td>
</tr>
<tr id="row1076032104314"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p15742180144415"><a name="p15742180144415"></a><a name="p15742180144415"></a>code_filename</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p1074215024420"><a name="p1074215024420"></a><a name="p1074215024420"></a>函数的文件名，当CodeType为jar/zip时必须提供该字段，inline和obs不需要提供。</p>
</td>
</tr>
<tr id="row1786611604313"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p13742109448"><a name="p13742109448"></a><a name="p13742109448"></a>code_size</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p117421024416"><a name="p117421024416"></a><a name="p117421024416"></a>函数大小，单位：字节。</p>
</td>
</tr>
<tr id="row1313816154439"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p474211074410"><a name="p474211074410"></a><a name="p474211074410"></a>user_data</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p4742406449"><a name="p4742406449"></a><a name="p4742406449"></a>用户自定义的name/value信息，在函数中使用的参数，举例：如函数要访问某个主机，可以设置自定义参数：Host={host_ip}，最多定义20个，总长度不超过4KB。</p>
</td>
</tr>
<tr id="row15321141316432"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p14742110114416"><a name="p14742110114416"></a><a name="p14742110114416"></a>digest</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p15742002443"><a name="p15742002443"></a><a name="p15742002443"></a>函数代码SHA512 hash值，用于判断函数是否变化。</p>
</td>
</tr>
<tr id="row17618151119439"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p974216013446"><a name="p974216013446"></a><a name="p974216013446"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p107422034415"><a name="p107422034415"></a><a name="p107422034415"></a>函数版本号，由系统自动生成，规则：vYYYYMMDD-HHMMSS（v+年月日-时分秒）。</p>
</td>
</tr>
<tr id="row118764984320"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p1374213015448"><a name="p1374213015448"></a><a name="p1374213015448"></a>image_name</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p1774390144413"><a name="p1774390144413"></a><a name="p1774390144413"></a>函数版本的内部标识。</p>
</td>
</tr>
<tr id="row10631585435"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p574315014411"><a name="p574315014411"></a><a name="p574315014411"></a>xrole</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p17743130164413"><a name="p17743130164413"></a><a name="p17743130164413"></a>函数使用的权限委托名称，需要IAM支持，并在IAM界面创建委托，当函数需要访问其他服务时，必须提供该字段。</p>
</td>
</tr>
<tr id="row19915616434"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p1574319024410"><a name="p1574319024410"></a><a name="p1574319024410"></a>app_xrole</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p147431508447"><a name="p147431508447"></a><a name="p147431508447"></a>函数app使用的权限委托名称，需要IAM支持，并在IAM界面创建委托，当函数需要访问其他服务时，必须提供该字段。</p>
</td>
</tr>
<tr id="row02151805439"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p157431703447"><a name="p157431703447"></a><a name="p157431703447"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p1274319064417"><a name="p1274319064417"></a><a name="p1274319064417"></a>函数描述。</p>
</td>
</tr>
<tr id="row235572114311"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p1174319014445"><a name="p1174319014445"></a><a name="p1174319014445"></a>version_description</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p12743301441"><a name="p12743301441"></a><a name="p12743301441"></a>函数版本描述。</p>
</td>
</tr>
<tr id="row88955816423"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p17743160114417"><a name="p17743160114417"></a><a name="p17743160114417"></a>last_modified</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p1174340134418"><a name="p1174340134418"></a><a name="p1174340134418"></a>函数最后一次更新时间。</p>
</td>
</tr>
<tr id="row1596515594218"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p197432094419"><a name="p197432094419"></a><a name="p197432094419"></a>func_code</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p6743607447"><a name="p6743607447"></a><a name="p6743607447"></a>函数代码，请参考<a href="#table18312152434512">表2</a>。</p>
</td>
</tr>
<tr id="row121771142174218"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p37437016444"><a name="p37437016444"></a><a name="p37437016444"></a>depend_list</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p167439014447"><a name="p167439014447"></a><a name="p167439014447"></a>依赖包列表。</p>
</td>
</tr>
<tr id="row9126135413426"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p474415016449"><a name="p474415016449"></a><a name="p474415016449"></a>strategy_config</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p157447014443"><a name="p157447014443"></a><a name="p157447014443"></a>函数策略配置，请参考<a href="#table4775818446">表3</a>。</p>
</td>
</tr>
<tr id="row18851839194211"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p12744100104410"><a name="p12744100104410"></a><a name="p12744100104410"></a>extend_config</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p1874440134418"><a name="p1874440134418"></a><a name="p1874440134418"></a>函数扩展配置。</p>
</td>
</tr>
<tr id="row4581320174210"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p07441602444"><a name="p07441602444"></a><a name="p07441602444"></a>dependencies</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p177449017441"><a name="p177449017441"></a><a name="p177449017441"></a>依赖代码包列表，<a href="#table3788232112820">表5</a>。</p>
</td>
</tr>
<tr id="row1581820104216"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p1274416019446"><a name="p1274416019446"></a><a name="p1274416019446"></a>initializer_handler</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p11744209445"><a name="p11744209445"></a><a name="p11744209445"></a>函数初始化入口，规则：xx.xx，必须包含“. ”，举例：对于node.js函数：myfunction.initializer，则表示函数的文件名为myfunction.js，初始化的入口函数名为initializer。</p>
</td>
</tr>
<tr id="row105819201425"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p374413017443"><a name="p374413017443"></a><a name="p374413017443"></a>initializer_timeout</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p674419016442"><a name="p674419016442"></a><a name="p674419016442"></a>初始化超时时间，超时函数将被强行停止，范围1～300秒。</p>
</td>
</tr>
<tr id="row658520154217"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p167441016444"><a name="p167441016444"></a><a name="p167441016444"></a>func_vpc</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p874490104410"><a name="p874490104410"></a><a name="p874490104410"></a>vpc配置，请参考<a href="#table11522131317013">表4</a>。</p>
</td>
</tr>
<tr id="row1246812310125"><td class="cellrowborder" valign="top" width="29.9%" headers="mcps1.2.3.1.1 "><p id="p17468183191219"><a name="p17468183191219"></a><a name="p17468183191219"></a>mount_config</p>
</td>
<td class="cellrowborder" valign="top" width="70.1%" headers="mcps1.2.3.1.2 "><p id="p046818311219"><a name="p046818311219"></a><a name="p046818311219"></a>文件系统配置，请参考表 <a href="#table2317745151313">表6 mount_config参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 2**  func\_code参数说明

<a name="table18312152434512"></a>
<table><thead align="left"><tr id="row73120247459"><th class="cellrowborder" valign="top" width="30.080000000000002%" id="mcps1.2.3.1.1"><p id="p772853624514"><a name="p772853624514"></a><a name="p772853624514"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="69.92%" id="mcps1.2.3.1.2"><p id="p1563154174512"><a name="p1563154174512"></a><a name="p1563154174512"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row11312102412456"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="p187281036104520"><a name="p187281036104520"></a><a name="p187281036104520"></a>file</p>
</td>
<td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="p126354116451"><a name="p126354116451"></a><a name="p126354116451"></a>函数代码内容，接口返回空</p>
</td>
</tr>
<tr id="row19312424104514"><td class="cellrowborder" valign="top" width="30.080000000000002%" headers="mcps1.2.3.1.1 "><p id="p16728123614517"><a name="p16728123614517"></a><a name="p16728123614517"></a>link</p>
</td>
<td class="cellrowborder" valign="top" width="69.92%" headers="mcps1.2.3.1.2 "><p id="p12631141174510"><a name="p12631141174510"></a><a name="p12631141174510"></a>函数代码链接，接口返回空</p>
</td>
</tr>
</tbody>
</table>

**表 3**  strategy\_config参数说明

<a name="table4775818446"></a>
<table><thead align="left"><tr id="row17785844414"><th class="cellrowborder" valign="top" width="29.470000000000002%" id="mcps1.2.3.1.1"><p id="p771581446"><a name="p771581446"></a><a name="p771581446"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="70.53%" id="mcps1.2.3.1.2"><p id="p974580442"><a name="p974580442"></a><a name="p974580442"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row47195819446"><td class="cellrowborder" valign="top" width="29.470000000000002%" headers="mcps1.2.3.1.1 "><p id="p17775834410"><a name="p17775834410"></a><a name="p17775834410"></a>concurrency</p>
</td>
<td class="cellrowborder" valign="top" width="70.53%" headers="mcps1.2.3.1.2 "><p id="p13755817443"><a name="p13755817443"></a><a name="p13755817443"></a>0：函数被禁用。</p>
<p id="p1411826144918"><a name="p1411826144918"></a><a name="p1411826144918"></a>-1：函数被启用。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  func\_vpc参数说明

<a name="table11522131317013"></a>
<table><thead align="left"><tr id="row5523191315016"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p9548942414"><a name="p9548942414"></a><a name="p9548942414"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="p1354814421111"><a name="p1354814421111"></a><a name="p1354814421111"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="p35481142416"><a name="p35481142416"></a><a name="p35481142416"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="p145488421311"><a name="p145488421311"></a><a name="p145488421311"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row115231137012"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p1754818422012"><a name="p1754818422012"></a><a name="p1754818422012"></a>vpc_name</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p1249815123165"><a name="p1249815123165"></a><a name="p1249815123165"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p1254814218116"><a name="p1254814218116"></a><a name="p1254814218116"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p9548542519"><a name="p9548542519"></a><a name="p9548542519"></a>虚拟私有云名称</p>
</td>
</tr>
<tr id="row10523181319015"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p1054814213111"><a name="p1054814213111"></a><a name="p1054814213111"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p169617140160"><a name="p169617140160"></a><a name="p169617140160"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p11548104211113"><a name="p11548104211113"></a><a name="p11548104211113"></a>当func_vpc非空时必选</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p65482422118"><a name="p65482422118"></a><a name="p65482422118"></a>虚拟私有云唯一标识</p>
</td>
</tr>
<tr id="row1852311320018"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p135483421012"><a name="p135483421012"></a><a name="p135483421012"></a>subnet_name</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p174097168169"><a name="p174097168169"></a><a name="p174097168169"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p7548142516"><a name="p7548142516"></a><a name="p7548142516"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p1054820424111"><a name="p1054820424111"></a><a name="p1054820424111"></a>子网名称</p>
</td>
</tr>
<tr id="row18523613406"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p35484421318"><a name="p35484421318"></a><a name="p35484421318"></a>subnet_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p17548242813"><a name="p17548242813"></a><a name="p17548242813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p68278307116"><a name="p68278307116"></a><a name="p68278307116"></a>当func_vpc非空时必选</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p1654817421817"><a name="p1654817421817"></a><a name="p1654817421817"></a>子网编号</p>
</td>
</tr>
<tr id="row452391317018"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p16548194217113"><a name="p16548194217113"></a><a name="p16548194217113"></a>cidr</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p1854824210114"><a name="p1854824210114"></a><a name="p1854824210114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p125491424111"><a name="p125491424111"></a><a name="p125491424111"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p754917421019"><a name="p754917421019"></a><a name="p754917421019"></a>子网掩码</p>
</td>
</tr>
<tr id="row175236131507"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p115492042813"><a name="p115492042813"></a><a name="p115492042813"></a>gateway</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p16753722101611"><a name="p16753722101611"></a><a name="p16753722101611"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p9549184215114"><a name="p9549184215114"></a><a name="p9549184215114"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p3549194218111"><a name="p3549194218111"></a><a name="p3549194218111"></a>网关</p>
</td>
</tr>
</tbody>
</table>

**表 5**  dependency参数说明

<a name="table3788232112820"></a>
<table><thead align="left"><tr id="row117885323287"><th class="cellrowborder" valign="top" width="23.28%" id="mcps1.2.5.1.1"><p id="p117889326283"><a name="p117889326283"></a><a name="p117889326283"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="27.529999999999998%" id="mcps1.2.5.1.2"><p id="p6788103216282"><a name="p6788103216282"></a><a name="p6788103216282"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="24.19%" id="mcps1.2.5.1.3"><p id="p14788203282816"><a name="p14788203282816"></a><a name="p14788203282816"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="p778820321285"><a name="p778820321285"></a><a name="p778820321285"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row16789193220285"><td class="cellrowborder" valign="top" width="23.28%" headers="mcps1.2.5.1.1 "><p id="p37898326288"><a name="p37898326288"></a><a name="p37898326288"></a>owner</p>
</td>
<td class="cellrowborder" valign="top" width="27.529999999999998%" headers="mcps1.2.5.1.2 "><p id="p578916322288"><a name="p578916322288"></a><a name="p578916322288"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="24.19%" headers="mcps1.2.5.1.3 "><p id="p478913211287"><a name="p478913211287"></a><a name="p478913211287"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p850405873011"><a name="p850405873011"></a><a name="p850405873011"></a>依赖包属主的domainId</p>
</td>
</tr>
<tr id="row37893325281"><td class="cellrowborder" valign="top" width="23.28%" headers="mcps1.2.5.1.1 "><p id="p1478913272815"><a name="p1478913272815"></a><a name="p1478913272815"></a>link</p>
</td>
<td class="cellrowborder" valign="top" width="27.529999999999998%" headers="mcps1.2.5.1.2 "><p id="p117891932132818"><a name="p117891932132818"></a><a name="p117891932132818"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="24.19%" headers="mcps1.2.5.1.3 "><p id="p12789132132817"><a name="p12789132132817"></a><a name="p12789132132817"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p4789153252814"><a name="p4789153252814"></a><a name="p4789153252814"></a>依赖包在OBS上的链接</p>
</td>
</tr>
<tr id="row47874148290"><td class="cellrowborder" valign="top" width="23.28%" headers="mcps1.2.5.1.1 "><p id="p6788171432920"><a name="p6788171432920"></a><a name="p6788171432920"></a>runtime</p>
</td>
<td class="cellrowborder" valign="top" width="27.529999999999998%" headers="mcps1.2.5.1.2 "><p id="p87501514309"><a name="p87501514309"></a><a name="p87501514309"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="24.19%" headers="mcps1.2.5.1.3 "><p id="p147881114162910"><a name="p147881114162910"></a><a name="p147881114162910"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p187885149295"><a name="p187885149295"></a><a name="p187885149295"></a>依赖包语言类型（仅作为分类条件）</p>
</td>
</tr>
<tr id="row197121711297"><td class="cellrowborder" valign="top" width="23.28%" headers="mcps1.2.5.1.1 "><p id="p1571117182911"><a name="p1571117182911"></a><a name="p1571117182911"></a>etag</p>
</td>
<td class="cellrowborder" valign="top" width="27.529999999999998%" headers="mcps1.2.5.1.2 "><p id="p27151752916"><a name="p27151752916"></a><a name="p27151752916"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="24.19%" headers="mcps1.2.5.1.3 "><p id="p5712176293"><a name="p5712176293"></a><a name="p5712176293"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p197191712290"><a name="p197191712290"></a><a name="p197191712290"></a>依赖包md5值</p>
</td>
</tr>
<tr id="row18364319122919"><td class="cellrowborder" valign="top" width="23.28%" headers="mcps1.2.5.1.1 "><p id="p2036441917298"><a name="p2036441917298"></a><a name="p2036441917298"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="27.529999999999998%" headers="mcps1.2.5.1.2 "><p id="p1836421922917"><a name="p1836421922917"></a><a name="p1836421922917"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="24.19%" headers="mcps1.2.5.1.3 "><p id="p4364101916297"><a name="p4364101916297"></a><a name="p4364101916297"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p136410194294"><a name="p136410194294"></a><a name="p136410194294"></a>依赖包大小</p>
</td>
</tr>
<tr id="row35521534152912"><td class="cellrowborder" valign="top" width="23.28%" headers="mcps1.2.5.1.1 "><p id="p12552103420291"><a name="p12552103420291"></a><a name="p12552103420291"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="27.529999999999998%" headers="mcps1.2.5.1.2 "><p id="p455213482912"><a name="p455213482912"></a><a name="p455213482912"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="24.19%" headers="mcps1.2.5.1.3 "><p id="p955363442915"><a name="p955363442915"></a><a name="p955363442915"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p5553143417296"><a name="p5553143417296"></a><a name="p5553143417296"></a>依赖包名称</p>
</td>
</tr>
<tr id="row17984153672917"><td class="cellrowborder" valign="top" width="23.28%" headers="mcps1.2.5.1.1 "><p id="p199844365296"><a name="p199844365296"></a><a name="p199844365296"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="27.529999999999998%" headers="mcps1.2.5.1.2 "><p id="p19841836132920"><a name="p19841836132920"></a><a name="p19841836132920"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="24.19%" headers="mcps1.2.5.1.3 "><p id="p1984133682911"><a name="p1984133682911"></a><a name="p1984133682911"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p2984113613295"><a name="p2984113613295"></a><a name="p2984113613295"></a>依赖包描述</p>
</td>
</tr>
<tr id="row96981850182917"><td class="cellrowborder" valign="top" width="23.28%" headers="mcps1.2.5.1.1 "><p id="p166987503294"><a name="p166987503294"></a><a name="p166987503294"></a>file_name</p>
</td>
<td class="cellrowborder" valign="top" width="27.529999999999998%" headers="mcps1.2.5.1.2 "><p id="p1769815042913"><a name="p1769815042913"></a><a name="p1769815042913"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="24.19%" headers="mcps1.2.5.1.3 "><p id="p069875072920"><a name="p069875072920"></a><a name="p069875072920"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p1069895017294"><a name="p1069895017294"></a><a name="p1069895017294"></a>依赖包文件名（如果创建方式为zip时）</p>
</td>
</tr>
</tbody>
</table>

**表 6**  mount\_config参数说明

<a name="table2317745151313"></a>
<table><thead align="left"><tr id="row11317184561317"><th class="cellrowborder" valign="top" width="23.28%" id="mcps1.2.5.1.1"><p id="p173171445191314"><a name="p173171445191314"></a><a name="p173171445191314"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="27.529999999999998%" id="mcps1.2.5.1.2"><p id="p8317154531311"><a name="p8317154531311"></a><a name="p8317154531311"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="24.19%" id="mcps1.2.5.1.3"><p id="p2317114551314"><a name="p2317114551314"></a><a name="p2317114551314"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="p1231774516132"><a name="p1231774516132"></a><a name="p1231774516132"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row8317194511138"><td class="cellrowborder" valign="top" width="23.28%" headers="mcps1.2.5.1.1 "><p id="p19317194541316"><a name="p19317194541316"></a><a name="p19317194541316"></a>mount_user</p>
</td>
<td class="cellrowborder" valign="top" width="27.529999999999998%" headers="mcps1.2.5.1.2 "><p id="p1031811451135"><a name="p1031811451135"></a><a name="p1031811451135"></a>mount_user(参考表 mount_user说明)</p>
</td>
<td class="cellrowborder" valign="top" width="24.19%" headers="mcps1.2.5.1.3 "><p id="p136301821614"><a name="p136301821614"></a><a name="p136301821614"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p1231894512136"><a name="p1231894512136"></a><a name="p1231894512136"></a>文件系统用户配置</p>
</td>
</tr>
<tr id="row19318154511310"><td class="cellrowborder" valign="top" width="23.28%" headers="mcps1.2.5.1.1 "><p id="p20318104517137"><a name="p20318104517137"></a><a name="p20318104517137"></a>func_mounts</p>
</td>
<td class="cellrowborder" valign="top" width="27.529999999999998%" headers="mcps1.2.5.1.2 "><p id="p231814520130"><a name="p231814520130"></a><a name="p231814520130"></a>func_mount（参考表 func_mount说明）</p>
</td>
<td class="cellrowborder" valign="top" width="24.19%" headers="mcps1.2.5.1.3 "><p id="p16318145191311"><a name="p16318145191311"></a><a name="p16318145191311"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p63181458137"><a name="p63181458137"></a><a name="p63181458137"></a>文件系统列表</p>
</td>
</tr>
</tbody>
</table>

**表 7**  mount\_user说明

<a name="table14797155061717"></a>
<table><thead align="left"><tr id="row18797105015171"><th class="cellrowborder" valign="top" width="23.28%" id="mcps1.2.5.1.1"><p id="p117975502173"><a name="p117975502173"></a><a name="p117975502173"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="27.529999999999998%" id="mcps1.2.5.1.2"><p id="p11798185091712"><a name="p11798185091712"></a><a name="p11798185091712"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="24.19%" id="mcps1.2.5.1.3"><p id="p679816501174"><a name="p679816501174"></a><a name="p679816501174"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="p9798175014177"><a name="p9798175014177"></a><a name="p9798175014177"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1279885031713"><td class="cellrowborder" valign="top" width="23.28%" headers="mcps1.2.5.1.1 "><p id="p1479815014174"><a name="p1479815014174"></a><a name="p1479815014174"></a>user_id</p>
</td>
<td class="cellrowborder" valign="top" width="27.529999999999998%" headers="mcps1.2.5.1.2 "><p id="p77981450131716"><a name="p77981450131716"></a><a name="p77981450131716"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="24.19%" headers="mcps1.2.5.1.3 "><p id="p1179865041715"><a name="p1179865041715"></a><a name="p1179865041715"></a>mount_user非空时必选</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p17798175015173"><a name="p17798175015173"></a><a name="p17798175015173"></a>用户ID(-1~65534的非0整数)</p>
</td>
</tr>
<tr id="row2079885011715"><td class="cellrowborder" valign="top" width="23.28%" headers="mcps1.2.5.1.1 "><p id="p079865019179"><a name="p079865019179"></a><a name="p079865019179"></a>user_group_id</p>
</td>
<td class="cellrowborder" valign="top" width="27.529999999999998%" headers="mcps1.2.5.1.2 "><p id="p17999500172"><a name="p17999500172"></a><a name="p17999500172"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="24.19%" headers="mcps1.2.5.1.3 "><p id="p11799750101714"><a name="p11799750101714"></a><a name="p11799750101714"></a>mount_user非空时必选</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p17755154919198"><a name="p17755154919198"></a><a name="p17755154919198"></a>用户组ID(-1~65534的非0整数)</p>
</td>
</tr>
</tbody>
</table>

**表 8**  func\_mount说明

<a name="table1937492111205"></a>
<table><thead align="left"><tr id="row6375142122013"><th class="cellrowborder" valign="top" width="23.28%" id="mcps1.2.5.1.1"><p id="p137518219203"><a name="p137518219203"></a><a name="p137518219203"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="27.529999999999998%" id="mcps1.2.5.1.2"><p id="p5375021172017"><a name="p5375021172017"></a><a name="p5375021172017"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="22.759999999999998%" id="mcps1.2.5.1.3"><p id="p1375121102012"><a name="p1375121102012"></a><a name="p1375121102012"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="26.43%" id="mcps1.2.5.1.4"><p id="p33751521122014"><a name="p33751521122014"></a><a name="p33751521122014"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row437522115208"><td class="cellrowborder" valign="top" width="23.28%" headers="mcps1.2.5.1.1 "><p id="p17375162118203"><a name="p17375162118203"></a><a name="p17375162118203"></a>mount_type</p>
</td>
<td class="cellrowborder" valign="top" width="27.529999999999998%" headers="mcps1.2.5.1.2 "><p id="p14375521122017"><a name="p14375521122017"></a><a name="p14375521122017"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="22.759999999999998%" headers="mcps1.2.5.1.3 "><p id="p1460462206"><a name="p1460462206"></a><a name="p1460462206"></a>func_mounts非空时必选</p>
</td>
<td class="cellrowborder" valign="top" width="26.43%" headers="mcps1.2.5.1.4 "><p id="p9509123292117"><a name="p9509123292117"></a><a name="p9509123292117"></a>挂载类型(sfs/sfsTurbo/ecs)</p>
</td>
</tr>
<tr id="row1837510211209"><td class="cellrowborder" valign="top" width="23.28%" headers="mcps1.2.5.1.1 "><p id="p037515213203"><a name="p037515213203"></a><a name="p037515213203"></a>mount_resource</p>
</td>
<td class="cellrowborder" valign="top" width="27.529999999999998%" headers="mcps1.2.5.1.2 "><p id="p1837592113204"><a name="p1837592113204"></a><a name="p1837592113204"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="22.759999999999998%" headers="mcps1.2.5.1.3 "><p id="p1455077142112"><a name="p1455077142112"></a><a name="p1455077142112"></a>func_mounts非空时必选</p>
</td>
<td class="cellrowborder" valign="top" width="26.43%" headers="mcps1.2.5.1.4 "><p id="p1251531812234"><a name="p1251531812234"></a><a name="p1251531812234"></a>挂载资源ID（对应云服务ID）</p>
</td>
</tr>
<tr id="row06073533239"><td class="cellrowborder" valign="top" width="23.28%" headers="mcps1.2.5.1.1 "><p id="p1608185313233"><a name="p1608185313233"></a><a name="p1608185313233"></a>mount_share_path</p>
</td>
<td class="cellrowborder" valign="top" width="27.529999999999998%" headers="mcps1.2.5.1.2 "><p id="p1460975311237"><a name="p1460975311237"></a><a name="p1460975311237"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="22.759999999999998%" headers="mcps1.2.5.1.3 "><p id="p172329172419"><a name="p172329172419"></a><a name="p172329172419"></a>如果mount_type为ecs，必选</p>
</td>
<td class="cellrowborder" valign="top" width="26.43%" headers="mcps1.2.5.1.4 "><p id="p3609185372312"><a name="p3609185372312"></a><a name="p3609185372312"></a>远端挂载路径（例如192.168.0.12:/data）</p>
</td>
</tr>
<tr id="row212845722318"><td class="cellrowborder" valign="top" width="23.28%" headers="mcps1.2.5.1.1 "><p id="p201298572237"><a name="p201298572237"></a><a name="p201298572237"></a>local_mount_path</p>
</td>
<td class="cellrowborder" valign="top" width="27.529999999999998%" headers="mcps1.2.5.1.2 "><p id="p1612918578236"><a name="p1612918578236"></a><a name="p1612918578236"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="22.759999999999998%" headers="mcps1.2.5.1.3 "><p id="p16129195716239"><a name="p16129195716239"></a><a name="p16129195716239"></a>func_mounts非空时必选</p>
</td>
<td class="cellrowborder" valign="top" width="26.43%" headers="mcps1.2.5.1.4 "><p id="p5129757132313"><a name="p5129757132313"></a><a name="p5129757132313"></a>函数访问路径</p>
</td>
</tr>
</tbody>
</table>

funcurn格式如下。

```
urn:fss:<region_id>:<project_id>:function:<package>:<function_name>[:<version>|:!<alias>]
```

>![](public_sys-resources/icon-note.gif) **说明：**   
>FuncUrn使用冒号分隔为8个域，region\_id为系统配置的值（测试时可以填成与后台相同的值），最后一个中括号的内容表示可以为函数的版本号，也可以为该版本指向的别名，如果为别名时需要在名称前加上感叹号！以示区分。  

当作为API参数时，可以提供简化格式的FuncUrn，具体如下。

-   提供1个域：解析为<function\_name\>，project\_id从token中获取，package为default，version为latest。
-   提供2个域：解析为<package\>:<function\_name\>，project\_id从token中获取，version为latest。
-   提供3个域：解析为<project\_id\>:<package\>:<function\_name\>，version为latest。
-   提供4个域：解析为<project\_id\>:<package\>:<function\_name\>:<Version or Alias\>。
-   提供7个域：解析为urn:fss:<region\_id\>:<project\_id\>:function:<package\>:<function\_name\>，Version为latest。
-   提供8个域：解析为urn:fss:<region\_id\>:<project\_id\>:function:<package\>:<function\_name\>:<Version or Alias\>。

