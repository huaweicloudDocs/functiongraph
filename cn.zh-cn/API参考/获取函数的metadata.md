# 获取函数的metadata<a name="ZH-CN_TOPIC_0115410481"></a>

## 功能介绍<a name="section21363070"></a>

获取指定函数的metadata。

## URI<a name="section58049908"></a>

GET /v2/\{project\_id\}/fgs/functions/\{function\_urn\}/config

URI参数说明如[表1](#d0e2233)所示。

**表 1**  URI参数说明

<a name="d0e2233"></a>
<table><thead align="left"><tr id="row35226659"><th class="cellrowborder" valign="top" width="15%" id="mcps1.2.5.1.1"><p id="p34787141"><a name="p34787141"></a><a name="p34787141"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.2"><p id="p66295060"><a name="p66295060"></a><a name="p66295060"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.3"><p id="p1190775"><a name="p1190775"></a><a name="p1190775"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="65%" id="mcps1.2.5.1.4"><p id="p29343959"><a name="p29343959"></a><a name="p29343959"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row28050459"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.1 "><p id="p57494700"><a name="p57494700"></a><a name="p57494700"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p26559089"><a name="p26559089"></a><a name="p26559089"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.3 "><p id="p3802578"><a name="p3802578"></a><a name="p3802578"></a>必选</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.5.1.4 "><p id="p39573433"><a name="p39573433"></a><a name="p39573433"></a>Project ID。</p>
</td>
</tr>
<tr id="row20616577"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.1 "><p id="p59330025"><a name="p59330025"></a><a name="p59330025"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p41002697"><a name="p41002697"></a><a name="p41002697"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.3 "><p id="p32884170"><a name="p32884170"></a><a name="p32884170"></a>必选</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.5.1.4 "><p id="p46372115"><a name="p46372115"></a><a name="p46372115"></a>函数的URN，详细解释见<a href="FunctionGraph函数模型.md">FunctionGraph函数模型</a>的描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section52687132"></a>

无

## 响应消息<a name="section4422141"></a>

响应参数说明如[表2](#table394445163918)所示。    

**表 2**  响应参数说明

<a name="table394445163918"></a>
<table><thead align="left"><tr id="row5944851163912"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p7944165193912"><a name="p7944165193912"></a><a name="p7944165193912"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.4.1.2"><p id="p494413519391"><a name="p494413519391"></a><a name="p494413519391"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="65%" id="mcps1.2.4.1.3"><p id="p159441351193918"><a name="p159441351193918"></a><a name="p159441351193918"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row898316393534"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15613952165015"><a name="p15613952165015"></a><a name="p15613952165015"></a>func_urn</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p159832399530"><a name="p159832399530"></a><a name="p159832399530"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p63770254"><a name="p63770254"></a><a name="p63770254"></a>函数的URN（Uniform Resource Name），唯一标识函数。</p>
</td>
</tr>
<tr id="row42001372535"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p49181313"><a name="p49181313"></a><a name="p49181313"></a>func_name</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p5201173725318"><a name="p5201173725318"></a><a name="p5201173725318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p24263425"><a name="p24263425"></a><a name="p24263425"></a>函数名称。</p>
</td>
</tr>
<tr id="row18461113155312"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p38405776"><a name="p38405776"></a><a name="p38405776"></a>domain_id</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p02891635145919"><a name="p02891635145919"></a><a name="p02891635145919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p23860166"><a name="p23860166"></a><a name="p23860166"></a>域名id。</p>
</td>
</tr>
<tr id="row12325311185316"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15177124215115"><a name="p15177124215115"></a><a name="p15177124215115"></a>namespace</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p830113515915"><a name="p830113515915"></a><a name="p830113515915"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p35485571"><a name="p35485571"></a><a name="p35485571"></a>租户的Project ID。</p>
</td>
</tr>
<tr id="row42345816531"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p32068643"><a name="p32068643"></a><a name="p32068643"></a>project_name</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p73101735165919"><a name="p73101735165919"></a><a name="p73101735165919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p47423267"><a name="p47423267"></a><a name="p47423267"></a>租户的Project Name。</p>
</td>
</tr>
<tr id="row71958611537"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p10497128"><a name="p10497128"></a><a name="p10497128"></a>package</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p10319103585917"><a name="p10319103585917"></a><a name="p10319103585917"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p44961053"><a name="p44961053"></a><a name="p44961053"></a>函数所属的分组Package，用于用户针对函数的自定义分组。</p>
</td>
</tr>
<tr id="row1121313416531"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p27482234"><a name="p27482234"></a><a name="p27482234"></a>runtime</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p143291358595"><a name="p143291358595"></a><a name="p143291358595"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p652094462816"><a name="p652094462816"></a><a name="p652094462816"></a>FunctionGraph函数的执行环境，支持Node.js 6.10、Node.js 8.10、Node.js 10.16、Node.js 12.13、Python 2.7、Python 3.6、Java 8、Go 1.8、C#.NET Core 2.0、C#.NET Core 2.1、C#.NET Core 3.1和PHP 7.3。</p>
</td>
</tr>
<tr id="row16165192105318"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p39009036"><a name="p39009036"></a><a name="p39009036"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p9339035135910"><a name="p9339035135910"></a><a name="p9339035135910"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p5615384"><a name="p5615384"></a><a name="p5615384"></a>函数执行超时时间，超时函数将被强行停止，范围3 ～ 900秒。</p>
</td>
</tr>
<tr id="row12238205710522"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p67083165"><a name="p67083165"></a><a name="p67083165"></a>handler</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p535063516598"><a name="p535063516598"></a><a name="p535063516598"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p1345215815308"><a name="p1345215815308"></a><a name="p1345215815308"></a>函数执行入口，规则：xx.xx，必须包含“. ”。</p>
<p id="p65027307"><a name="p65027307"></a><a name="p65027307"></a>举例：对于Node.js函数：myfunction.handler，则表示函数的文件名为myfunction.js，执行的入口函数名为handler。</p>
</td>
</tr>
<tr id="row1229205512521"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p26048945"><a name="p26048945"></a><a name="p26048945"></a>memory_size</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p6360153545914"><a name="p6360153545914"></a><a name="p6360153545914"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p18996171473110"><a name="p18996171473110"></a><a name="p18996171473110"></a>函数消耗的内存，单位M。</p>
<p id="p29589819"><a name="p29589819"></a><a name="p29589819"></a>取值范围为：128、256、512、768、1024、1280、1536、1792、2048、2560、3072、3584、4096。最小值为128，最大值为4096。</p>
</td>
</tr>
<tr id="row192981153205213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p29032981"><a name="p29032981"></a><a name="p29032981"></a>cpu</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p1037073510592"><a name="p1037073510592"></a><a name="p1037073510592"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p730228163117"><a name="p730228163117"></a><a name="p730228163117"></a>函数占用的CPU资源，单位为millicore（1 core=1000 millicores）。</p>
<p id="p2861285"><a name="p2861285"></a><a name="p2861285"></a>取值与MemorySize成比例，默认是128M内存占0.1个核（100 millicores），函数占用的CPU为基础CPU：200 millicores，再加上内存按比例占用的CPU，计算方法：内存/128 *100 + 200。</p>
</td>
</tr>
<tr id="row618615514526"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p151601843195211"><a name="p151601843195211"></a><a name="p151601843195211"></a>code_type</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p1738033513599"><a name="p1738033513599"></a><a name="p1738033513599"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p43048911"><a name="p43048911"></a><a name="p43048911"></a>函数代码类型，取值有4种：</p>
<a name="ul113261839123118"></a><a name="ul113261839123118"></a><ul id="ul113261839123118"><li>inline：UI在线编辑代码</li><li>zip：函数代码为zip包</li><li>jar：函数代码为jar包，主要针对Java函数</li><li>obs：函数代码来源于OBS存储</li></ul>
</td>
</tr>
<tr id="row1854324825113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p20276110185319"><a name="p20276110185319"></a><a name="p20276110185319"></a>code_url</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p38271640155912"><a name="p38271640155912"></a><a name="p38271640155912"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><a name="ul1515514761216"></a><a name="ul1515514761216"></a><ul id="ul1515514761216"><li>当“code_type”为“obs”时，该值为函数代码包在OBS上的地址。</li><li>当“code_type”为“inline”、“zip”或“jar”时，该字段为空。</li></ul>
</td>
</tr>
<tr id="row761414555118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p34277422"><a name="p34277422"></a><a name="p34277422"></a>code_filename</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p3839240115913"><a name="p3839240115913"></a><a name="p3839240115913"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p277424914328"><a name="p277424914328"></a><a name="p277424914328"></a>函数的文件名。</p>
<a name="ul98901953141211"></a><a name="ul98901953141211"></a><ul id="ul98901953141211"><li>当“code_type”为“zip”或“jar”时，必须提供该字段。</li><li>当“code_type”为“obs”或“inline”，不需要提供该字段。</li></ul>
</td>
</tr>
<tr id="row45128232510"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p44188613"><a name="p44188613"></a><a name="p44188613"></a>code_size</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p4850114010594"><a name="p4850114010594"></a><a name="p4850114010594"></a>Int64</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p22507915"><a name="p22507915"></a><a name="p22507915"></a>函数大小，单位：字节。</p>
</td>
</tr>
<tr id="row112081421205117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p9832816195415"><a name="p9832816195415"></a><a name="p9832816195415"></a>user_data</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p1861440185912"><a name="p1861440185912"></a><a name="p1861440185912"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p65331171333"><a name="p65331171333"></a><a name="p65331171333"></a>用户自定义的name/value信息，在函数中使用的参数。</p>
<p id="p45964432"><a name="p45964432"></a><a name="p45964432"></a>举例：如函数要访问某个主机，可以设置自定义参数：Host={host_ip}，最多定义20个，总长度不超过4KB。</p>
</td>
</tr>
<tr id="row12112101985115"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p20747816"><a name="p20747816"></a><a name="p20747816"></a>digest</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p1687714404594"><a name="p1687714404594"></a><a name="p1687714404594"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p2851512"><a name="p2851512"></a><a name="p2851512"></a>函数代码SHA512 hash值，用于判断函数是否变化。</p>
</td>
</tr>
<tr id="row134021765117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p65486773"><a name="p65486773"></a><a name="p65486773"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p388920409598"><a name="p388920409598"></a><a name="p388920409598"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p2828410"><a name="p2828410"></a><a name="p2828410"></a>函数版本号，由系统自动生成，规则：vYYYYMMDD-HHMMSS（v+年月日-时分秒）。</p>
</td>
</tr>
<tr id="row162071015105114"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p48645199"><a name="p48645199"></a><a name="p48645199"></a>image_name</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p189011840195919"><a name="p189011840195919"></a><a name="p189011840195919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p47947026"><a name="p47947026"></a><a name="p47947026"></a>函数版本的内部标识。</p>
</td>
</tr>
<tr id="row1251115812517"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p56772777"><a name="p56772777"></a><a name="p56772777"></a>xrole</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p139143403598"><a name="p139143403598"></a><a name="p139143403598"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p35192261"><a name="p35192261"></a><a name="p35192261"></a>函数使用的权限委托名称，需要IAM支持，并在IAM界面创建委托，当函数需要访问其他服务时，必须提供该字段。</p>
</td>
</tr>
<tr id="row354514614513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15157838201310"><a name="p15157838201310"></a><a name="p15157838201310"></a>app_xrole</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p8925154095912"><a name="p8925154095912"></a><a name="p8925154095912"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p215783891315"><a name="p215783891315"></a><a name="p215783891315"></a>函数app使用的权限委托名称，需要IAM支持，并在IAM界面创建委托，当函数需要访问其他服务时，必须提供该字段。</p>
</td>
</tr>
<tr id="row848184115116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19572290"><a name="p19572290"></a><a name="p19572290"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p17880477596"><a name="p17880477596"></a><a name="p17880477596"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p41851680"><a name="p41851680"></a><a name="p41851680"></a>函数描述。</p>
</td>
</tr>
<tr id="row722816218514"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p42450590"><a name="p42450590"></a><a name="p42450590"></a>version_description</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p7991247145910"><a name="p7991247145910"></a><a name="p7991247145910"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p15945784"><a name="p15945784"></a><a name="p15945784"></a>函数版本描述。</p>
</td>
</tr>
<tr id="row19286204517"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p16975145355517"><a name="p16975145355517"></a><a name="p16975145355517"></a>last_modified</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p20110547185915"><a name="p20110547185915"></a><a name="p20110547185915"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p45259754"><a name="p45259754"></a><a name="p45259754"></a>函数最后一次更新时间。</p>
</td>
</tr>
<tr id="row188192822711"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p78812287273"><a name="p78812287273"></a><a name="p78812287273"></a>depend_list</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p18881162882714"><a name="p18881162882714"></a><a name="p18881162882714"></a>[]String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p18881182842710"><a name="p18881182842710"></a><a name="p18881182842710"></a>依赖包列表。</p>
</td>
</tr>
<tr id="row1732519315277"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p163252312270"><a name="p163252312270"></a><a name="p163252312270"></a>strategy_config</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p1832518315276"><a name="p1832518315276"></a><a name="p1832518315276"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p18325531142712"><a name="p18325531142712"></a><a name="p18325531142712"></a>函数策略配置，请参考<a href="#table4775818446">表3</a>。</p>
</td>
</tr>
<tr id="row225127192"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p56491446899"><a name="p56491446899"></a><a name="p56491446899"></a>extend_config</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p166491461591"><a name="p166491461591"></a><a name="p166491461591"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p664918461915"><a name="p664918461915"></a><a name="p664918461915"></a>函数扩展配置。</p>
</td>
</tr>
<tr id="row636641018914"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p564910461791"><a name="p564910461791"></a><a name="p564910461791"></a>initializer_handler</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p564916463910"><a name="p564916463910"></a><a name="p564916463910"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p39611930183313"><a name="p39611930183313"></a><a name="p39611930183313"></a>函数初始化入口，规则：xx.xx，必须包含“. ”。</p>
<p id="p46491246490"><a name="p46491246490"></a><a name="p46491246490"></a>举例：对于Node.js函数：myfunction.initializer，则表示函数的文件名为myfunction.js，初始化的入口函数名为initializer。</p>
</td>
</tr>
<tr id="row18983171213911"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p16649144612911"><a name="p16649144612911"></a><a name="p16649144612911"></a>initializer_timeout</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p146491446791"><a name="p146491446791"></a><a name="p146491446791"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p1564917467913"><a name="p1564917467913"></a><a name="p1564917467913"></a>初始化超时时间，超时函数将被强行停止，范围1～300秒。</p>
</td>
</tr>
<tr id="row145286151296"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1264914461694"><a name="p1264914461694"></a><a name="p1264914461694"></a>func_vpc</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p1564919465910"><a name="p1564919465910"></a><a name="p1564919465910"></a>*String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p11649846890"><a name="p11649846890"></a><a name="p11649846890"></a>VPC配置，请参考<a href="获取函数列表.md#table11522131317013">表6</a>。</p>
</td>
</tr>
<tr id="row3101117131016"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p71033173107"><a name="p71033173107"></a><a name="p71033173107"></a>mount_config</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p16103161711105"><a name="p16103161711105"></a><a name="p16103161711105"></a>*String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p1810341717104"><a name="p1810341717104"></a><a name="p1810341717104"></a>磁盘挂载配置，请参考<a href="获取函数列表.md#table4760111014199">表7</a>。</p>
</td>
</tr>
<tr id="row9745162419207"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p84907518207"><a name="p84907518207"></a><a name="p84907518207"></a>encrypted_user_data</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.4.1.2 "><p id="p3745102492019"><a name="p3745102492019"></a><a name="p3745102492019"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.4.1.3 "><p id="p1074572452014"><a name="p1074572452014"></a><a name="p1074572452014"></a>函数加密配置。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  strategy\_config参数说明

<a name="table4775818446"></a>
<table><thead align="left"><tr id="row17785844414"><th class="cellrowborder" valign="top" width="15%" id="mcps1.2.5.1.1"><p id="p771581446"><a name="p771581446"></a><a name="p771581446"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.2"><p id="p1773582447"><a name="p1773582447"></a><a name="p1773582447"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="10%" id="mcps1.2.5.1.3"><p id="p107115884415"><a name="p107115884415"></a><a name="p107115884415"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="65%" id="mcps1.2.5.1.4"><p id="p974580442"><a name="p974580442"></a><a name="p974580442"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row47195819446"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.1 "><p id="p17775834410"><a name="p17775834410"></a><a name="p17775834410"></a>concurrency</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.2 "><p id="p9285359487"><a name="p9285359487"></a><a name="p9285359487"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="10%" headers="mcps1.2.5.1.3 "><p id="p13745811441"><a name="p13745811441"></a><a name="p13745811441"></a>必选</p>
</td>
<td class="cellrowborder" valign="top" width="65%" headers="mcps1.2.5.1.4 "><a name="ul935320313341"></a><a name="ul935320313341"></a><ul id="ul935320313341"><li>0：函数被禁用。</li><li>-1：函数被启用。</li></ul>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section1127134651713"></a>

**请求示例**

```
GET /v2/7aad83af3e8d42e99ac194e8419e2c9b/fgs/functions/urn:fss:xxxxxxxxx:7aad83af3e8d42e99ac194e8419e2c9b:function:default:test:latest/config HTTP/1.1
```

**响应示例**

**成功时的返回格式：**

```
HTTP/1.1 200 OK 
{ 
  "code_filename": "index.js", 
  "code_size": 272, 
  "code_type": "inline", 
  "cpu": 300, 
  "description": "111", 
  "digest": "decbce6939297b0b5ec6d1a23bf9c725870f5e69fc338a89a6a4029264688dc26338f56d08b6535de47f15ad538e22ca66613b9a46f807d50b687bb53fded1c6", 
  "func_name": "test", 
  "func_urn": "urn:fss:xxxxxxxxxx:7aad83af3e8d42e99ac194e8419e2c9b:function:default:test:latest", 
  "handler": "test.handler", 
  "image_name": "latest-5qe8e", 
  "last_modified": "2018-03-28T11:30:32+08:00", 
  "memory_size": 128, 
  "namespace": "7aad83af3e8d42e99ac194e8419e2c9b", 
  "package": "default", 
  "project_name": "xxxxxxxxx", 
  "runtime": "Node.js6.10", 
  "timeout": 3, 
  "user_domain": "cff01_hk", 
  "version": "latest", 
  "xrole": "cff",
  "strategy_config": {
      "concurrency": -1
  },
 }
```

**失败时的返回格式（示例）：**

```
HTTP/1.1 404 Not Found 
{ 
  "error_code": "FSS.1051", 
  "error_msg": "Not found the function" 
 }
```

## 状态码<a name="section39799274"></a>

状态码请参见[状态码](状态码.md)。

