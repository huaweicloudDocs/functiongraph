# 工作流定时器Cron表达式说明<a name="ZH-CN_TOPIC_0149027333"></a>

工作流定时器Cron表达式由5或者6个子表达式构成，每个子表达式都有不同的规则和意义，可以实现复杂的工作流执行规则。子表达式的具体规则如[表1](#table392462612523)所示。

**表 1**  子表达式具体规则说明

<a name="table392462612523"></a>
<table><thead align="left"><tr id="row1692422620527"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p168922356522"><a name="p168922356522"></a><a name="p168922356522"></a>字段</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p2900133575213"><a name="p2900133575213"></a><a name="p2900133575213"></a>填写说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row192462615526"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p13900133565220"><a name="p13900133565220"></a><a name="p13900133565220"></a>Minutes</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p5900103575210"><a name="p5900103575210"></a><a name="p5900103575210"></a>必选域，规则如下：</p>
<a name="ul89002350524"></a><a name="ul89002350524"></a><ul id="ul89002350524"><li>允许值0-59</li><li>允许特殊字符, - * /</li></ul>
</td>
</tr>
<tr id="row10924112665219"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1916153565216"><a name="p1916153565216"></a><a name="p1916153565216"></a>Hours</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p119161635175214"><a name="p119161635175214"></a><a name="p119161635175214"></a>必选域，规则如下：</p>
<a name="ul11916163511522"></a><a name="ul11916163511522"></a><ul id="ul11916163511522"><li>允许值0-23</li><li>允许特殊字符, - * /</li></ul>
</td>
</tr>
<tr id="row14924102655217"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p10924153510522"><a name="p10924153510522"></a><a name="p10924153510522"></a>Day-of-Month</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1592403535219"><a name="p1592403535219"></a><a name="p1592403535219"></a>必选域，规则如下：</p>
<a name="ul1592412354529"></a><a name="ul1592412354529"></a><ul id="ul1592412354529"><li>允许值1-31（但要注意一些特别的月份的天数）</li><li>允许特殊字符, - * ? / L W</li></ul>
</td>
</tr>
<tr id="row1092452616522"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p4931123595218"><a name="p4931123595218"></a><a name="p4931123595218"></a>Month</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p8931153515529"><a name="p8931153515529"></a><a name="p8931153515529"></a>必选域，规则如下：</p>
<a name="ul1393153515521"></a><a name="ul1393153515521"></a><ul id="ul1393153515521"><li>允许值1-12或JAN-DEC（不区分大小写）</li><li>允许特殊字符, - * /</li></ul>
</td>
</tr>
<tr id="row189240264524"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p199394353524"><a name="p199394353524"></a><a name="p199394353524"></a>Day-of-Week</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p159391235115213"><a name="p159391235115213"></a><a name="p159391235115213"></a>必选域，规则如下：</p>
<a name="ul129391435165210"></a><a name="ul129391435165210"></a><ul id="ul129391435165210"><li>允许值1-7或SUN-SAT（不区分大小写）</li><li>允许特殊字符, - * ? / L #</li></ul>
</td>
</tr>
<tr id="row5924172665216"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p694723585213"><a name="p694723585213"></a><a name="p694723585213"></a>Year</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p11947335165220"><a name="p11947335165220"></a><a name="p11947335165220"></a>非必选域，规则如下：</p>
<a name="ul1494783555213"></a><a name="ul1494783555213"></a><ul id="ul1494783555213"><li>空或者1970-2099</li><li>允许特殊字符, - * /</li></ul>
</td>
</tr>
</tbody>
</table>

对于特殊字符的介绍如[表2](#table1741101085420)所示。

**表 2**  特殊字符含义介绍

<a name="table1741101085420"></a>
<table><thead align="left"><tr id="row37411110185411"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p1150119467546"><a name="p1150119467546"></a><a name="p1150119467546"></a>特殊字符</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p1350114612549"><a name="p1350114612549"></a><a name="p1350114612549"></a>含义</p>
</th>
</tr>
</thead>
<tbody><tr id="row107416102542"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p750944616542"><a name="p750944616542"></a><a name="p750944616542"></a>,</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><a name="ul3509846135414"></a><a name="ul3509846135414"></a><ul id="ul3509846135414"><li>用来定义追加的值（列表）。例如，在星期字段中的“MON，WED，FRI”指“星期一，星期三，星期五”。</li></ul>
</td>
</tr>
<tr id="row3751181919548"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p8516246115420"><a name="p8516246115420"></a><a name="p8516246115420"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><a name="ul14524104612549"></a><a name="ul14524104612549"></a><ul id="ul14524104612549"><li>用来定义范围。例如，在时字段中的“10-12”指是“10，11 及 12 点”</li></ul>
</td>
</tr>
<tr id="row1674111016549"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p25321446125414"><a name="p25321446125414"></a><a name="p25321446125414"></a>*</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><a name="ul653214620543"></a><a name="ul653214620543"></a><ul id="ul653214620543"><li>匹配某个字段内的所有的值。如，在“day of month”字段中的“*”代表“每天”。</li></ul>
</td>
</tr>
<tr id="row674101085416"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p185481146155416"><a name="p185481146155416"></a><a name="p185481146155416"></a>?</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><a name="ul55482046195414"></a><a name="ul55482046195414"></a><ul id="ul55482046195414"><li>指不关心该字段的值，只能用在“Day-of-Month”和“Day-of-Week”字段中，例如设置计划每月10号执行，那面在Day-of-Week段需设置为？，表示不管周几。</li><li>该符号必须在两段中有且仅有一个。</li></ul>
</td>
</tr>
<tr id="row1474171055411"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p2563124645418"><a name="p2563124645418"></a><a name="p2563124645418"></a>/</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><a name="ul19563134645416"></a><a name="ul19563134645416"></a><ul id="ul19563134645416"><li>用来定义增量，但只局限于存在的字段。比如7/6，如放在分钟段，会在0-59的范围增量，如放在月度段，只指7月份。</li></ul>
</td>
</tr>
<tr id="row974191012542"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1571174625412"><a name="p1571174625412"></a><a name="p1571174625412"></a>L</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><a name="ul6571114618542"></a><a name="ul6571114618542"></a><ul id="ul6571114618542"><li>L只能用在“Day-of-Month”和“Day-of-Week”段。</li><li>在“Day-of-Month”段，表示月末，即一个月的最后一天（1 月的 31，平年 2 月的 28），你也可以指定从该月的最后第几天，如“L-3”这意味着日历月的最后第三天。</li><li>在“Day-of-Week”字段中，则表示 “7” 或 “SAT”，即星期六。在“Day-of-Week”字段中的 “L” 出现在一个数字之后意思是“某个月的最后一个星期几”，如“6L”指“某个月的最后一个星期五”。</li><li>在使用“L”选项的时候最好不要再用列表、范围值，否则的话会得到令人迷惑的结果。</li></ul>
</td>
</tr>
<tr id="row974101013544"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p759594613548"><a name="p759594613548"></a><a name="p759594613548"></a>W</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><a name="ul136028463545"></a><a name="ul136028463545"></a><ul id="ul136028463545"><li>只用在“Day-of-Month”用来定义距离给定某一天最近的一个工作日（星期一到星期五）。例如，在日期字段中定义了 “15W” 意思是“某个月中距离 15 号最近的一个工作日”。</li><li>“1W”，如果 1 号是星期六的话，定时器会在下个星期一即 3 号触发，它不会跳回到上个月去触发。“W” 只能定义在日期中字段中，并且在日期字段中只能定义单独的一天，不能定义一个范围或一个日期列表。</li><li>“L” 和 “W” 还可以组合出现在日期字段中，即“LW”，表示“某个月的最后一个工作日”。</li></ul>
</td>
</tr>
<tr id="row174131013541"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1862634614548"><a name="p1862634614548"></a><a name="p1862634614548"></a>#</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><a name="ul136261246115414"></a><a name="ul136261246115414"></a><ul id="ul136261246115414"><li>用来定义“某个月的第 n 个星期几”，只允许出现在星期字段中。例如，在星期字段中的“6#3”表示“某个月的第 3 个星期 5”（6 表示星期 5 ，3 表示某个月的第 3 周）。</li><li>如果在“Day-of-Week”段中出现该字符，则不能有多个表达式。如（“3#1,6#3”）是不合法的，因这里有两个表达式。</li></ul>
</td>
</tr>
</tbody>
</table>

Cron表达式范例如[表3](#table0360185510551)所示。

**表 3**  Cron表达式范例

<a name="table0360185510551"></a>
<table><thead align="left"><tr id="row13601855145519"><th class="cellrowborder" valign="top" width="48%" id="mcps1.2.3.1.1"><p id="p10930151125617"><a name="p10930151125617"></a><a name="p10930151125617"></a>Cron表达式范例</p>
</th>
<th class="cellrowborder" valign="top" width="52%" id="mcps1.2.3.1.2"><p id="p41741346134213"><a name="p41741346134213"></a><a name="p41741346134213"></a>含义</p>
</th>
</tr>
</thead>
<tbody><tr id="row136019553551"><td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.3.1.1 "><p id="p1593811117566"><a name="p1593811117566"></a><a name="p1593811117566"></a>*/1 * * * ?</p>
</td>
<td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.3.1.2 "><p id="p017714462429"><a name="p017714462429"></a><a name="p017714462429"></a>每1分钟执行一次</p>
</td>
</tr>
<tr id="row1036045545516"><td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.3.1.1 "><p id="p994631195617"><a name="p994631195617"></a><a name="p994631195617"></a>0 23 * * ?</p>
</td>
<td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.3.1.2 "><p id="p161801946154214"><a name="p161801946154214"></a><a name="p161801946154214"></a>每天23点执行一次</p>
</td>
</tr>
<tr id="row8360115575513"><td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.3.1.1 "><p id="p2095410116565"><a name="p2095410116565"></a><a name="p2095410116565"></a>0 1 * * ?</p>
</td>
<td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.3.1.2 "><p id="p1618411466425"><a name="p1618411466425"></a><a name="p1618411466425"></a>每天凌晨1点执行一次</p>
</td>
</tr>
<tr id="row836095545520"><td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.3.1.1 "><p id="p189541019563"><a name="p189541019563"></a><a name="p189541019563"></a>0 23 L * ?</p>
</td>
<td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.3.1.2 "><p id="p018814616427"><a name="p018814616427"></a><a name="p018814616427"></a>每月最后一天23点执行一次</p>
</td>
</tr>
<tr id="row6360165535510"><td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.3.1.1 "><p id="p196161135611"><a name="p196161135611"></a><a name="p196161135611"></a>0 1 ? * L</p>
</td>
<td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.3.1.2 "><p id="p41921546134214"><a name="p41921546134214"></a><a name="p41921546134214"></a>每周星期天凌晨1点实行一次</p>
</td>
</tr>
<tr id="row133608553559"><td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.3.1.1 "><p id="p39691010562"><a name="p39691010562"></a><a name="p39691010562"></a>26,29,33 * * * ?</p>
</td>
<td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.3.1.2 "><p id="p10194946144217"><a name="p10194946144217"></a><a name="p10194946144217"></a>在26分、29分、33分执行一次</p>
</td>
</tr>
<tr id="row9360135595516"><td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.3.1.1 "><p id="p2096918115565"><a name="p2096918115565"></a><a name="p2096918115565"></a>0 0,13,18,21 * * ?</p>
</td>
<td class="cellrowborder" valign="top" width="52%" headers="mcps1.2.3.1.2 "><p id="p119612461421"><a name="p119612461421"></a><a name="p119612461421"></a>每天的0点、13点、18点、21点都执行一次</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-notice.gif) **须知：**   
>对于有的定时规则用cron表达式会比较复杂，例如，使用一个表达式来表示“9点到10点的每五分钟及13点到22点的每20分钟”，解决这种场景，建议使用两个定时器来完成。  

