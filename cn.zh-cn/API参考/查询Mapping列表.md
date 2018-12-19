# 查询Mapping列表<a name="functiongraph_06_0750"></a>

## 功能介绍<a name="section51379511"></a>

依据输入的查询参数，查询多个触发器Mapping，返回所需触发器Mapping详细信息列表。

## URI<a name="section59762422"></a>

GET/v1.0/\{project\_id\}/trigger\_graph\_mappings?graph\_urn=xxx&trigger\_urn=xxx

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
<tr id="row6631505171946"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p32830679171950"><a name="p32830679171950"></a><a name="p32830679171950"></a>graph_urn</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p42039361171950"><a name="p42039361171950"></a><a name="p42039361171950"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p49745071171950"><a name="p49745071171950"></a><a name="p49745071171950"></a>工作流URN</p>
</td>
</tr>
<tr id="row31272958171945"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p25370587171950"><a name="p25370587171950"></a><a name="p25370587171950"></a>trigger_urn</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p41751684171950"><a name="p41751684171950"></a><a name="p41751684171950"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p26443213171950"><a name="p26443213171950"></a><a name="p26443213171950"></a>触发器URN</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section990892"></a>

不涉及

## 响应<a name="section8918034"></a>

-   正常响应

    **响应参数**

    响应参数如[表2](#table77026151513)所示。

    **表 2**  响应参数

    <a name="table77026151513"></a>
    <table><thead align="left"><tr id="row1970213119159"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p4544341312645"><a name="p4544341312645"></a><a name="p4544341312645"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p5703784512645"><a name="p5703784512645"></a><a name="p5703784512645"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p5666271312645"><a name="p5666271312645"></a><a name="p5666271312645"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1770212116155"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p4806497512645"><a name="p4806497512645"></a><a name="p4806497512645"></a>mappings</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p94888012645"><a name="p94888012645"></a><a name="p94888012645"></a>列表数据结构</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p2064551912645"><a name="p2064551912645"></a><a name="p2064551912645"></a>满足查询条件的Mapping列表，具体请参见<a href="#table32073546172118">表3</a></p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  mappings列表数据结构说明

    <a name="table32073546172118"></a>
    <table><thead align="left"><tr id="row16156794172118"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p33631909172118"><a name="p33631909172118"></a><a name="p33631909172118"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p39830113172118"><a name="p39830113172118"></a><a name="p39830113172118"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p5013717172118"><a name="p5013717172118"></a><a name="p5013717172118"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3457962172118"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p11659528172118"><a name="p11659528172118"></a><a name="p11659528172118"></a>trigger_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p4897686172118"><a name="p4897686172118"></a><a name="p4897686172118"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p13643360172118"><a name="p13643360172118"></a><a name="p13643360172118"></a>触发器URN</p>
    </td>
    </tr>
    <tr id="row55681379172118"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p13897842172118"><a name="p13897842172118"></a><a name="p13897842172118"></a>graph_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p51983442172118"><a name="p51983442172118"></a><a name="p51983442172118"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p46530436172118"><a name="p46530436172118"></a><a name="p46530436172118"></a>工作流URN</p>
    </td>
    </tr>
    <tr id="row16120740172118"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p30711525172118"><a name="p30711525172118"></a><a name="p30711525172118"></a>enabled</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p4605591172118"><a name="p4605591172118"></a><a name="p4605591172118"></a>Bool</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p2032879172118"><a name="p2032879172118"></a><a name="p2032879172118"></a>Mapping是否被启用</p>
    </td>
    </tr>
    <tr id="row18295916172118"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p5574240172118"><a name="p5574240172118"></a><a name="p5574240172118"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p48860259172118"><a name="p48860259172118"></a><a name="p48860259172118"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p51431587172118"><a name="p51431587172118"></a><a name="p51431587172118"></a>Mapping的ID</p>
    </td>
    </tr>
    <tr id="row5601782293144"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p4114970193144"><a name="p4114970193144"></a><a name="p4114970193144"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p4479150593144"><a name="p4479150593144"></a><a name="p4479150593144"></a>Int64</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p423332293144"><a name="p423332293144"></a><a name="p423332293144"></a>Mapping的创建时间</p>
    </td>
    </tr>
    </tbody>
    </table>

    **响应样例**：

    ```
    {
        "mappings": [
            {
                "trigger_urn": "urn:fgs:cn-north-1:9800716a0c604a8690963103a85754f0:trigger:SMN_pzwtopic_smnevt52c820c8-f842-4dd6-5941-c4752e5887a8_1506657391",
                "graph_urn": "urn:fgs:cn-north-1:9800716a0c604a8690963103a85754f0:graph:EMF",
                "enabled": true,
                "id": "EMF:SMN_pzwtopic_smnevt52c820c8-f842-4dd6-5941-c4752e5887a8_1506657391",
                "created_at": 1513820002
            },
            {
                "trigger_urn": "urn:fgs:cn-north-1:9800716a0c604a8690963103a85754f0:trigger:SMN_pzwtopic_extTriggerEvt38953093-52b6-4d6b-64c4-37a6f064e479_1506348617",
                "graph_urn": "urn:fgs:cn-north-1:9800716a0c604a8690963103a85754f0:graph:extTriggerTestGraph",
                "enabled": true,
                "id": "extTriggerTestGraph:SMN_pzwtopic_extTriggerEvt38953093-52b6-4d6b-64c4-37a6f064e479_1506348617",
                "created_at": 1513820001
            },
            {
                "trigger_urn": "urn:fgs:cn-north-1:9800716a0c604a8690963103a85754f0:trigger:SMN_pzwtopic_smnevt52c820c8-f842-4dd6-5941-c4752e5887a8_1506657391",
                "graph_urn": "urn:fgs:cn-north-1:9800716a0c604a8690963103a85754f0:graph:workflow-4d46",
                "enabled": true,
                "id": "workflow-4d46:SMN_pzwtopic_smnevt52c820c8-f842-4dd6-5941-c4752e5887a8_1506657391",           
                "created_at": 1513820000
            }
        ]
    }
    ```


-   异常响应

    请参考[异常响应](请求结果.md#section88241732388)。


## 返回值<a name="section370272717123"></a>

请参考[返回值](请求结果.md#section20306194210386)。

