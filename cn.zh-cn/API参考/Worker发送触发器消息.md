# Worker发送触发器消息<a name="functiongraph_06_1010"></a>

## 功能介绍<a name="section55493137"></a>

Worker事件源向FunctionGraph服务发送触发器消息。

## URI<a name="section29676185"></a>

POST /v1.0/\{project\_id\}/worker\_messages

参数说明如[表1](#table47304076)所示。  

**表 1**  参数说明

<a name="table47304076"></a>
<table><thead align="left"><tr id="row9638516"><th class="cellrowborder" valign="top" width="17.169999999999998%" id="mcps1.2.4.1.1"><p id="p42522357"><a name="p42522357"></a><a name="p42522357"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.169999999999998%" id="mcps1.2.4.1.2"><p id="p21758931"><a name="p21758931"></a><a name="p21758931"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="p17642997"><a name="p17642997"></a><a name="p17642997"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row19796676"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.4.1.1 "><p id="p60026919"><a name="p60026919"></a><a name="p60026919"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.4.1.2 "><p id="p30342279"><a name="p30342279"></a><a name="p30342279"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p41805515"><a name="p41805515"></a><a name="p41805515"></a>租户ID</p>
</td>
</tr>
</tbody>
</table>

## 消息头<a name="section65759080"></a>

<a name="table43595579"></a>
<table><thead align="left"><tr id="row6047043"><th class="cellrowborder" valign="top" width="19.59%" id="mcps1.1.5.1.1"><p id="p20048509"><a name="p20048509"></a><a name="p20048509"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="26.8%" id="mcps1.1.5.1.2"><p id="p13316560"><a name="p13316560"></a><a name="p13316560"></a>描述</p>
</th>
<th class="cellrowborder" valign="top" width="19.59%" id="mcps1.1.5.1.3"><p id="p4899555"><a name="p4899555"></a><a name="p4899555"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="34.02%" id="mcps1.1.5.1.4"><p id="p61319646"><a name="p61319646"></a><a name="p61319646"></a>示例</p>
</th>
</tr>
</thead>
<tbody><tr id="row835434"><td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.1.5.1.1 "><p id="p561326"><a name="p561326"></a><a name="p561326"></a>X-FGS-EVENT-TYPE</p>
</td>
<td class="cellrowborder" valign="top" width="26.8%" headers="mcps1.1.5.1.2 "><p id="p45467475"><a name="p45467475"></a><a name="p45467475"></a>触发器类型</p>
</td>
<td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.1.5.1.3 "><p id="p58986881"><a name="p58986881"></a><a name="p58986881"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="34.02%" headers="mcps1.1.5.1.4 "><p id="p10037349141639"><a name="p10037349141639"></a><a name="p10037349141639"></a>workrequest</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>支持的触发器类型为：\{workrequest,heartbeat,worksuccess,workfailure\}。  

## 请求<a name="section28496157141456"></a>

不同的事件源的发送触发器消息请求中携带的消息结构不同。

-   Worker触发器消息参数说明

    **表 2**  WorkerRequest触发器消息

    <a name="table18979904141712"></a>
    <table><thead align="left"><tr id="row54970291141712"><th class="cellrowborder" valign="top" width="15.291529152915292%" id="mcps1.2.6.1.1"><p id="p23408549141712"><a name="p23408549141712"></a><a name="p23408549141712"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.291529152915292%" id="mcps1.2.6.1.2"><p id="p17044332141712"><a name="p17044332141712"></a><a name="p17044332141712"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="27.412741274127413%" id="mcps1.2.6.1.3"><p id="p38413680141712"><a name="p38413680141712"></a><a name="p38413680141712"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.52245224522452%" id="mcps1.2.6.1.4"><p id="p24500376141712"><a name="p24500376141712"></a><a name="p24500376141712"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.481748174817483%" id="mcps1.2.6.1.5"><p id="p24742675103311"><a name="p24742675103311"></a><a name="p24742675103311"></a>约束</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row38373453141712"><td class="cellrowborder" valign="top" width="15.291529152915292%" headers="mcps1.2.6.1.1 "><p id="p21241974141712"><a name="p21241974141712"></a><a name="p21241974141712"></a>trigger_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.291529152915292%" headers="mcps1.2.6.1.2 "><p id="p42878332141712"><a name="p42878332141712"></a><a name="p42878332141712"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.412741274127413%" headers="mcps1.2.6.1.3 "><p id="p50592838141712"><a name="p50592838141712"></a><a name="p50592838141712"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.52245224522452%" headers="mcps1.2.6.1.4 "><p id="p4379196141712"><a name="p4379196141712"></a><a name="p4379196141712"></a>触发器ID</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.481748174817483%" headers="mcps1.2.6.1.5 "><p id="p57999663103311"><a name="p57999663103311"></a><a name="p57999663103311"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  Heartbeat触发器消息

    <a name="table19170632141712"></a>
    <table><thead align="left"><tr id="row20419353141712"><th class="cellrowborder" valign="top" width="15.290000000000001%" id="mcps1.2.6.1.1"><p id="p43354863141712"><a name="p43354863141712"></a><a name="p43354863141712"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.290000000000001%" id="mcps1.2.6.1.2"><p id="p22083014141712"><a name="p22083014141712"></a><a name="p22083014141712"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="27.41%" id="mcps1.2.6.1.3"><p id="p43893701141712"><a name="p43893701141712"></a><a name="p43893701141712"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.9%" id="mcps1.2.6.1.4"><p id="p65728917141712"><a name="p65728917141712"></a><a name="p65728917141712"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.11%" id="mcps1.2.6.1.5"><p id="p17531621103316"><a name="p17531621103316"></a><a name="p17531621103316"></a>约束</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row22442078141712"><td class="cellrowborder" valign="top" width="15.290000000000001%" headers="mcps1.2.6.1.1 "><p id="p5868999141712"><a name="p5868999141712"></a><a name="p5868999141712"></a>trigger_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.290000000000001%" headers="mcps1.2.6.1.2 "><p id="p5626872141712"><a name="p5626872141712"></a><a name="p5626872141712"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.41%" headers="mcps1.2.6.1.3 "><p id="p53123482141712"><a name="p53123482141712"></a><a name="p53123482141712"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.9%" headers="mcps1.2.6.1.4 "><p id="p8034772141712"><a name="p8034772141712"></a><a name="p8034772141712"></a>触发器ID</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.11%" headers="mcps1.2.6.1.5 "><p id="p10775231103316"><a name="p10775231103316"></a><a name="p10775231103316"></a>-</p>
    </td>
    </tr>
    <tr id="row5204090141712"><td class="cellrowborder" valign="top" width="15.290000000000001%" headers="mcps1.2.6.1.1 "><p id="p18878156141712"><a name="p18878156141712"></a><a name="p18878156141712"></a>task_token</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.290000000000001%" headers="mcps1.2.6.1.2 "><p id="p52735691141712"><a name="p52735691141712"></a><a name="p52735691141712"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="27.41%" headers="mcps1.2.6.1.3 "><p id="p43732574141712"><a name="p43732574141712"></a><a name="p43732574141712"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.9%" headers="mcps1.2.6.1.4 "><p id="p52677614141712"><a name="p52677614141712"></a><a name="p52677614141712"></a>任务token</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.11%" headers="mcps1.2.6.1.5 "><p id="p378546103316"><a name="p378546103316"></a><a name="p378546103316"></a>-</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  WorkSuccess触发器消息

    <a name="table39028322141712"></a>
    <table><thead align="left"><tr id="row32138488141712"><th class="cellrowborder" valign="top" width="15.65%" id="mcps1.2.6.1.1"><p id="p53080768141712"><a name="p53080768141712"></a><a name="p53080768141712"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.65%" id="mcps1.2.6.1.2"><p id="p4574936141712"><a name="p4574936141712"></a><a name="p4574936141712"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.99%" id="mcps1.2.6.1.3"><p id="p35025512141712"><a name="p35025512141712"></a><a name="p35025512141712"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.23%" id="mcps1.2.6.1.4"><p id="p18494233141712"><a name="p18494233141712"></a><a name="p18494233141712"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.48%" id="mcps1.2.6.1.5"><p id="p58995499103324"><a name="p58995499103324"></a><a name="p58995499103324"></a>约束</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row21637906141712"><td class="cellrowborder" valign="top" width="15.65%" headers="mcps1.2.6.1.1 "><p id="p7839996141712"><a name="p7839996141712"></a><a name="p7839996141712"></a>trigger_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.65%" headers="mcps1.2.6.1.2 "><p id="p31059967141712"><a name="p31059967141712"></a><a name="p31059967141712"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.99%" headers="mcps1.2.6.1.3 "><p id="p32829378141712"><a name="p32829378141712"></a><a name="p32829378141712"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.23%" headers="mcps1.2.6.1.4 "><p id="p41933933141712"><a name="p41933933141712"></a><a name="p41933933141712"></a>触发器ID。</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.2.6.1.5 "><p id="p13906094103324"><a name="p13906094103324"></a><a name="p13906094103324"></a>-</p>
    </td>
    </tr>
    <tr id="row41861081141712"><td class="cellrowborder" valign="top" width="15.65%" headers="mcps1.2.6.1.1 "><p id="p35304437141712"><a name="p35304437141712"></a><a name="p35304437141712"></a>task_token</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.65%" headers="mcps1.2.6.1.2 "><p id="p41087116141712"><a name="p41087116141712"></a><a name="p41087116141712"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.99%" headers="mcps1.2.6.1.3 "><p id="p39722120141712"><a name="p39722120141712"></a><a name="p39722120141712"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.23%" headers="mcps1.2.6.1.4 "><p id="p63375185141712"><a name="p63375185141712"></a><a name="p63375185141712"></a>任务token。</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.2.6.1.5 "><p id="p52651801103324"><a name="p52651801103324"></a><a name="p52651801103324"></a>-</p>
    </td>
    </tr>
    <tr id="row33505758141712"><td class="cellrowborder" valign="top" width="15.65%" headers="mcps1.2.6.1.1 "><p id="p29611844141712"><a name="p29611844141712"></a><a name="p29611844141712"></a>result</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.65%" headers="mcps1.2.6.1.2 "><p id="p49749163141712"><a name="p49749163141712"></a><a name="p49749163141712"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.99%" headers="mcps1.2.6.1.3 "><p id="p3150394141712"><a name="p3150394141712"></a><a name="p3150394141712"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.23%" headers="mcps1.2.6.1.4 "><p id="p53855386141712"><a name="p53855386141712"></a><a name="p53855386141712"></a>任务执行返回值</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.48%" headers="mcps1.2.6.1.5 "><p id="p36937493103324"><a name="p36937493103324"></a><a name="p36937493103324"></a>JSON格式数据，长度1-32768</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 5**  WorkFailure触发器消息

    <a name="table210163141712"></a>
    <table><thead align="left"><tr id="row47081433141712"><th class="cellrowborder" valign="top" width="15.65%" id="mcps1.2.6.1.1"><p id="p55499767141712"><a name="p55499767141712"></a><a name="p55499767141712"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.65%" id="mcps1.2.6.1.2"><p id="p66296153141712"><a name="p66296153141712"></a><a name="p66296153141712"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.99%" id="mcps1.2.6.1.3"><p id="p1279336141712"><a name="p1279336141712"></a><a name="p1279336141712"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.42%" id="mcps1.2.6.1.4"><p id="p36517387141712"><a name="p36517387141712"></a><a name="p36517387141712"></a>说明</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.29%" id="mcps1.2.6.1.5"><p id="p12349278103340"><a name="p12349278103340"></a><a name="p12349278103340"></a>约束</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row5118379141712"><td class="cellrowborder" valign="top" width="15.65%" headers="mcps1.2.6.1.1 "><p id="p11935535141712"><a name="p11935535141712"></a><a name="p11935535141712"></a>trigger_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.65%" headers="mcps1.2.6.1.2 "><p id="p27254272141712"><a name="p27254272141712"></a><a name="p27254272141712"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.99%" headers="mcps1.2.6.1.3 "><p id="p60112389141712"><a name="p60112389141712"></a><a name="p60112389141712"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.42%" headers="mcps1.2.6.1.4 "><p id="p37265318141712"><a name="p37265318141712"></a><a name="p37265318141712"></a>触发器ID</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.29%" headers="mcps1.2.6.1.5 "><p id="p60767465103340"><a name="p60767465103340"></a><a name="p60767465103340"></a>-</p>
    </td>
    </tr>
    <tr id="row66952413141712"><td class="cellrowborder" valign="top" width="15.65%" headers="mcps1.2.6.1.1 "><p id="p54436405141712"><a name="p54436405141712"></a><a name="p54436405141712"></a>task_token</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.65%" headers="mcps1.2.6.1.2 "><p id="p47272669141712"><a name="p47272669141712"></a><a name="p47272669141712"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.99%" headers="mcps1.2.6.1.3 "><p id="p3880957141712"><a name="p3880957141712"></a><a name="p3880957141712"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.42%" headers="mcps1.2.6.1.4 "><p id="p45922110141712"><a name="p45922110141712"></a><a name="p45922110141712"></a>任务token</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.29%" headers="mcps1.2.6.1.5 "><p id="p23217608103340"><a name="p23217608103340"></a><a name="p23217608103340"></a>-</p>
    </td>
    </tr>
    <tr id="row10645810141712"><td class="cellrowborder" valign="top" width="15.65%" headers="mcps1.2.6.1.1 "><p id="p57004295141712"><a name="p57004295141712"></a><a name="p57004295141712"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.65%" headers="mcps1.2.6.1.2 "><p id="p53945168141712"><a name="p53945168141712"></a><a name="p53945168141712"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.99%" headers="mcps1.2.6.1.3 "><p id="p7482486141712"><a name="p7482486141712"></a><a name="p7482486141712"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.42%" headers="mcps1.2.6.1.4 "><p id="p2101600141712"><a name="p2101600141712"></a><a name="p2101600141712"></a>任务执行返回值</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.29%" headers="mcps1.2.6.1.5 "><p id="p1578084103340"><a name="p1578084103340"></a><a name="p1578084103340"></a>长度1-32768</p>
    </td>
    </tr>
    </tbody>
    </table>


-   Worker触发器消息样例

    WorkRequest触发器消息

    ```
    {
        "trigger_urn": "urn:fgs:cn-north-1:9800716a0c604a8690963103a85754f0:trigger:Worker_WorkRequest_event-28fcb8447a67-d48d-474a-632f-8fb6b67e9bbf_1505544100"
    }
    ```

    Heartbeat触发器消息

    ```
    {
        "trigger_urn": "urn:fgs:cn-north-1:9800716a0c604a8690963103a85754f0:trigger:Worker_HeartBeat_event-88af46478e85-f47f-47e2-5f43-e8011baf2afd_1505544125",
        "task_token": "urn:fgs:cn-north-1:9800716a0c604a8690963103a85754f0:execution:workflow-8f84:e1:ae0d3e648af440af5828696f16f0d1b4"
    }
    ```

    WorkSuccess触发器消息

    ```
    {
        "trigger_urn": "urn:fgs:cn-north-1:9800716a0c604a8690963103a85754f0:trigger:Worker_WorkSuccess_event-c7ce9d4f603c-29fd-4295-7d68-796f19286920_1505544141",
        "task_token": "urn:fgs:cn-north-1:9800716a0c604a8690963103a85754f0:execution:workflow-8f84:e1:ae0d3e648af440af5828696f16f0d1b4",
        "result": "{\"abc\":\"123\"}" 
    }
    ```

    WorkFailure触发器消息

    ```
    {
        "trigger_urn": "urn:fgs:cn-north-1:9800716a0c604a8690963103a85754f0:trigger:Worker_WorkFailure_event-13d7affbbfe4-4f57-44a8-7507-2f4898a901ca_1505544157",
        "task_token": "urn:fgs:cn-north-1:9800716a0c604a8690963103a85754f0:execution:workflow-8f84:e1:ae0d3e648af440af5828696f16f0d1b4",
        "error": "{\"abc\":\"123\"}" 
    }
    ```


## 响应<a name="section24885284"></a>

-   正常响应

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >-   正常响应只存在于同步的触发器消息发送请求的返回值中，其他异步触发器消息发送请求的正常响应为空。  
    >-   目前，同步触发器消息请求为：WorkRequest  

    **响应参数**

    正常响应参数如[表6](#table1262276014348)所示

    **表 6**  正常响应参数

    <a name="table1262276014348"></a>
    <table><thead align="left"><tr id="row5026901014348"><th class="cellrowborder" valign="top" width="25.252525252525253%" id="mcps1.2.4.1.1"><p id="p4525802514348"><a name="p4525802514348"></a><a name="p4525802514348"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.252525252525253%" id="mcps1.2.4.1.2"><p id="p4202143714348"><a name="p4202143714348"></a><a name="p4202143714348"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="49.494949494949495%" id="mcps1.2.4.1.3"><p id="p4829323714348"><a name="p4829323714348"></a><a name="p4829323714348"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1943813814348"><td class="cellrowborder" valign="top" width="25.252525252525253%" headers="mcps1.2.4.1.1 "><p id="p3098533114348"><a name="p3098533114348"></a><a name="p3098533114348"></a>task_token</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.252525252525253%" headers="mcps1.2.4.1.2 "><p id="p2678388114348"><a name="p2678388114348"></a><a name="p2678388114348"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.2.4.1.3 "><p id="p2201072314348"><a name="p2201072314348"></a><a name="p2201072314348"></a>任务token</p>
    </td>
    </tr>
    <tr id="row6387878114348"><td class="cellrowborder" valign="top" width="25.252525252525253%" headers="mcps1.2.4.1.1 "><p id="p679877714348"><a name="p679877714348"></a><a name="p679877714348"></a>work_item</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.252525252525253%" headers="mcps1.2.4.1.2 "><p id="p1383006114348"><a name="p1383006114348"></a><a name="p1383006114348"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.2.4.1.3 "><p id="p4649318614348"><a name="p4649318614348"></a><a name="p4649318614348"></a>任务相关信息</p>
    </td>
    </tr>
    </tbody>
    </table>

-   正常响应样例

    ```
    {
        "task_token": "urn:fgs:cn-north-1:9800716a0c604a8690963103a85754f0:execution:workflow-8f84:e1:ae0d3e648af440af5828696f16f0d1b4",
        "work_item": "{\"question\":\"whats one plus one?\"}"
    }
    ```


-   异常响应

    请参考[异常响应](请求结果.md#section88241732388)。


## 返回值<a name="section44211207557"></a>

请参考[返回值](请求结果.md#section20306194210386)。

