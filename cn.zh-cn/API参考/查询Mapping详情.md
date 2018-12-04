# 查询Mapping详情<a name="functiongraph_06_0740"></a>

## 功能介绍<a name="section51379511"></a>

查询指定的触发器Mapping的相关信息。

## URI<a name="section59762422"></a>

GET /v1.0/\{project\_id\}/trigger\_graph\_mappings/\{mapping\_id\}

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
<tr id="row33581998171734"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p7509671171738"><a name="p7509671171738"></a><a name="p7509671171738"></a>mapping_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p4303640171738"><a name="p4303640171738"></a><a name="p4303640171738"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p13050598171738"><a name="p13050598171738"></a><a name="p13050598171738"></a>Mapping的ID</p>
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
    <table><thead align="left"><tr id="row1970213119159"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p12178651171823"><a name="p12178651171823"></a><a name="p12178651171823"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p46946666171823"><a name="p46946666171823"></a><a name="p46946666171823"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p44583626171823"><a name="p44583626171823"></a><a name="p44583626171823"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1770212116155"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p52745500171823"><a name="p52745500171823"></a><a name="p52745500171823"></a>trigger_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p44527069171823"><a name="p44527069171823"></a><a name="p44527069171823"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p46652297171823"><a name="p46652297171823"></a><a name="p46652297171823"></a>触发器URN</p>
    </td>
    </tr>
    <tr id="row7927001171813"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p52440036171823"><a name="p52440036171823"></a><a name="p52440036171823"></a>graph_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p19784536171823"><a name="p19784536171823"></a><a name="p19784536171823"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p61629883171823"><a name="p61629883171823"></a><a name="p61629883171823"></a>工作流URN</p>
    </td>
    </tr>
    <tr id="row36841490171820"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p32355125171823"><a name="p32355125171823"></a><a name="p32355125171823"></a>enabled</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p3519450171823"><a name="p3519450171823"></a><a name="p3519450171823"></a>Bool</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p15542709171823"><a name="p15542709171823"></a><a name="p15542709171823"></a>Mapping是否被启用</p>
    </td>
    </tr>
    <tr id="row13766751171818"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p56345869171823"><a name="p56345869171823"></a><a name="p56345869171823"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p612709171823"><a name="p612709171823"></a><a name="p612709171823"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p44011894171823"><a name="p44011894171823"></a><a name="p44011894171823"></a>Mapping的ID</p>
    </td>
    </tr>
    <tr id="row483657411498"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p1243436311498"><a name="p1243436311498"></a><a name="p1243436311498"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p45845724114917"><a name="p45845724114917"></a><a name="p45845724114917"></a>Int64</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p846083311498"><a name="p846083311498"></a><a name="p846083311498"></a>Mapping的创建时间</p>
    </td>
    </tr>
    </tbody>
    </table>

    **响应样例**：

    ```
    {
        "trigger_urn": "urn:fgs:cn-north-1:7aad83af3e8d42e99ac194e8419e2c9b:trigger:Worker_WorkRequest_Worker-test-event2axe02567d3-9e50-4b5a-48f4-8263cd9f85e7_1505960298",
        "graph_urn": "urn:fgs:cn-north-1:7aad83af3e8d42e99ac194e8419e2c9b:graph:workflow-2d98",
        "enabled": true,
        "id": "workflow-2d98:Worker_WorkRequest_Worker-test-event2axe02567d3-9e50-4b5a-48f4-8263cd9f85e7_1505960298",
        "created_at": 1513820002
    } 
    ```


-   异常响应

    请参考[异常响应](请求结果.md#section88241732388)。


## 返回值<a name="section370272717123"></a>

请参考[返回值](请求结果.md#section20306194210386)。

