# 创建Mapping<a name="ZH-CN_TOPIC_0115410427"></a>

## 功能介绍<a name="section51379511"></a>

创建一个触发器-工作流Mapping。

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   带有触发器的工作流不能创建触发器Mapping。  
>-   Worker触发器不能绑定到工作流上。  
>-   若触发器、工作流之间创建了Mapping，则必须先删除该Mapping才能删除相应触发器、工作流  

## URI<a name="section59762422"></a>

POST /v1.0/\{project\_id\}/trigger\_graph\_mappings

参数说明如[表1](#table13216186)所示。  

**表 1**  参数说明

<a name="table13216186"></a>
<table><thead align="left"><tr id="row19124697"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p5596611"><a name="p5596611"></a><a name="p5596611"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p50672366"><a name="p50672366"></a><a name="p50672366"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p4085285"><a name="p4085285"></a><a name="p4085285"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row62472706"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p27124415"><a name="p27124415"></a><a name="p27124415"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p49593988"><a name="p49593988"></a><a name="p49593988"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p42387016"><a name="p42387016"></a><a name="p42387016"></a>租户ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section990892"></a>

**请求参数**

请求参数如[表2](#table63351959)所示。

**表 2**  请求参数

<a name="table63351959"></a>
<table><thead align="left"><tr id="row15085294"><th class="cellrowborder" valign="top" width="20.84791520847915%" id="mcps1.2.6.1.1"><p id="p13949281"><a name="p13949281"></a><a name="p13949281"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.788521147885211%" id="mcps1.2.6.1.2"><p id="p56149948"><a name="p56149948"></a><a name="p56149948"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20.84791520847915%" id="mcps1.2.6.1.3"><p id="p51851944"><a name="p51851944"></a><a name="p51851944"></a><em id="i64014316"><a name="i64014316"></a><a name="i64014316"></a>参数类型</em></p>
</th>
<th class="cellrowborder" valign="top" width="35.99640035996401%" id="mcps1.2.6.1.4"><p id="p17777075"><a name="p17777075"></a><a name="p17777075"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="7.519248075192481%" id="mcps1.2.6.1.5"><p id="p14578630102655"><a name="p14578630102655"></a><a name="p14578630102655"></a>约束</p>
</th>
</tr>
</thead>
<tbody><tr id="row188376"><td class="cellrowborder" valign="top" width="20.84791520847915%" headers="mcps1.2.6.1.1 "><p id="p19071154163314"><a name="p19071154163314"></a><a name="p19071154163314"></a>trigger_urn</p>
</td>
<td class="cellrowborder" valign="top" width="14.788521147885211%" headers="mcps1.2.6.1.2 "><p id="p1259617163314"><a name="p1259617163314"></a><a name="p1259617163314"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.84791520847915%" headers="mcps1.2.6.1.3 "><p id="p34920141163314"><a name="p34920141163314"></a><a name="p34920141163314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.99640035996401%" headers="mcps1.2.6.1.4 "><p id="p22523334163314"><a name="p22523334163314"></a><a name="p22523334163314"></a>Mapping中触发器的URN</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.6.1.5 "><p id="p40018407102655"><a name="p40018407102655"></a><a name="p40018407102655"></a>-</p>
</td>
</tr>
<tr id="row49585950"><td class="cellrowborder" valign="top" width="20.84791520847915%" headers="mcps1.2.6.1.1 "><p id="p44947978163314"><a name="p44947978163314"></a><a name="p44947978163314"></a>graph_urn</p>
</td>
<td class="cellrowborder" valign="top" width="14.788521147885211%" headers="mcps1.2.6.1.2 "><p id="p16907640163314"><a name="p16907640163314"></a><a name="p16907640163314"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.84791520847915%" headers="mcps1.2.6.1.3 "><p id="p27341610163314"><a name="p27341610163314"></a><a name="p27341610163314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.99640035996401%" headers="mcps1.2.6.1.4 "><p id="p701652163314"><a name="p701652163314"></a><a name="p701652163314"></a>Mapping中工作流的URN</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.6.1.5 "><p id="p20265573102655"><a name="p20265573102655"></a><a name="p20265573102655"></a>-</p>
</td>
</tr>
<tr id="row53994596"><td class="cellrowborder" valign="top" width="20.84791520847915%" headers="mcps1.2.6.1.1 "><p id="p41742956163314"><a name="p41742956163314"></a><a name="p41742956163314"></a>enabled</p>
</td>
<td class="cellrowborder" valign="top" width="14.788521147885211%" headers="mcps1.2.6.1.2 "><p id="p25736256163314"><a name="p25736256163314"></a><a name="p25736256163314"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.84791520847915%" headers="mcps1.2.6.1.3 "><p id="p4261985163314"><a name="p4261985163314"></a><a name="p4261985163314"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="35.99640035996401%" headers="mcps1.2.6.1.4 "><p id="p92701526535"><a name="p92701526535"></a><a name="p92701526535"></a>创建成功之后是否立即启用该Mapping，不指定即使用默认值false</p>
</td>
<td class="cellrowborder" valign="top" width="7.519248075192481%" headers="mcps1.2.6.1.5 "><p id="p30898727102655"><a name="p30898727102655"></a><a name="p30898727102655"></a>-</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section8918034"></a>

**响应参数**

响应参数如[表3](#table77026151513)所示。  

**表 3**  响应参数

<a name="table77026151513"></a>
<table><thead align="left"><tr id="row1970213119159"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p117023121517"><a name="p117023121517"></a><a name="p117023121517"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p970211161518"><a name="p970211161518"></a><a name="p970211161518"></a><em id="i157021515159"><a name="i157021515159"></a><a name="i157021515159"></a>参数类型</em></p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p970231141517"><a name="p970231141517"></a><a name="p970231141517"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1770212116155"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p6653042416343"><a name="p6653042416343"></a><a name="p6653042416343"></a>response</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p2025527216343"><a name="p2025527216343"></a><a name="p2025527216343"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p214339116343"><a name="p214339116343"></a><a name="p214339116343"></a>触发器Mapping的ID</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>触发器Mapping的ID由工作流URN的最后一段以及触发器URN的最后一段以冒号连接组成。  

## 示例<a name="section793794610303"></a>

**请求示例**

```
{
    "trigger_urn": "urn:fgs:cn-north-1:7aad83af3e8d42e99ac194e8419e2c9b:trigger:Worker_WorkRequest_Worker-test-event2axe02567d3-9e50-4b5a-48f4-8263cd9f85e7_1505960298",
    "graph_urn": "urn:fgs:cn-north-1:7aad83af3e8d42e99ac194e8419e2c9b:graph:workflow-2d98",
    "enabled": true
}
```

**响应示例**：

```
{
    "response": "extTriggerTestGraph:SMN_HelloWorldTopic_xxx5c8bfe0e-104a-4ebf-4a3a-e12bfbf11e60_1506757403"
}

```

## 返回值<a name="section370272717123"></a>

状态码请参见[状态码](状态码.md)。

