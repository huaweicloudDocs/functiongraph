# FunctionGraph函数模型<a name="functiongraph_06_0102"></a>

## 函数模型<a name="section26908673"></a>

FunctionGraph函数模型如下。

```
{
	"FuncUrn": "string",
	"FuncName": "string",
	"UserDomain": "string",
	"Namespace": "string",
	"ProjectName": "string"
	"Package": "string",
	"Runtime": "string",
	"Timeout": number,
	"Handler": "string",
	"MemorySize": number,
	"Cpu": number,
	"CodeType": "string",
	"CodeUrl": "string",
	"CodeFileName": "string",
	"CodeSize": number,
	"UserData": "string",
	"Digest": "string",
	"Version": "string",
	"ImageName": "string",
	"DependencyPkg": "string",
	"Xrole": "string",
	"Description": "string",
	"VersionDescription": "string",
	"LastModified": "string",
	"FuncCode": {
		"File": "string"
	}
}
```

## 字段说明<a name="section40851470"></a>

FunctionGraph函数字段说明如[表1](#table4539774994724)所示。

**表 1**  FunctionGraph函数字段说明表

<a name="table4539774994724"></a>
<table><thead align="left"><tr id="row35845618"><th class="cellrowborder" valign="top" width="24.240000000000002%" id="mcps1.2.3.1.1"><p id="p17813907"><a name="p17813907"></a><a name="p17813907"></a>字段名称</p>
</th>
<th class="cellrowborder" valign="top" width="75.76%" id="mcps1.2.3.1.2"><p id="p33640357"><a name="p33640357"></a><a name="p33640357"></a>字段说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row40514383"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p60439610"><a name="p60439610"></a><a name="p60439610"></a>FuncUrn</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p63770254"><a name="p63770254"></a><a name="p63770254"></a>函数的URN（Uniform Resource Name），唯一标识函数。</p>
</td>
</tr>
<tr id="row37061374"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p49181313"><a name="p49181313"></a><a name="p49181313"></a>FuncName</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p24263425"><a name="p24263425"></a><a name="p24263425"></a>函数名称，只能以大小写字母开头，且只能包含字母、数字、下划线和中划线，以字母或者数字结尾。</p>
</td>
</tr>
<tr id="row17044235"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p38405776"><a name="p38405776"></a><a name="p38405776"></a>UserDomain</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p23860166"><a name="p23860166"></a><a name="p23860166"></a>租户名称。</p>
</td>
</tr>
<tr id="row13414907"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p12865660"><a name="p12865660"></a><a name="p12865660"></a>Namespace</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p35485571"><a name="p35485571"></a><a name="p35485571"></a>租户的project id。</p>
</td>
</tr>
<tr id="row50934683"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p32068643"><a name="p32068643"></a><a name="p32068643"></a>ProjectName</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p47423267"><a name="p47423267"></a><a name="p47423267"></a>租户的project name。</p>
</td>
</tr>
<tr id="row24156224"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p10497128"><a name="p10497128"></a><a name="p10497128"></a>Package</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p44961053"><a name="p44961053"></a><a name="p44961053"></a>函数所属的分组Package，用于用户针对函数的自定义分组。</p>
</td>
</tr>
<tr id="row1996295"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p27482234"><a name="p27482234"></a><a name="p27482234"></a>Runtime</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p652094462816"><a name="p652094462816"></a><a name="p652094462816"></a>FunctionGraph函数的执行环境，支持Node.js6.10、Python2.7、Python3.6、Java8、Go1.8、Node.js 8.10、C#.NET Core 2.0、C#.NET Core 2.1。</p>
</td>
</tr>
<tr id="row36107286"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p39009036"><a name="p39009036"></a><a name="p39009036"></a>Timeout</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p5615384"><a name="p5615384"></a><a name="p5615384"></a>函数的超时时间，超时函数将被强行停止，范围3～300秒。</p>
</td>
</tr>
<tr id="row50538456"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p67083165"><a name="p67083165"></a><a name="p67083165"></a>Handler</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p65027307"><a name="p65027307"></a><a name="p65027307"></a>函数执行入口，规则：xx.xx，必须包含“. ”，举例：对于node.js函数：myfunction.handler，则表示函数的文件名为myfunction.js，执行的入口函数名为handler。</p>
</td>
</tr>
<tr id="row48374852"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p26048945"><a name="p26048945"></a><a name="p26048945"></a>MemorySize</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p29589819"><a name="p29589819"></a><a name="p29589819"></a>函数消耗的内存，单位M，取值为128的整数倍，最小值为128，最大值为1536。</p>
</td>
</tr>
<tr id="row64981782"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p29032981"><a name="p29032981"></a><a name="p29032981"></a>Cpu</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p2861285"><a name="p2861285"></a><a name="p2861285"></a>函数占用的cpu资源，单位为millicore（1 core=1000 millicores），取值与MemorySize成比例，默认是128M内存占0.1个核（100 millicores），函数占用的CPU为基础CPU：200 millicores，再加上内存按比例占用的CPU，计算方法：内存/128 *100 + 200。</p>
</td>
</tr>
<tr id="row25751571"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p5502495"><a name="p5502495"></a><a name="p5502495"></a>CodeType</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p43048911"><a name="p43048911"></a><a name="p43048911"></a>函数代码类型，取值有4种：</p>
<p id="p51895880"><a name="p51895880"></a><a name="p51895880"></a>inline：UI在线编辑代码</p>
<p id="p64409739"><a name="p64409739"></a><a name="p64409739"></a>zip：函数代码为zip包</p>
<p id="p42816746"><a name="p42816746"></a><a name="p42816746"></a>jar：函数代码为jar包，主要针对Java函数</p>
<p id="p49806396"><a name="p49806396"></a><a name="p49806396"></a>obs：函数代码来源于obs存储</p>
</td>
</tr>
<tr id="row45604388"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p2967967"><a name="p2967967"></a><a name="p2967967"></a>CodeUrl</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p39078787"><a name="p39078787"></a><a name="p39078787"></a>当CodeType为obs时，该值为函数代码包在OBS上的地址，CodeType为其他值时，该字段为空；CodeUrl中文件名（url的由"/"分割的最后一段）也要符合CodeFileName字段的规范。</p>
</td>
</tr>
<tr id="row16164763"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p34277422"><a name="p34277422"></a><a name="p34277422"></a>CodeFileName</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p25007806"><a name="p25007806"></a><a name="p25007806"></a>函数的文件名，当CodeType为jar/zip时如果不提供该字段，会以函数名作为文件名，以CodeType作为文件类型，inline和obs不需要提供；文件名只能包含大小写字母、数字、中划线（-）、下划线（_）和点（.），另外文件名结尾要和CodeType对应。</p>
</td>
</tr>
<tr id="row23743664"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p44188613"><a name="p44188613"></a><a name="p44188613"></a>CodeSize</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p22507915"><a name="p22507915"></a><a name="p22507915"></a>函数大小，单位：字节。</p>
</td>
</tr>
<tr id="row1244648"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p33707641"><a name="p33707641"></a><a name="p33707641"></a>UserData</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p45964432"><a name="p45964432"></a><a name="p45964432"></a>用户自定义的name/value信息，在函数中使用的参数，举例：如函数要访问某个主机，可以设置自定义参数：Host={host_ip}，最多定义20个，总长度不超过4KB。</p>
</td>
</tr>
<tr id="row11026704"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p20747816"><a name="p20747816"></a><a name="p20747816"></a>Digest</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p2851512"><a name="p2851512"></a><a name="p2851512"></a>函数代码SHA512 hash值，用于判断函数是否变化。</p>
</td>
</tr>
<tr id="row25663613"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p65486773"><a name="p65486773"></a><a name="p65486773"></a>Version</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p2828410"><a name="p2828410"></a><a name="p2828410"></a>函数版本号，由系统自动生成，规则：vYYYYMMDD-HHMMSS（v+年月日-时分秒）。</p>
</td>
</tr>
<tr id="row25455692"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p48645199"><a name="p48645199"></a><a name="p48645199"></a>ImageName</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p47947026"><a name="p47947026"></a><a name="p47947026"></a>函数版本的内部标识。</p>
</td>
</tr>
<tr id="row28870051"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p56772777"><a name="p56772777"></a><a name="p56772777"></a>Xrole</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p35192261"><a name="p35192261"></a><a name="p35192261"></a>函数使用的权限委托名称，需要IAM支持，并在IAM界面创建委托，当函数需要访问其他服务时，必须提供该字段。</p>
</td>
</tr>
<tr id="row48294893"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p19572290"><a name="p19572290"></a><a name="p19572290"></a>Description</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p41851680"><a name="p41851680"></a><a name="p41851680"></a>函数描述。</p>
</td>
</tr>
<tr id="row41120801"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p42450590"><a name="p42450590"></a><a name="p42450590"></a>VersionDescription</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p15945784"><a name="p15945784"></a><a name="p15945784"></a>函数版本描述。</p>
</td>
</tr>
<tr id="row9294331"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p14643338"><a name="p14643338"></a><a name="p14643338"></a>LastModified</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p45259754"><a name="p45259754"></a><a name="p45259754"></a>函数最后一次更新时间。</p>
</td>
</tr>
<tr id="row4684608"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p43908956"><a name="p43908956"></a><a name="p43908956"></a>FuncCode.File</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p66964508"><a name="p66964508"></a><a name="p66964508"></a>函数代码，当CodeTye为inline/zip/jar时必选，且代码必须要进行base64编码。</p>
</td>
</tr>
</tbody>
</table>

FuncUrn格式如下。

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

