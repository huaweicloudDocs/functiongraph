# 获取函数的metadata<a name="functiongraph_06_0106"></a>

## 功能介绍<a name="section21363070"></a>

获取指定函数的metadata。

## URI<a name="section58049908"></a>

URL：/v2/\{project\_id\}/fgs/functions/\{function\_urn\}/config

Method：GET

参数说明如[表1](#d0e2233)所示。

**表 1**  参数说明

<a name="d0e2233"></a>
<table><thead align="left"><tr id="row35226659"><th class="cellrowborder" valign="top" width="17.52824717528247%" id="mcps1.2.5.1.1"><p id="p34787141"><a name="p34787141"></a><a name="p34787141"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="12.368763123687629%" id="mcps1.2.5.1.2"><p id="p66295060"><a name="p66295060"></a><a name="p66295060"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="17.52824717528247%" id="mcps1.2.5.1.3"><p id="p1190775"><a name="p1190775"></a><a name="p1190775"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="52.57474252574742%" id="mcps1.2.5.1.4"><p id="p29343959"><a name="p29343959"></a><a name="p29343959"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row28050459"><td class="cellrowborder" valign="top" width="17.52824717528247%" headers="mcps1.2.5.1.1 "><p id="p57494700"><a name="p57494700"></a><a name="p57494700"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.368763123687629%" headers="mcps1.2.5.1.2 "><p id="p26559089"><a name="p26559089"></a><a name="p26559089"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="17.52824717528247%" headers="mcps1.2.5.1.3 "><p id="p3802578"><a name="p3802578"></a><a name="p3802578"></a>必选</p>
</td>
<td class="cellrowborder" valign="top" width="52.57474252574742%" headers="mcps1.2.5.1.4 "><p id="p39573433"><a name="p39573433"></a><a name="p39573433"></a>Project Id。</p>
</td>
</tr>
<tr id="row20616577"><td class="cellrowborder" valign="top" width="17.52824717528247%" headers="mcps1.2.5.1.1 "><p id="p59330025"><a name="p59330025"></a><a name="p59330025"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="12.368763123687629%" headers="mcps1.2.5.1.2 "><p id="p41002697"><a name="p41002697"></a><a name="p41002697"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="17.52824717528247%" headers="mcps1.2.5.1.3 "><p id="p32884170"><a name="p32884170"></a><a name="p32884170"></a>必选</p>
</td>
<td class="cellrowborder" valign="top" width="52.57474252574742%" headers="mcps1.2.5.1.4 "><p id="p46372115"><a name="p46372115"></a><a name="p46372115"></a>函数的URN，详细解释见<a href="FunctionGraph函数模型.md">FunctionGraph函数模型</a>的描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section52687132"></a>

**请求参数**

无

**请求示例**

```
GET /v2/7aad83af3e8d42e99ac194e8419e2c9b/fgs/functions/urn:fss:cn-north-1:7aad83af3e8d42e99ac194e8419e2c9b:function:default:test:latest/config HTTP/1.1
```

## 响应消息<a name="section4422141"></a>

**响应参数**

响应参数如[表2](#table394445163918)所示。    

**表 2**  响应参数

<a name="table394445163918"></a>
<table><thead align="left"><tr id="row5944851163912"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.4.1.1"><p id="p7944165193912"><a name="p7944165193912"></a><a name="p7944165193912"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.112511251125113%" id="mcps1.2.4.1.2"><p id="p494413519391"><a name="p494413519391"></a><a name="p494413519391"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.68546854685468%" id="mcps1.2.4.1.3"><p id="p159441351193918"><a name="p159441351193918"></a><a name="p159441351193918"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row898316393534"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p15613952165015"><a name="p15613952165015"></a><a name="p15613952165015"></a>func_urn</p>
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
<tr id="row18461113155312"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p6342113115111"><a name="p6342113115111"></a><a name="p6342113115111"></a>user_domain</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p02891635145919"><a name="p02891635145919"></a><a name="p02891635145919"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p23860166"><a name="p23860166"></a><a name="p23860166"></a>租户名称。</p>
</td>
</tr>
<tr id="row12325311185316"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p15177124215115"><a name="p15177124215115"></a><a name="p15177124215115"></a>namespace</p>
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
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p1037073510592"><a name="p1037073510592"></a><a name="p1037073510592"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p2861285"><a name="p2861285"></a><a name="p2861285"></a>函数占用的cpu资源，单位为millicore（1 core=1000 millicores），取值与MemorySize成比例，默认是128M内存占0.1个核（100 millicores），函数占用的CPU为基础CPU：200 millicores，再加上内存按比例占用的CPU，计算方法：内存/128 *100 + 200。</p>
</td>
</tr>
<tr id="row618615514526"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p151601843195211"><a name="p151601843195211"></a><a name="p151601843195211"></a>code_type</p>
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
<tr id="row1854324825113"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p20276110185319"><a name="p20276110185319"></a><a name="p20276110185319"></a>code_url</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p38271640155912"><a name="p38271640155912"></a><a name="p38271640155912"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p39078787"><a name="p39078787"></a><a name="p39078787"></a>当CodeType为obs时，该值为函数代码包在OBS上的地址，CodeType为其他值时，该字段为空。</p>
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
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p4850114010594"><a name="p4850114010594"></a><a name="p4850114010594"></a>int64</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p22507915"><a name="p22507915"></a><a name="p22507915"></a>函数大小，单位：字节。</p>
</td>
</tr>
<tr id="row112081421205117"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p9832816195415"><a name="p9832816195415"></a><a name="p9832816195415"></a>user_data</p>
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
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p8925154095912"><a name="p8925154095912"></a><a name="p8925154095912"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p215783891315"><a name="p215783891315"></a><a name="p215783891315"></a>函数app使用的权限委托名称，需要IAM支持，并在IAM界面创建委托，当函数需要访问其他服务时，必须提供该字段。</p>
</td>
</tr>
<tr id="row1937154145711"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p1947817508576"><a name="p1947817508576"></a><a name="p1947817508576"></a>dependency_pkg</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p13478750125716"><a name="p13478750125716"></a><a name="p13478750125716"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p129371741195717"><a name="p129371741195717"></a><a name="p129371741195717"></a>函数依赖的第三方软件zip包在obs上的地址，多个第三方软件要打包到一个zip文件中，如果未使用第三方软件。</p>
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
<tr id="row19286204517"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p16975145355517"><a name="p16975145355517"></a><a name="p16975145355517"></a>last_modified</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p20110547185915"><a name="p20110547185915"></a><a name="p20110547185915"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p45259754"><a name="p45259754"></a><a name="p45259754"></a>函数最后一次更新时间。</p>
</td>
</tr>
<tr id="row188192822711"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p78812287273"><a name="p78812287273"></a><a name="p78812287273"></a>depend_list</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p18881162882714"><a name="p18881162882714"></a><a name="p18881162882714"></a>[]string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p18881182842710"><a name="p18881182842710"></a><a name="p18881182842710"></a>依赖包列表</p>
</td>
</tr>
<tr id="row1732519315277"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p163252312270"><a name="p163252312270"></a><a name="p163252312270"></a>strategy_config</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p1832518315276"><a name="p1832518315276"></a><a name="p1832518315276"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p18325531142712"><a name="p18325531142712"></a><a name="p18325531142712"></a>函数策略配置，请参考<a href="#table4775818446">表3</a>。</p>
</td>
</tr>
<tr id="row225127192"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p56491446899"><a name="p56491446899"></a><a name="p56491446899"></a>extend_config</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p166491461591"><a name="p166491461591"></a><a name="p166491461591"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p664918461915"><a name="p664918461915"></a><a name="p664918461915"></a>函数扩展配置</p>
</td>
</tr>
<tr id="row636641018914"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p564910461791"><a name="p564910461791"></a><a name="p564910461791"></a>initializer_handler</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p564916463910"><a name="p564916463910"></a><a name="p564916463910"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p46491246490"><a name="p46491246490"></a><a name="p46491246490"></a>函数初始化入口，规则：xx.xx，必须包含“. ”，举例：对于node.js函数：myfunction.initializer，则表示函数的文件名为myfunction.js，初始化的入口函数名为initializer</p>
</td>
</tr>
<tr id="row18983171213911"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p16649144612911"><a name="p16649144612911"></a><a name="p16649144612911"></a>initializer_timeout</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p146491446791"><a name="p146491446791"></a><a name="p146491446791"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p1564917467913"><a name="p1564917467913"></a><a name="p1564917467913"></a>初始化超时时间，超时函数将被强行停止，范围1～300秒</p>
</td>
</tr>
<tr id="row145286151296"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p1264914461694"><a name="p1264914461694"></a><a name="p1264914461694"></a>func_vpc</p>
</td>
<td class="cellrowborder" valign="top" width="25.112511251125113%" headers="mcps1.2.4.1.2 "><p id="p1564919465910"><a name="p1564919465910"></a><a name="p1564919465910"></a>*string</p>
</td>
<td class="cellrowborder" valign="top" width="54.68546854685468%" headers="mcps1.2.4.1.3 "><p id="p11649846890"><a name="p11649846890"></a><a name="p11649846890"></a>vpc配置，请参考<a href="获取函数列表.md#table11522131317013">表6 func_vpc参数说明</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  strategy\_config参数说明

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
<tbody><tr id="row47195819446"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.1 "><p id="p17775834410"><a name="p17775834410"></a><a name="p17775834410"></a>concurrency</p>
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

**响应示例**

成功时的返回格式：

```
HTTP/1.1 200 OK 
{ 
  "code_filename": "index.js", 
  "code_size": 272, 
  "code_type": "inline", 
  "code_url": "", 
  "cpu": 300, 
  "dependency_pkg": "", 
  "description": "111", 
  "digest": "decbce6939297b0b5ec6d1a23bf9c725870f5e69fc338a89a6a4029264688dc26338f56d08b6535de47f15ad538e22ca66613b9a46f807d50b687bb53fded1c6", 
  "func_name": "test", 
  "func_urn": "urn:fss:cn-north-1:7aad83af3e8d42e99ac194e8419e2c9b:function:default:test:latest", 
  "handler": "test.handler", 
  "image_name": "latest-5qe8e", 
  "last_modified": "2018-03-28T11:30:32+08:00", 
  "memory_size": 128, 
  "namespace": "7aad83af3e8d42e99ac194e8419e2c9b", 
  "package": "default", 
  "project_name": "cn-north-1", 
  "runtime": "Node.js6.10", 
  "timeout": 3, 
  "user_data": "", 
  "user_domain": "cff01_hk", 
  "version": "latest", 
  "version_description": "", 
  "xrole": "cff",
  "app_xrole": "",
  "concurrency": 0,
  "depend_list": null,
  "strategy_config": {
      "concurrency": -1
  },
  "extend_config": "",
  "dependencies": []
  "initializer_handler": "",
   "initializer_timeout": 0,
    "func_vpc": null
 }
```

```
失败时的返回格式（示例）：
```

```
HTTP/1.1 404 Not Found 
{ 
  "error_code": "FSS.1051", 
  "error_msg": "Not found the function" 
 }
```

## 状态码<a name="section39799274"></a>

状态码说明如[表4](#d0e2312)所示。

**表 4**  状态码说明

<a name="d0e2312"></a>
<table><thead align="left"><tr id="row58182238"><th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.3.1.1"><p id="p15140815"><a name="p15140815"></a><a name="p15140815"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="86.87%" id="mcps1.2.3.1.2"><p id="p18446534"><a name="p18446534"></a><a name="p18446534"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row17774248"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p30427999"><a name="p30427999"></a><a name="p30427999"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p48748883"><a name="p48748883"></a><a name="p48748883"></a>InvalidParameterValueException：输入参数错误。</p>
</td>
</tr>
<tr id="row36086767"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p37347016"><a name="p37347016"></a><a name="p37347016"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p5209490"><a name="p5209490"></a><a name="p5209490"></a>UnauthorizedAccess：未授权的访问。</p>
</td>
</tr>
<tr id="row179461988382"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p1694613843812"><a name="p1694613843812"></a><a name="p1694613843812"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p1394612883820"><a name="p1394612883820"></a><a name="p1394612883820"></a>Forbidden：禁止访问。</p>
</td>
</tr>
<tr id="row46885417"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p39622431"><a name="p39622431"></a><a name="p39622431"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p55300313"><a name="p55300313"></a><a name="p55300313"></a>ResourceNotFoundException：函数没有找到。</p>
</td>
</tr>
<tr id="row27940771"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p48609983"><a name="p48609983"></a><a name="p48609983"></a>429</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p45094547"><a name="p45094547"></a><a name="p45094547"></a>TooManyRequestsException：并发请求数太多。</p>
</td>
</tr>
<tr id="row3197746"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p57690894"><a name="p57690894"></a><a name="p57690894"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p42450871"><a name="p42450871"></a><a name="p42450871"></a>InternalServerError：服务内部出错。</p>
</td>
</tr>
</tbody>
</table>

