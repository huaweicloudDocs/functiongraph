# FunctionGraph服务监控指标说明<a name="ZH-CN_TOPIC_0134295092"></a>

## 功能说明<a name="section37797504358"></a>

本节定义了FunctionGraph服务中“函数”上报云监控服务的监控指标。

指标的命名空间和维度，您可以通过云监控服务提供的API接口来检索FunctionGraph服务中“函数”产生的监控指标和告警信息。

## 命名空间<a name="section08080510301"></a>

SYS.FunctionGraph

## 监控指标<a name="section10550132020361"></a>

**表 1**  监控指标

<a name="table3687212203710"></a>
<table><thead align="left"><tr id="row1268871212379"><th class="cellrowborder" valign="top" width="9.090909090909092%" id="mcps1.2.11.1.1"><p id="p3607154316377"><a name="p3607154316377"></a><a name="p3607154316377"></a><strong id="b48959453436"><a name="b48959453436"></a><a name="b48959453436"></a>指标名称</strong></p>
</th>
<th class="cellrowborder" valign="top" width="9.090909090909092%" id="mcps1.2.11.1.2"><p id="p206084433375"><a name="p206084433375"></a><a name="p206084433375"></a><strong id="b14897144554319"><a name="b14897144554319"></a><a name="b14897144554319"></a>显示名</strong></p>
</th>
<th class="cellrowborder" valign="top" width="12.858585858585858%" id="mcps1.2.11.1.3"><p id="p8608194311378"><a name="p8608194311378"></a><a name="p8608194311378"></a><strong id="b1989744584315"><a name="b1989744584315"></a><a name="b1989744584315"></a>描述</strong></p>
</th>
<th class="cellrowborder" valign="top" width="5.323232323232323%" id="mcps1.2.11.1.4"><p id="p1760818431373"><a name="p1760818431373"></a><a name="p1760818431373"></a><strong id="b6898144574315"><a name="b6898144574315"></a><a name="b6898144574315"></a>单位</strong></p>
</th>
<th class="cellrowborder" valign="top" width="8.080808080808081%" id="mcps1.2.11.1.5"><p id="p2608204316374"><a name="p2608204316374"></a><a name="p2608204316374"></a><strong id="b10900134554314"><a name="b10900134554314"></a><a name="b10900134554314"></a>上限值</strong></p>
</th>
<th class="cellrowborder" valign="top" width="8.080808080808081%" id="mcps1.2.11.1.6"><p id="p106088430373"><a name="p106088430373"></a><a name="p106088430373"></a><strong id="b7901134516431"><a name="b7901134516431"></a><a name="b7901134516431"></a>下限值</strong></p>
</th>
<th class="cellrowborder" valign="top" width="8.080808080808081%" id="mcps1.2.11.1.7"><p id="p116081443193712"><a name="p116081443193712"></a><a name="p116081443193712"></a><strong id="b390354574319"><a name="b390354574319"></a><a name="b390354574319"></a>建议阈值</strong></p>
</th>
<th class="cellrowborder" valign="top" width="7.070707070707072%" id="mcps1.2.11.1.8"><p id="p760854310378"><a name="p760854310378"></a><a name="p760854310378"></a><strong id="b15904134584310"><a name="b15904134584310"></a><a name="b15904134584310"></a>值类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="16.161616161616163%" id="mcps1.2.11.1.9"><p id="p96081943173720"><a name="p96081943173720"></a><a name="p96081943173720"></a><strong id="b15906154544318"><a name="b15906154544318"></a><a name="b15906154544318"></a>指标意义</strong></p>
</th>
<th class="cellrowborder" valign="top" width="16.161616161616163%" id="mcps1.2.11.1.10"><p id="p15608543133711"><a name="p15608543133711"></a><a name="p15608543133711"></a><strong id="b149060456438"><a name="b149060456438"></a><a name="b149060456438"></a>所属维度</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row068911283714"><td class="cellrowborder" valign="top" width="9.090909090909092%" headers="mcps1.2.11.1.1 "><p id="p1608104314376"><a name="p1608104314376"></a><a name="p1608104314376"></a>count</p>
</td>
<td class="cellrowborder" valign="top" width="9.090909090909092%" headers="mcps1.2.11.1.2 "><p id="p1608243123717"><a name="p1608243123717"></a><a name="p1608243123717"></a>调用次数</p>
</td>
<td class="cellrowborder" valign="top" width="12.858585858585858%" headers="mcps1.2.11.1.3 "><p id="p960874317373"><a name="p960874317373"></a><a name="p960874317373"></a>该指标用于统计函数调用次数</p>
</td>
<td class="cellrowborder" valign="top" width="5.323232323232323%" headers="mcps1.2.11.1.4 "><p id="p1860844313378"><a name="p1860844313378"></a><a name="p1860844313378"></a>次数</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.5 "><p id="p146081243173719"><a name="p146081243173719"></a><a name="p146081243173719"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.6 "><p id="p960916437379"><a name="p960916437379"></a><a name="p960916437379"></a>0</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.7 "><p id="p9609154311376"><a name="p9609154311376"></a><a name="p9609154311376"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="7.070707070707072%" headers="mcps1.2.11.1.8 "><p id="p160916436373"><a name="p160916436373"></a><a name="p160916436373"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.11.1.9 "><p id="p660974323719"><a name="p660974323719"></a><a name="p660974323719"></a>该指标用于统计函数调用次数</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.11.1.10 "><p id="p160914313371"><a name="p160914313371"></a><a name="p160914313371"></a>package-functionname</p>
</td>
</tr>
<tr id="row1669051219377"><td class="cellrowborder" valign="top" width="9.090909090909092%" headers="mcps1.2.11.1.1 "><p id="p18609643153718"><a name="p18609643153718"></a><a name="p18609643153718"></a>failcount</p>
</td>
<td class="cellrowborder" valign="top" width="9.090909090909092%" headers="mcps1.2.11.1.2 "><p id="p660915438373"><a name="p660915438373"></a><a name="p660915438373"></a>错误次数</p>
</td>
<td class="cellrowborder" valign="top" width="12.858585858585858%" headers="mcps1.2.11.1.3 "><p id="p146091843193714"><a name="p146091843193714"></a><a name="p146091843193714"></a>该指标用于统计函数调用错误次数</p>
</td>
<td class="cellrowborder" valign="top" width="5.323232323232323%" headers="mcps1.2.11.1.4 "><p id="p76091343143719"><a name="p76091343143719"></a><a name="p76091343143719"></a>次数</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.5 "><p id="p86731741104012"><a name="p86731741104012"></a><a name="p86731741104012"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.6 "><p id="p10674641194016"><a name="p10674641194016"></a><a name="p10674641194016"></a>0</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.7 "><p id="p367510411400"><a name="p367510411400"></a><a name="p367510411400"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="7.070707070707072%" headers="mcps1.2.11.1.8 "><p id="p861064353711"><a name="p861064353711"></a><a name="p861064353711"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.11.1.9 "><p id="p10610543193720"><a name="p10610543193720"></a><a name="p10610543193720"></a>该指标用于统计函数调用错误次数</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.11.1.10 "><p id="p261004318379"><a name="p261004318379"></a><a name="p261004318379"></a>package-functionname</p>
</td>
</tr>
<tr id="row169014128378"><td class="cellrowborder" valign="top" width="9.090909090909092%" headers="mcps1.2.11.1.1 "><p id="p961074363716"><a name="p961074363716"></a><a name="p961074363716"></a>rejectcount</p>
</td>
<td class="cellrowborder" valign="top" width="9.090909090909092%" headers="mcps1.2.11.1.2 "><p id="p116101743183716"><a name="p116101743183716"></a><a name="p116101743183716"></a>被拒绝次数</p>
</td>
<td class="cellrowborder" valign="top" width="12.858585858585858%" headers="mcps1.2.11.1.3 "><p id="p126101943183716"><a name="p126101943183716"></a><a name="p126101943183716"></a>该指标用于统计函数调用被拒绝次数</p>
</td>
<td class="cellrowborder" valign="top" width="5.323232323232323%" headers="mcps1.2.11.1.4 "><p id="p761084312374"><a name="p761084312374"></a><a name="p761084312374"></a>次数</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.5 "><p id="p19560184419404"><a name="p19560184419404"></a><a name="p19560184419404"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.6 "><p id="p145621449401"><a name="p145621449401"></a><a name="p145621449401"></a>0</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.7 "><p id="p11563194412405"><a name="p11563194412405"></a><a name="p11563194412405"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="7.070707070707072%" headers="mcps1.2.11.1.8 "><p id="p7610943183717"><a name="p7610943183717"></a><a name="p7610943183717"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.11.1.9 "><p id="p12610154315374"><a name="p12610154315374"></a><a name="p12610154315374"></a>该指标用于统计函数调用被拒绝次数</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.11.1.10 "><p id="p161044363718"><a name="p161044363718"></a><a name="p161044363718"></a>package-functionname</p>
</td>
</tr>
<tr id="row18690912173710"><td class="cellrowborder" valign="top" width="9.090909090909092%" headers="mcps1.2.11.1.1 "><p id="p1661064393711"><a name="p1661064393711"></a><a name="p1661064393711"></a>duration</p>
</td>
<td class="cellrowborder" valign="top" width="9.090909090909092%" headers="mcps1.2.11.1.2 "><p id="p1610143113718"><a name="p1610143113718"></a><a name="p1610143113718"></a>平均运行时间</p>
</td>
<td class="cellrowborder" valign="top" width="12.858585858585858%" headers="mcps1.2.11.1.3 "><p id="p18610144343719"><a name="p18610144343719"></a><a name="p18610144343719"></a>该指标用于统计函数调用平均运行时间</p>
</td>
<td class="cellrowborder" valign="top" width="5.323232323232323%" headers="mcps1.2.11.1.4 "><p id="p5610124320372"><a name="p5610124320372"></a><a name="p5610124320372"></a>毫秒</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.5 "><p id="p816474634018"><a name="p816474634018"></a><a name="p816474634018"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.6 "><p id="p181642465409"><a name="p181642465409"></a><a name="p181642465409"></a>0</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.7 "><p id="p616614664018"><a name="p616614664018"></a><a name="p616614664018"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="7.070707070707072%" headers="mcps1.2.11.1.8 "><p id="p20611343133710"><a name="p20611343133710"></a><a name="p20611343133710"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.11.1.9 "><p id="p1461114433378"><a name="p1461114433378"></a><a name="p1461114433378"></a>该指标用于统计函数调用平均运行时间</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.11.1.10 "><p id="p1361124313719"><a name="p1361124313719"></a><a name="p1361124313719"></a>package-functionname</p>
</td>
</tr>
<tr id="row16691812133719"><td class="cellrowborder" valign="top" width="9.090909090909092%" headers="mcps1.2.11.1.1 "><p id="p196111143153711"><a name="p196111143153711"></a><a name="p196111143153711"></a>maxDuration</p>
</td>
<td class="cellrowborder" valign="top" width="9.090909090909092%" headers="mcps1.2.11.1.2 "><p id="p1461118437379"><a name="p1461118437379"></a><a name="p1461118437379"></a>最大运行时间</p>
</td>
<td class="cellrowborder" valign="top" width="12.858585858585858%" headers="mcps1.2.11.1.3 "><p id="p7611114333711"><a name="p7611114333711"></a><a name="p7611114333711"></a>该指标用于统计函数调用最大运行时间</p>
</td>
<td class="cellrowborder" valign="top" width="5.323232323232323%" headers="mcps1.2.11.1.4 "><p id="p5611184315375"><a name="p5611184315375"></a><a name="p5611184315375"></a>毫秒</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.5 "><p id="p157418473408"><a name="p157418473408"></a><a name="p157418473408"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.6 "><p id="p15575134754012"><a name="p15575134754012"></a><a name="p15575134754012"></a>0</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.7 "><p id="p15576134744014"><a name="p15576134744014"></a><a name="p15576134744014"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="7.070707070707072%" headers="mcps1.2.11.1.8 "><p id="p1361114318375"><a name="p1361114318375"></a><a name="p1361114318375"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.11.1.9 "><p id="p146111143173712"><a name="p146111143173712"></a><a name="p146111143173712"></a>该指标用于统计函数调用最大运行时间</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.11.1.10 "><p id="p561174323714"><a name="p561174323714"></a><a name="p561174323714"></a>package-functionname</p>
</td>
</tr>
<tr id="row206911912193714"><td class="cellrowborder" valign="top" width="9.090909090909092%" headers="mcps1.2.11.1.1 "><p id="p2611243193712"><a name="p2611243193712"></a><a name="p2611243193712"></a>minDuration</p>
</td>
<td class="cellrowborder" valign="top" width="9.090909090909092%" headers="mcps1.2.11.1.2 "><p id="p1761164313714"><a name="p1761164313714"></a><a name="p1761164313714"></a>最小运行时间</p>
</td>
<td class="cellrowborder" valign="top" width="12.858585858585858%" headers="mcps1.2.11.1.3 "><p id="p17611243113714"><a name="p17611243113714"></a><a name="p17611243113714"></a>该指标用于统计函数调用最小运行时间</p>
</td>
<td class="cellrowborder" valign="top" width="5.323232323232323%" headers="mcps1.2.11.1.4 "><p id="p12611643153719"><a name="p12611643153719"></a><a name="p12611643153719"></a>毫秒</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.5 "><p id="p19879048124015"><a name="p19879048124015"></a><a name="p19879048124015"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.6 "><p id="p088024864010"><a name="p088024864010"></a><a name="p088024864010"></a>0</p>
</td>
<td class="cellrowborder" valign="top" width="8.080808080808081%" headers="mcps1.2.11.1.7 "><p id="p188814487404"><a name="p188814487404"></a><a name="p188814487404"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="7.070707070707072%" headers="mcps1.2.11.1.8 "><p id="p86121043163717"><a name="p86121043163717"></a><a name="p86121043163717"></a>Int</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.11.1.9 "><p id="p1361234312372"><a name="p1361234312372"></a><a name="p1361234312372"></a>该指标用于统计函数调用最小运行时间</p>
</td>
<td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.2.11.1.10 "><p id="p19612124383720"><a name="p19612124383720"></a><a name="p19612124383720"></a>package-functionname</p>
</td>
</tr>
</tbody>
</table>

## 维度<a name="section18855813194218"></a>

**表 2**  维度

<a name="table101881229134219"></a>
<table><thead align="left"><tr id="row151881029184210"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p7189122904219"><a name="p7189122904219"></a><a name="p7189122904219"></a><strong id="b15375253114312"><a name="b15375253114312"></a><a name="b15375253114312"></a>Key</strong></p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p9189729184215"><a name="p9189729184215"></a><a name="p9189729184215"></a><strong id="b113767535438"><a name="b113767535438"></a><a name="b113767535438"></a>Value</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row12189329134220"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p11786175818487"><a name="p11786175818487"></a><a name="p11786175818487"></a>package-functionname</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1718918298421"><a name="p1718918298421"></a><a name="p1718918298421"></a>应用名称-函数名称</p>
</td>
</tr>
</tbody>
</table>

