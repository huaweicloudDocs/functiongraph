# 删除Mapping<a name="functiongraph_06_0720"></a>

## 功能介绍<a name="section51379511"></a>

删除一个触发器-工作流Mapping。

## URI<a name="section59762422"></a>

DELETE /v1.0/\{project\_id\}/trigger\_graph\_mappings/\{mapping\_id\}

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
<tr id="row19238864171332"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p50793202171337"><a name="p50793202171337"></a><a name="p50793202171337"></a>mapping_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p20608698171337"><a name="p20608698171337"></a><a name="p20608698171337"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p42263690171348"><a name="p42263690171348"></a><a name="p42263690171348"></a>触发器Mapping的ID</p>
</td>
</tr>
</tbody>
</table>

## 请求<a name="section990892"></a>

不涉及

## 响应<a name="section8918034"></a>

-   正常响应

    **响应参数**

    响应参数如[表2](#table394445163918)所示。 

    **表 2**  响应参数

    <a name="table394445163918"></a>
    <table><thead align="left"><tr id="row5944851163912"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.4.1.1"><p id="p7944165193912"><a name="p7944165193912"></a><a name="p7944165193912"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="31.313131313131308%" id="mcps1.2.4.1.2"><p id="p494413519391"><a name="p494413519391"></a><a name="p494413519391"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.2.4.1.3"><p id="p159441351193918"><a name="p159441351193918"></a><a name="p159441351193918"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row149441251173914"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.4.1.1 "><p id="p159441151143920"><a name="p159441151143920"></a><a name="p159441151143920"></a>response</p>
    </td>
    <td class="cellrowborder" valign="top" width="31.313131313131308%" headers="mcps1.2.4.1.2 "><p id="p994485116397"><a name="p994485116397"></a><a name="p994485116397"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.2.4.1.3 "><p id="p18944951193920"><a name="p18944951193920"></a><a name="p18944951193920"></a>此次操作的返回信息</p>
    </td>
    </tr>
    </tbody>
    </table>

    **响应示例**

    ```
    {
        "response": "OK"
    }
    ```


-   异常响应

    请参考[异常响应](请求结果.md#section88241732388)。


## 返回值<a name="section370272717123"></a>

请参考[返回值](请求结果.md#section20306194210386)。

