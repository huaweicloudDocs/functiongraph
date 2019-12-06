# 工作流定时器Cron表达式规则<a name="ZH-CN_TOPIC_0115410473"></a>

Cron表达式功能强大，但却难以理解，因为Cron表达式，实际由5或者6个子表达式构成，每个子表达式都有不同的规则和意义。子表达式的具体规则[表1](#table3976998615740)所示。

**表 1**  Cron子表达式规则

<a name="table3976998615740"></a>
<table><thead align="left"><tr id="row3744116215740"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p1283525915740"><a name="p1283525915740"></a><a name="p1283525915740"></a>字段</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p3302309015740"><a name="p3302309015740"></a><a name="p3302309015740"></a>填写说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row5762459615740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p3708071515740"><a name="p3708071515740"></a><a name="p3708071515740"></a>Minutes</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p5074796715740"><a name="p5074796715740"></a><a name="p5074796715740"></a>必选域，规则如下：</p>
<a name="ul5407852315740"></a><a name="ul5407852315740"></a><ul id="ul5407852315740"><li>允许值0-59</li><li>允许特殊字符, - * /</li></ul>
</td>
</tr>
<tr id="row3034047615740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p4165947715740"><a name="p4165947715740"></a><a name="p4165947715740"></a>Hours</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1897447515740"><a name="p1897447515740"></a><a name="p1897447515740"></a>必选域，规则如下：</p>
<a name="ul3655254815740"></a><a name="ul3655254815740"></a><ul id="ul3655254815740"><li>允许值0-23</li><li>允许特殊字符, - * /</li></ul>
</td>
</tr>
<tr id="row458858715740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p3613130315740"><a name="p3613130315740"></a><a name="p3613130315740"></a>Day-of-Month</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p4095439815740"><a name="p4095439815740"></a><a name="p4095439815740"></a>必选域，规则如下：</p>
<a name="ul3304526815740"></a><a name="ul3304526815740"></a><ul id="ul3304526815740"><li>允许值1-31（但要注意一些特别的月份的天数）</li><li>允许特殊字符, - * ? / L W</li></ul>
</td>
</tr>
<tr id="row6502761915740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p3274579215740"><a name="p3274579215740"></a><a name="p3274579215740"></a>Month</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p3516351415740"><a name="p3516351415740"></a><a name="p3516351415740"></a>必选域，规则如下：</p>
<a name="ul4803617315740"></a><a name="ul4803617315740"></a><ul id="ul4803617315740"><li>允许值1-12 或JAN-DEC（不区分大小写）</li><li>允许特殊字符, - * /</li></ul>
</td>
</tr>
<tr id="row5465225915740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p6475683415740"><a name="p6475683415740"></a><a name="p6475683415740"></a>Day-of-Week</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1081219015740"><a name="p1081219015740"></a><a name="p1081219015740"></a>必选域，规则如下：</p>
<a name="ul3020084615740"></a><a name="ul3020084615740"></a><ul id="ul3020084615740"><li>允许值1-7 或SUN-SAT（不区分大小写）</li><li>允许特殊字符, - * ? / L #</li></ul>
</td>
</tr>
<tr id="row470935415740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p4591341915740"><a name="p4591341915740"></a><a name="p4591341915740"></a>Year</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p2799949715740"><a name="p2799949715740"></a><a name="p2799949715740"></a>非必选域，规则如下：</p>
<a name="ul5066888615740"></a><a name="ul5066888615740"></a><ul id="ul5066888615740"><li>空或者1970-2099</li><li>允许特殊字符, - * /</li></ul>
</td>
</tr>
</tbody>
</table>

对于特殊字符的介绍如[表2](#table4836186915740)所示。

**表 2**  Cron表达式特殊字符介绍

<a name="table4836186915740"></a>
<table><thead align="left"><tr id="row3656918515740"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p931400215740"><a name="p931400215740"></a><a name="p931400215740"></a>特殊字符</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p1623666315740"><a name="p1623666315740"></a><a name="p1623666315740"></a>含义</p>
</th>
</tr>
</thead>
<tbody><tr id="row4010130415740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p2698022315740"><a name="p2698022315740"></a><a name="p2698022315740"></a>,</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><a name="ul3791441715740"></a><a name="ul3791441715740"></a><ul id="ul3791441715740"><li>用来定义追加的值（列表）。例如，在星期字段中的“MON，WED，FRI”指“星期一，星期三，星期五”。</li></ul>
</td>
</tr>
<tr id="row5116895215740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p5104447615740"><a name="p5104447615740"></a><a name="p5104447615740"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><a name="ul4096189215740"></a><a name="ul4096189215740"></a><ul id="ul4096189215740"><li>用来定义范围。例如，在时字段中的“10-12”指是“10，11及 12 点”。</li></ul>
</td>
</tr>
<tr id="row1091739215740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1189355615740"><a name="p1189355615740"></a><a name="p1189355615740"></a>*</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><a name="ul2385400915740"></a><a name="ul2385400915740"></a><ul id="ul2385400915740"><li>匹配某个字段内的所有的值。如，在“day of month”字段中的“*”代表“每天”。</li></ul>
</td>
</tr>
<tr id="row1438264215740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p2414334515740"><a name="p2414334515740"></a><a name="p2414334515740"></a>?</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><a name="ul945395315740"></a><a name="ul945395315740"></a><ul id="ul945395315740"><li>指不关心该字段的值，只能用在“Day-of-Month”和“Day-of-Week”字段中，例如设置计划每月10号执行，那面在Day-of-Week段需设置为？，表示不管周几。</li><li>该符号必须在两段中有且仅有一个。</li></ul>
</td>
</tr>
<tr id="row5606879515740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p4527855915740"><a name="p4527855915740"></a><a name="p4527855915740"></a>/</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><a name="ul4368462615740"></a><a name="ul4368462615740"></a><ul id="ul4368462615740"><li>用来定义增量，但只局限于存在的字段，如放在分钟段，会在0-59的范围增量，形如7/6，并不指每6个月，而是7月。</li></ul>
</td>
</tr>
<tr id="row4879385515740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p5998817215740"><a name="p5998817215740"></a><a name="p5998817215740"></a>L</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><a name="ul2720374515740"></a><a name="ul2720374515740"></a><ul id="ul2720374515740"><li>L只能用在“Day-of-Month”和“Day-of-Week”段。</li><li>在“Day-of-Month”段，表示月末，即一个月的最后一天（1 月的 31，平年 2 月的 28），你也可以指定从该月的最后第几天，如“L-3”这意味着日历月的最后第三天。</li><li>在“Day-of-Week”字段中，则表示 “7” 或 “SAT”，即星期六。在“Day-of-Week”字段中的“L” 出现在一个数字之后意思是“某个月的最后一个星期几”，如“6L”指“某个月的最后一个星期五”。</li><li>在使用“L”选项的时候最好不要再用列表、范围值，否则的话会得到令人迷惑的结果。</li></ul>
</td>
</tr>
<tr id="row938679915740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p2213325315740"><a name="p2213325315740"></a><a name="p2213325315740"></a>W</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><a name="ul4796303915740"></a><a name="ul4796303915740"></a><ul id="ul4796303915740"><li>只用在“Day-of-Month”用来定义距离给定某一天最近的一个工作日（星期一到星期五）。例如，在日期字段中定义了 “15W” 意思是“某个月中距离 15 号最近的一个工作日”。</li><li>“1W”，如果 1 号是星期六的话，触发器会在下个星期一即 3 号触发，它不会跳回到上个月去触发。“W” 只能定义在日期中字段中，并且在日期字段中只能定义单独的一天，不能定义一个范围或一个日期列表。</li><li>“L” 和 “W” 还可以组合出现在日期字段中，即“LW”，表示“某个月的最后一个工作日”。</li></ul>
</td>
</tr>
<tr id="row2474304615740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p5802972715740"><a name="p5802972715740"></a><a name="p5802972715740"></a>#</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><a name="ul278741615740"></a><a name="ul278741615740"></a><ul id="ul278741615740"><li>用来定义“某个月的第 n 个星期几”，只允许出现在星期字段中。例如，在星期字段中的“6#3”表示“某个月的第 3 个星期 5”（6 表示星期 5 ，3 表示某个月的第 3 周）。</li><li>如果在“Day-of-Week”段中出现该字符，则不能有多个表达式。如（“3#1,6#3”）是不合法的，因这里有两个表达式。</li></ul>
</td>
</tr>
</tbody>
</table>

Cron表达式范例如[表3](#table2763665815740)所示。

**表 3**  Cron表达式含义及范例

<a name="table2763665815740"></a>
<table><thead align="left"><tr id="row3082413715740"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p1372714515740"><a name="p1372714515740"></a><a name="p1372714515740"></a>含义</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p3815697015740"><a name="p3815697015740"></a><a name="p3815697015740"></a>Cron表达式范例</p>
</th>
</tr>
</thead>
<tbody><tr id="row370686715740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p3182084515740"><a name="p3182084515740"></a><a name="p3182084515740"></a>每1分钟执行一次</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p2735168015740"><a name="p2735168015740"></a><a name="p2735168015740"></a>*/1 * * * ?</p>
</td>
</tr>
<tr id="row4483853015740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p804228415740"><a name="p804228415740"></a><a name="p804228415740"></a>每天23点执行一次</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p4744525015740"><a name="p4744525015740"></a><a name="p4744525015740"></a>0 23 * * ?</p>
</td>
</tr>
<tr id="row2435407415740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p2652297415740"><a name="p2652297415740"></a><a name="p2652297415740"></a>每天凌晨1点执行一次</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p3558341815740"><a name="p3558341815740"></a><a name="p3558341815740"></a>0 1 * * ?</p>
</td>
</tr>
<tr id="row5181531115740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p3629062915740"><a name="p3629062915740"></a><a name="p3629062915740"></a>每月最后一天23点执行一次</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p513529015740"><a name="p513529015740"></a><a name="p513529015740"></a>0 23 L * ?</p>
</td>
</tr>
<tr id="row4621761115740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p5263902815740"><a name="p5263902815740"></a><a name="p5263902815740"></a>每周星期天凌晨1点实行一次</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p71705715740"><a name="p71705715740"></a><a name="p71705715740"></a>0 1 ? * L</p>
</td>
</tr>
<tr id="row645352015740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p5297309815740"><a name="p5297309815740"></a><a name="p5297309815740"></a>在26分、29分、33分执行一次</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p5943666015740"><a name="p5943666015740"></a><a name="p5943666015740"></a>26,29,33 * * * ?</p>
</td>
</tr>
<tr id="row6516789415740"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p4410804315740"><a name="p4410804315740"></a><a name="p4410804315740"></a>每天的0点、13点、18点、21点都执行一次</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p3082527915740"><a name="p3082527915740"></a><a name="p3082527915740"></a>0 0,13,18,21 * * ?</p>
</td>
</tr>
</tbody>
</table>

