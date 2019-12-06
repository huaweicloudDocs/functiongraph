# 模拟事件消息触发event state<a name="ZH-CN_TOPIC_0115410464"></a>

## 功能介绍<a name="section5238527"></a>

模拟一个事件消息，触发指定的event state。

## URI<a name="section47146745"></a>

POST /v1.0/\{project\_id\}/cloud\_graphs/\{graph\_urn\}/executions/\{execution\_urn\}/event\_test

参数说明如[表1](#table30785969)所示：  

**表 1**  参数说明

<a name="table30785969"></a>
<table><thead align="left"><tr id="row53868469"><th class="cellrowborder" valign="top" width="23.23%" id="mcps1.2.4.1.1"><p id="p1269896"><a name="p1269896"></a><a name="p1269896"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="11.110000000000001%" id="mcps1.2.4.1.2"><p id="p35752731"><a name="p35752731"></a><a name="p35752731"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="p10290070"><a name="p10290070"></a><a name="p10290070"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row28189346"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p1635686"><a name="p1635686"></a><a name="p1635686"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.4.1.2 "><p id="p65381771"><a name="p65381771"></a><a name="p65381771"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p61432121"><a name="p61432121"></a><a name="p61432121"></a>租户ID</p>
</td>
</tr>
<tr id="row16018178"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p22404047"><a name="p22404047"></a><a name="p22404047"></a>graph_urn</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.4.1.2 "><p id="p2788537"><a name="p2788537"></a><a name="p2788537"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p2006050514524"><a name="p2006050514524"></a><a name="p2006050514524"></a>工作流的URN</p>
</td>
</tr>
<tr id="row19577827"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.4.1.1 "><p id="p42300179"><a name="p42300179"></a><a name="p42300179"></a>execution_urn</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.4.1.2 "><p id="p3762492"><a name="p3762492"></a><a name="p3762492"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p4268161114530"><a name="p4268161114530"></a><a name="p4268161114530"></a>运行实例的URN</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section21667523"></a>

**请求参数**

请求参数如[表2](#table33967256)所示。  

**表 2**  请求参数

<a name="table33967256"></a>
<table><thead align="left"><tr id="row4581796"><th class="cellrowborder" valign="top" width="17.191719171917192%" id="mcps1.2.6.1.1"><p id="p35581233"><a name="p35581233"></a><a name="p35581233"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.191719171917192%" id="mcps1.2.6.1.2"><p id="p63507614"><a name="p63507614"></a><a name="p63507614"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.391839183918393%" id="mcps1.2.6.1.3"><p id="p43843091"><a name="p43843091"></a><a name="p43843091"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="30.683068306830684%" id="mcps1.2.6.1.4"><p id="p61629497"><a name="p61629497"></a><a name="p61629497"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="16.541654165416542%" id="mcps1.2.6.1.5"><p id="p34145971103220"><a name="p34145971103220"></a><a name="p34145971103220"></a>约束</p>
</th>
</tr>
</thead>
<tbody><tr id="row20228022"><td class="cellrowborder" valign="top" width="17.191719171917192%" headers="mcps1.2.6.1.1 "><p id="p27857118"><a name="p27857118"></a><a name="p27857118"></a>input</p>
</td>
<td class="cellrowborder" valign="top" width="17.191719171917192%" headers="mcps1.2.6.1.2 "><p id="p41834070"><a name="p41834070"></a><a name="p41834070"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.391839183918393%" headers="mcps1.2.6.1.3 "><p id="p33116486"><a name="p33116486"></a><a name="p33116486"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30.683068306830684%" headers="mcps1.2.6.1.4 "><p id="p49836563"><a name="p49836563"></a><a name="p49836563"></a>为实例运行提供的输入参数。</p>
</td>
<td class="cellrowborder" valign="top" width="16.541654165416542%" headers="mcps1.2.6.1.5 "><p id="p14360230103220"><a name="p14360230103220"></a><a name="p14360230103220"></a>必须是包含JSON格式的内容的String长度最小为1，最长为32768</p>
</td>
</tr>
<tr id="row24959482"><td class="cellrowborder" valign="top" width="17.191719171917192%" headers="mcps1.2.6.1.1 "><p id="p8452189"><a name="p8452189"></a><a name="p8452189"></a>trigger_urn</p>
</td>
<td class="cellrowborder" valign="top" width="17.191719171917192%" headers="mcps1.2.6.1.2 "><p id="p13538688"><a name="p13538688"></a><a name="p13538688"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.391839183918393%" headers="mcps1.2.6.1.3 "><p id="p22891915"><a name="p22891915"></a><a name="p22891915"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30.683068306830684%" headers="mcps1.2.6.1.4 "><p id="p45208163"><a name="p45208163"></a><a name="p45208163"></a>触发器URN。</p>
</td>
<td class="cellrowborder" valign="top" width="16.541654165416542%" headers="mcps1.2.6.1.5 "><p id="p22328019103220"><a name="p22328019103220"></a><a name="p22328019103220"></a>-</p>
</td>
</tr>
<tr id="row6298672"><td class="cellrowborder" valign="top" width="17.191719171917192%" headers="mcps1.2.6.1.1 "><p id="p40430446"><a name="p40430446"></a><a name="p40430446"></a>invocation_mode</p>
</td>
<td class="cellrowborder" valign="top" width="17.191719171917192%" headers="mcps1.2.6.1.2 "><p id="p53640668"><a name="p53640668"></a><a name="p53640668"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.391839183918393%" headers="mcps1.2.6.1.3 "><p id="p49926818"><a name="p49926818"></a><a name="p49926818"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30.683068306830684%" headers="mcps1.2.6.1.4 "><p id="p23646388"><a name="p23646388"></a><a name="p23646388"></a>调用模式，sync标识同步调用，需等event state运行返回结果；async标识异步调用，无需等待结果返回。</p>
</td>
<td class="cellrowborder" valign="top" width="16.541654165416542%" headers="mcps1.2.6.1.5 "><p id="p63739104103220"><a name="p63739104103220"></a><a name="p63739104103220"></a>-</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section60789982"></a>

**响应参数**

响应参数如[表3](#table60801917)所示。  

**表 3**  响应参数

<a name="table60801917"></a>
<table><thead align="left"><tr id="row49159881"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.2.4.1.1"><p id="p22527411"><a name="p22527411"></a><a name="p22527411"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="27.55%" id="mcps1.2.4.1.2"><p id="p12781022"><a name="p12781022"></a><a name="p12781022"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="51.019999999999996%" id="mcps1.2.4.1.3"><p id="p28629874"><a name="p28629874"></a><a name="p28629874"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row37318421"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.2.4.1.1 "><p id="p306190049371"><a name="p306190049371"></a><a name="p306190049371"></a>response</p>
</td>
<td class="cellrowborder" valign="top" width="27.55%" headers="mcps1.2.4.1.2 "><p id="p146852545217"><a name="p146852545217"></a><a name="p146852545217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="51.019999999999996%" headers="mcps1.2.4.1.3 "><p id="p1368112515212"><a name="p1368112515212"></a><a name="p1368112515212"></a>触发器触发后返回的结果</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section1625911216433"></a>

**请求示例**

```
{
    "trigger_urn": "urn:fgs:cn-north-1:9800716a0c604a8690963103a85754f0:execution:workflow-8f84:e1:ae0d3e648af440af5828696f16f0d1b4", 
    "input": "{\"in\":\"0123\"}", 
    "invocation_mode": "sync"
}
```

**响应示例**

```
{
    "response": "{\"in\":\"0123\",\"workItem\":\"{\\\"workItem\\\":\\\"123456789\\\"}\"}"
}
```

## 返回值<a name="section10238932"></a>

状态码请参见[状态码](状态码.md)。

