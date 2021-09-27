# FunctionGraph服务的监控指标参考<a name="ZH-CN_TOPIC_0195706908"></a>

## 功能说明<a name="section37243617558"></a>

本节定义了FunctionGraph上报云监控服务的监控指标的命名空间，监控指标列表和维度定义，用户可以通过云监控服务提供管理控制台或API接口来检索FunctionGraph产生的监控指标和告警信息。

## 命名空间<a name="section177503620559"></a>

SYS.FunctionGraph

## 函数监控指标<a name="section177783615510"></a>

<a name="table692281511117"></a>
<table><thead align="left"><tr id="row11923101510116"><th class="cellrowborder" valign="top" width="17.956408718256352%" id="mcps1.1.7.1.1"><p id="p1595311435285"><a name="p1595311435285"></a><a name="p1595311435285"></a>指标</p>
</th>
<th class="cellrowborder" valign="top" width="15.486902619476107%" id="mcps1.1.7.1.2"><p id="p139231315917"><a name="p139231315917"></a><a name="p139231315917"></a>指标名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.86482703459308%" id="mcps1.1.7.1.3"><p id="p192314153115"><a name="p192314153115"></a><a name="p192314153115"></a>含义</p>
</th>
<th class="cellrowborder" valign="top" width="14.057188562287543%" id="mcps1.1.7.1.4"><p id="p99231515512"><a name="p99231515512"></a><a name="p99231515512"></a>取值范围</p>
</th>
<th class="cellrowborder" valign="top" width="11.327734453109379%" id="mcps1.1.7.1.5"><p id="p392314151917"><a name="p392314151917"></a><a name="p392314151917"></a>测量对象</p>
</th>
<th class="cellrowborder" valign="top" width="15.306938612277547%" id="mcps1.1.7.1.6"><p id="p1923615418"><a name="p1923615418"></a><a name="p1923615418"></a>监控周期（原始指标）</p>
</th>
</tr>
</thead>
<tbody><tr id="row1992318151612"><td class="cellrowborder" valign="top" width="17.956408718256352%" headers="mcps1.1.7.1.1 "><p id="p1895304342820"><a name="p1895304342820"></a><a name="p1895304342820"></a>count</p>
</td>
<td class="cellrowborder" valign="top" width="15.486902619476107%" headers="mcps1.1.7.1.2 "><p id="p12105192310115"><a name="p12105192310115"></a><a name="p12105192310115"></a>调用次数</p>
</td>
<td class="cellrowborder" valign="top" width="25.86482703459308%" headers="mcps1.1.7.1.3 "><p id="p7105623312"><a name="p7105623312"></a><a name="p7105623312"></a>该指标用于统计函数调用次数。</p>
<p id="p410582315115"><a name="p410582315115"></a><a name="p410582315115"></a>单位：次</p>
</td>
<td class="cellrowborder" valign="top" width="14.057188562287543%" headers="mcps1.1.7.1.4 "><p id="p81051923812"><a name="p81051923812"></a><a name="p81051923812"></a>≥ 0 counts</p>
</td>
<td class="cellrowborder" valign="top" width="11.327734453109379%" headers="mcps1.1.7.1.5 "><p id="p1410542313111"><a name="p1410542313111"></a><a name="p1410542313111"></a>函数</p>
</td>
<td class="cellrowborder" valign="top" width="15.306938612277547%" headers="mcps1.1.7.1.6 "><p id="p121058236119"><a name="p121058236119"></a><a name="p121058236119"></a>1分钟</p>
</td>
</tr>
<tr id="row392312156116"><td class="cellrowborder" valign="top" width="17.956408718256352%" headers="mcps1.1.7.1.1 "><p id="p7953943172814"><a name="p7953943172814"></a><a name="p7953943172814"></a>failcount</p>
</td>
<td class="cellrowborder" valign="top" width="15.486902619476107%" headers="mcps1.1.7.1.2 "><p id="p15105192310112"><a name="p15105192310112"></a><a name="p15105192310112"></a>错误次数</p>
</td>
<td class="cellrowborder" valign="top" width="25.86482703459308%" headers="mcps1.1.7.1.3 "><p id="p17105142315118"><a name="p17105142315118"></a><a name="p17105142315118"></a>该指标用于统计函数调用错误次数。</p>
<p id="p564717151895"><a name="p564717151895"></a><a name="p564717151895"></a>以下两种情况都会记入错误次数：</p>
<a name="ul645810174920"></a><a name="ul645810174920"></a><ul id="ul645810174920"><li>函数请求异常，导致无法执行完成且返回200。</li><li>函数自身语法错误或者自身执行错误。</li></ul>
<p id="p1410518233118"><a name="p1410518233118"></a><a name="p1410518233118"></a>单位：次</p>
</td>
<td class="cellrowborder" valign="top" width="14.057188562287543%" headers="mcps1.1.7.1.4 "><p id="p191057232015"><a name="p191057232015"></a><a name="p191057232015"></a>≥ 0 counts</p>
</td>
<td class="cellrowborder" valign="top" width="11.327734453109379%" headers="mcps1.1.7.1.5 "><p id="p010519231116"><a name="p010519231116"></a><a name="p010519231116"></a>函数</p>
</td>
<td class="cellrowborder" valign="top" width="15.306938612277547%" headers="mcps1.1.7.1.6 "><p id="p8105523318"><a name="p8105523318"></a><a name="p8105523318"></a>1分钟</p>
</td>
</tr>
<tr id="row12924215714"><td class="cellrowborder" valign="top" width="17.956408718256352%" headers="mcps1.1.7.1.1 "><p id="p1995320433289"><a name="p1995320433289"></a><a name="p1995320433289"></a>rejectcount</p>
</td>
<td class="cellrowborder" valign="top" width="15.486902619476107%" headers="mcps1.1.7.1.2 "><p id="p1105823513"><a name="p1105823513"></a><a name="p1105823513"></a>被拒绝次数</p>
</td>
<td class="cellrowborder" valign="top" width="25.86482703459308%" headers="mcps1.1.7.1.3 "><p id="p161054231911"><a name="p161054231911"></a><a name="p161054231911"></a>该指标用于统计函数调用被拒绝次数。</p>
<p id="p6304153484817"><a name="p6304153484817"></a><a name="p6304153484817"></a>被拒绝次数是指并发请求太多，系统流控而被拒绝的请求次数。</p>
<p id="p18105223318"><a name="p18105223318"></a><a name="p18105223318"></a>单位：次</p>
</td>
<td class="cellrowborder" valign="top" width="14.057188562287543%" headers="mcps1.1.7.1.4 "><p id="p101051123217"><a name="p101051123217"></a><a name="p101051123217"></a>≥ 0 counts</p>
</td>
<td class="cellrowborder" valign="top" width="11.327734453109379%" headers="mcps1.1.7.1.5 "><p id="p0105142319119"><a name="p0105142319119"></a><a name="p0105142319119"></a>函数</p>
</td>
<td class="cellrowborder" valign="top" width="15.306938612277547%" headers="mcps1.1.7.1.6 "><p id="p161051623310"><a name="p161051623310"></a><a name="p161051623310"></a>1分钟</p>
</td>
</tr>
<tr id="row1192416154112"><td class="cellrowborder" valign="top" width="17.956408718256352%" headers="mcps1.1.7.1.1 "><p id="p1953164352816"><a name="p1953164352816"></a><a name="p1953164352816"></a>duration</p>
</td>
<td class="cellrowborder" valign="top" width="15.486902619476107%" headers="mcps1.1.7.1.2 "><p id="p3105142316112"><a name="p3105142316112"></a><a name="p3105142316112"></a>平均运行时间</p>
</td>
<td class="cellrowborder" valign="top" width="25.86482703459308%" headers="mcps1.1.7.1.3 "><p id="p1010519231015"><a name="p1010519231015"></a><a name="p1010519231015"></a>该指标用于统计函数调用平均运行时间。</p>
<p id="p610522315119"><a name="p610522315119"></a><a name="p610522315119"></a>单位：毫秒</p>
</td>
<td class="cellrowborder" valign="top" width="14.057188562287543%" headers="mcps1.1.7.1.4 "><p id="p41061323517"><a name="p41061323517"></a><a name="p41061323517"></a>≥ 0 ms</p>
</td>
<td class="cellrowborder" valign="top" width="11.327734453109379%" headers="mcps1.1.7.1.5 "><p id="p1610619231219"><a name="p1610619231219"></a><a name="p1610619231219"></a>函数</p>
</td>
<td class="cellrowborder" valign="top" width="15.306938612277547%" headers="mcps1.1.7.1.6 "><p id="p111061023412"><a name="p111061023412"></a><a name="p111061023412"></a>1分钟</p>
</td>
</tr>
<tr id="row119244151513"><td class="cellrowborder" valign="top" width="17.956408718256352%" headers="mcps1.1.7.1.1 "><p id="p495318439287"><a name="p495318439287"></a><a name="p495318439287"></a>maxDuration</p>
</td>
<td class="cellrowborder" valign="top" width="15.486902619476107%" headers="mcps1.1.7.1.2 "><p id="p1210610230117"><a name="p1210610230117"></a><a name="p1210610230117"></a>最大运行时间</p>
</td>
<td class="cellrowborder" valign="top" width="25.86482703459308%" headers="mcps1.1.7.1.3 "><p id="p101066231914"><a name="p101066231914"></a><a name="p101066231914"></a>该指标用于统计函数调用最大运行时间。</p>
<p id="p111069232117"><a name="p111069232117"></a><a name="p111069232117"></a>单位：毫秒</p>
</td>
<td class="cellrowborder" valign="top" width="14.057188562287543%" headers="mcps1.1.7.1.4 "><p id="p181061923512"><a name="p181061923512"></a><a name="p181061923512"></a>≥ 0 ms</p>
</td>
<td class="cellrowborder" valign="top" width="11.327734453109379%" headers="mcps1.1.7.1.5 "><p id="p2106423114"><a name="p2106423114"></a><a name="p2106423114"></a>函数</p>
</td>
<td class="cellrowborder" valign="top" width="15.306938612277547%" headers="mcps1.1.7.1.6 "><p id="p210617234115"><a name="p210617234115"></a><a name="p210617234115"></a>1分钟</p>
</td>
</tr>
<tr id="row1792431516119"><td class="cellrowborder" valign="top" width="17.956408718256352%" headers="mcps1.1.7.1.1 "><p id="p695314317287"><a name="p695314317287"></a><a name="p695314317287"></a>minDuration</p>
</td>
<td class="cellrowborder" valign="top" width="15.486902619476107%" headers="mcps1.1.7.1.2 "><p id="p01061123418"><a name="p01061123418"></a><a name="p01061123418"></a>最小运行时间</p>
</td>
<td class="cellrowborder" valign="top" width="25.86482703459308%" headers="mcps1.1.7.1.3 "><p id="p191066239119"><a name="p191066239119"></a><a name="p191066239119"></a>该指标用于统计函数最小运行时间。</p>
<p id="p31061123117"><a name="p31061123117"></a><a name="p31061123117"></a>单位：毫秒</p>
</td>
<td class="cellrowborder" valign="top" width="14.057188562287543%" headers="mcps1.1.7.1.4 "><p id="p16106223915"><a name="p16106223915"></a><a name="p16106223915"></a>≥ 0 ms</p>
</td>
<td class="cellrowborder" valign="top" width="11.327734453109379%" headers="mcps1.1.7.1.5 "><p id="p1410614235117"><a name="p1410614235117"></a><a name="p1410614235117"></a>函数</p>
</td>
<td class="cellrowborder" valign="top" width="15.306938612277547%" headers="mcps1.1.7.1.6 "><p id="p81069231117"><a name="p81069231117"></a><a name="p81069231117"></a>1分钟</p>
</td>
</tr>
</tbody>
</table>

## 维度<a name="section17346143012499"></a>

<a name="table076413085020"></a>
<table><thead align="left"><tr id="row876480165020"><th class="cellrowborder" valign="top" width="35.27%" id="mcps1.1.3.1.1"><p id="p167644010504"><a name="p167644010504"></a><a name="p167644010504"></a>key</p>
</th>
<th class="cellrowborder" valign="top" width="64.73%" id="mcps1.1.3.1.2"><p id="p176412020502"><a name="p176412020502"></a><a name="p176412020502"></a>value</p>
</th>
</tr>
</thead>
<tbody><tr id="row10764130185013"><td class="cellrowborder" valign="top" width="35.27%" headers="mcps1.1.3.1.1 "><p id="p376490115011"><a name="p376490115011"></a><a name="p376490115011"></a>package-functionname</p>
</td>
<td class="cellrowborder" valign="top" width="64.73%" headers="mcps1.1.3.1.2 "><p id="p111198624315"><a name="p111198624315"></a><a name="p111198624315"></a>应用名-函数名。</p>
<p id="p37641203506"><a name="p37641203506"></a><a name="p37641203506"></a>示例：default-myfunction_Python。</p>
</td>
</tr>
</tbody>
</table>

