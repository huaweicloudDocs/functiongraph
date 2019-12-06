# 启用、禁用Mapping<a name="ZH-CN_TOPIC_0115410468"></a>

## 功能介绍<a name="section51379511"></a>

启用或禁用一个触发器-工作流Mapping。

## URI<a name="section59762422"></a>

PUT /v1.0/\{project\_id\}/trigger\_graph\_mappings/\{mapping\_id\}

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
<tr id="row32372117160"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p1824089917164"><a name="p1824089917164"></a><a name="p1824089917164"></a>mapping_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p111783317164"><a name="p111783317164"></a><a name="p111783317164"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p2343568517164"><a name="p2343568517164"></a><a name="p2343568517164"></a>触发器Mapping的ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section990892"></a>

**请求参数**

请求参数如[表2](#table63351959)所示。

**表 2**  请求参数

<a name="table63351959"></a>
<table><thead align="left"><tr id="row15085294"><th class="cellrowborder" valign="top" width="22.72772722727727%" id="mcps1.2.5.1.1"><p id="p13949281"><a name="p13949281"></a><a name="p13949281"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.66833316668333%" id="mcps1.2.5.1.2"><p id="p56149948"><a name="p56149948"></a><a name="p56149948"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="22.72772722727727%" id="mcps1.2.5.1.3"><p id="p51851944"><a name="p51851944"></a><a name="p51851944"></a><em id="i64014316"><a name="i64014316"></a><a name="i64014316"></a>参数类型</em></p>
</th>
<th class="cellrowborder" valign="top" width="37.876212378762126%" id="mcps1.2.5.1.4"><p id="p17777075"><a name="p17777075"></a><a name="p17777075"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row53994596"><td class="cellrowborder" valign="top" width="22.72772722727727%" headers="mcps1.2.5.1.1 "><p id="p41742956163314"><a name="p41742956163314"></a><a name="p41742956163314"></a>enabled</p>
</td>
<td class="cellrowborder" valign="top" width="16.66833316668333%" headers="mcps1.2.5.1.2 "><p id="p25736256163314"><a name="p25736256163314"></a><a name="p25736256163314"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="22.72772722727727%" headers="mcps1.2.5.1.3 "><p id="p4261985163314"><a name="p4261985163314"></a><a name="p4261985163314"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="37.876212378762126%" headers="mcps1.2.5.1.4 "><p id="p19979367163314"><a name="p19979367163314"></a><a name="p19979367163314"></a>是否启用该Mapping</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section8918034"></a>

**响应参数**

响应参数如[表3](#table4105182711362)所示。  

**表 3**  响应参数

<a name="table4105182711362"></a>
<table><thead align="left"><tr id="row2176336011362"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.4.1.1"><p id="p1800170711362"><a name="p1800170711362"></a><a name="p1800170711362"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="31.313131313131308%" id="mcps1.2.4.1.2"><p id="p4885216711362"><a name="p4885216711362"></a><a name="p4885216711362"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.2.4.1.3"><p id="p6471145111362"><a name="p6471145111362"></a><a name="p6471145111362"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row713620811362"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p4116199811362"><a name="p4116199811362"></a><a name="p4116199811362"></a>response</p>
</td>
<td class="cellrowborder" valign="top" width="31.313131313131308%" headers="mcps1.2.4.1.2 "><p id="p4578751611362"><a name="p4578751611362"></a><a name="p4578751611362"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.4.1.3 "><p id="p1780128211362"><a name="p1780128211362"></a><a name="p1780128211362"></a>此次操作的返回信息</p>
</td>
</tr>
</tbody>
</table>

## 示例<a name="section2438183083217"></a>

**请求示例**

```
{
    "enabled": true
}
```

**响应示例**

```
{
    "response": "OK"
}
```

## 返回值<a name="section370272717123"></a>

状态码请参见[状态码](状态码.md)。

