# 函数Trigger Management触发器模型<a name="ZH-CN_TOPIC_0115410470"></a>

## 触发器类型模型<a name="section29630533"></a>

```
{ 
    "trigger_type_code":"string", 
    "display_name":"string", 
    "status":"string", 
    "event_codes":"array of string", 
    "description":"string" 
}
```

触发器类型模型字段说明如[表1](#table1072087614167)所示。

**表 1**  触发器类型模型字段说明表

<a name="table1072087614167"></a>
<table><thead align="left"><tr id="row4078305"><th class="cellrowborder" valign="top" width="23.23%" id="mcps1.2.3.1.1"><p id="p61907274"><a name="p61907274"></a><a name="p61907274"></a>字段名称</p>
</th>
<th class="cellrowborder" valign="top" width="76.77000000000001%" id="mcps1.2.3.1.2"><p id="p48433296"><a name="p48433296"></a><a name="p48433296"></a>字段说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row30782874"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.3.1.1 "><p id="p10384848"><a name="p10384848"></a><a name="p10384848"></a>trigger_type_code</p>
</td>
<td class="cellrowborder" valign="top" width="76.77000000000001%" headers="mcps1.2.3.1.2 "><p id="p35866396"><a name="p35866396"></a><a name="p35866396"></a>触发器类型代码，取值：SMN、DMS、OBS、DIS、APIG、TIMER、CTS、LTS。</p>
</td>
</tr>
<tr id="row54362108"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.3.1.1 "><p id="p41254657"><a name="p41254657"></a><a name="p41254657"></a>display_name</p>
</td>
<td class="cellrowborder" valign="top" width="76.77000000000001%" headers="mcps1.2.3.1.2 "><p id="p53292943"><a name="p53292943"></a><a name="p53292943"></a>触发器类型显示值。</p>
</td>
</tr>
<tr id="row9874440"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.3.1.1 "><p id="p61632181"><a name="p61632181"></a><a name="p61632181"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="76.77000000000001%" headers="mcps1.2.3.1.2 "><p id="p26150783"><a name="p26150783"></a><a name="p26150783"></a>触发器类型状态，可能的状态如下：</p>
<p id="p34030458"><a name="p34030458"></a><a name="p34030458"></a>“DISABLED”： 禁用该触发器。</p>
<p id="p37838669"><a name="p37838669"></a><a name="p37838669"></a>“TEST”：触发器处于测试状态，用户端应设为不可见。</p>
<p id="p5003705"><a name="p5003705"></a><a name="p5003705"></a>“ACTIVE”：触发器可用。</p>
</td>
</tr>
<tr id="row52786299"><td class="cellrowborder" valign="top" width="23.23%" headers="mcps1.2.3.1.1 "><p id="p47831788"><a name="p47831788"></a><a name="p47831788"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="76.77000000000001%" headers="mcps1.2.3.1.2 "><p id="p49169614"><a name="p49169614"></a><a name="p49169614"></a>触发器说明。</p>
</td>
</tr>
</tbody>
</table>

## 触发器实例模型<a name="section50261965"></a>

```
{ 
    "trigger_id":"string",
    "trigger_type_code":"string",
    "event_type_code":"string",
    "status":"string",
    "event_data":"json struct",
    "last_updated_time":"string",
    "created_time":"string" 
}
```

触发器实例模型字段说明如[表2](#table11855096142915)所示。

**表 2**  触发器实例模型字段说明表

<a name="table11855096142915"></a>
<table><thead align="left"><tr id="row7455633"><th class="cellrowborder" valign="top" width="24.240000000000002%" id="mcps1.2.3.1.1"><p id="p67035395"><a name="p67035395"></a><a name="p67035395"></a>字段名称</p>
</th>
<th class="cellrowborder" valign="top" width="75.76%" id="mcps1.2.3.1.2"><p id="p61157901"><a name="p61157901"></a><a name="p61157901"></a>字段说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row54842968"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p13095436"><a name="p13095436"></a><a name="p13095436"></a>trigger_id</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p54097359"><a name="p54097359"></a><a name="p54097359"></a>触发器ID。</p>
</td>
</tr>
<tr id="row17114191"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p44072239"><a name="p44072239"></a><a name="p44072239"></a>trigger_type_code</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p13081587"><a name="p13081587"></a><a name="p13081587"></a>触发器类型代码，取值：SMN、DMS、OBS、DIS、APIG、TIMER、CTS、LTS。</p>
</td>
</tr>
<tr id="row50625422"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p7018532"><a name="p7018532"></a><a name="p7018532"></a>event_type_code</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p31630226"><a name="p31630226"></a><a name="p31630226"></a>事件类型代码，必填字段，可以填任意非空字符串（deprecated）。</p>
</td>
</tr>
<tr id="row16236586"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p40095121"><a name="p40095121"></a><a name="p40095121"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p26479331"><a name="p26479331"></a><a name="p26479331"></a>触发器状态：ACTIVE / DISABLED。</p>
</td>
</tr>
<tr id="row36987393"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p43188833"><a name="p43188833"></a><a name="p43188833"></a>event_data</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p8634594"><a name="p8634594"></a><a name="p8634594"></a>触发器相关定义数据，以JSON结构形式出现。</p>
</td>
</tr>
<tr id="row10602486"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p53495051"><a name="p53495051"></a><a name="p53495051"></a>last_updated_time</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p38131860"><a name="p38131860"></a><a name="p38131860"></a>最后一次更新时间。</p>
</td>
</tr>
<tr id="row7642424"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.3.1.1 "><p id="p15056587"><a name="p15056587"></a><a name="p15056587"></a>created_time</p>
</td>
<td class="cellrowborder" valign="top" width="75.76%" headers="mcps1.2.3.1.2 "><p id="p11624006"><a name="p11624006"></a><a name="p11624006"></a>创建时间。</p>
</td>
</tr>
</tbody>
</table>

## 触发器实例数据<a name="section196721276373"></a>

OBS触发器实例

OBS触发器数据如下。

```
{ 
   "bucket": "yourBucketName", 
   "events": ["s3:ObjectCreated:Put"], 
   "prefix": "yourPrefix", 
   "suffix": "yourSuffix" 
}
```

**表 3**  OBS触发器数据说明表

<a name="table0330352133017"></a>
<table><thead align="left"><tr id="row43304525304"><th class="cellrowborder" valign="top" width="19.59%" id="mcps1.2.3.1.1"><p id="p193301052173013"><a name="p193301052173013"></a><a name="p193301052173013"></a>字段名称</p>
</th>
<th class="cellrowborder" valign="top" width="80.41%" id="mcps1.2.3.1.2"><p id="p8330452103017"><a name="p8330452103017"></a><a name="p8330452103017"></a>字段说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1633025210304"><td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.3.1.1 "><p id="p11330252133019"><a name="p11330252133019"></a><a name="p11330252133019"></a>bucket</p>
</td>
<td class="cellrowborder" valign="top" width="80.41%" headers="mcps1.2.3.1.2 "><p id="p13303527304"><a name="p13303527304"></a><a name="p13303527304"></a>OBS桶名，必填。</p>
</td>
</tr>
<tr id="row2330125293014"><td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.3.1.1 "><p id="p43301952133017"><a name="p43301952133017"></a><a name="p43301952133017"></a>events</p>
</td>
<td class="cellrowborder" valign="top" width="80.41%" headers="mcps1.2.3.1.2 "><p id="p1533035283017"><a name="p1533035283017"></a><a name="p1533035283017"></a>OBS触发事件集合，取值有如下情况：["s3:ObjectCreated:*","s3:ObjectCreated:Put","s3:ObjectCreated:Post","s3:ObjectCreated:Copy","s3:ObjectCreated:CompleteMultipartUpload","s3:ObjectRemoved:*","s3:ObjectRemoved:DeleteMarkerCreated","s3:ObjectRemoved:Delete"]，必填。</p>
<p id="p11330105263017"><a name="p11330105263017"></a><a name="p11330105263017"></a>其中"s3:objectcreated:*"包含所有其他以"s3:objectcreated"开头的所有事件，"s3:objectremoved:*"包含所有以"s3:objectremoved"开头的所有事件。</p>
</td>
</tr>
<tr id="row15331125213020"><td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.3.1.1 "><p id="p033114529302"><a name="p033114529302"></a><a name="p033114529302"></a>prefix</p>
</td>
<td class="cellrowborder" valign="top" width="80.41%" headers="mcps1.2.3.1.2 "><p id="p633125293014"><a name="p633125293014"></a><a name="p633125293014"></a>OBS对象的前缀，选填。</p>
</td>
</tr>
<tr id="row1033185219300"><td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.3.1.1 "><p id="p733185219308"><a name="p733185219308"></a><a name="p733185219308"></a>suffix</p>
</td>
<td class="cellrowborder" valign="top" width="80.41%" headers="mcps1.2.3.1.2 "><p id="p033135214307"><a name="p033135214307"></a><a name="p033135214307"></a>OBS对象的后缀，选填。</p>
</td>
</tr>
</tbody>
</table>

-   SMN触发器实例

    SMN触发器数据如下。

    ```
    { 
        "topic_urn":"string", 
        "subscription_status":"string" 
    } 
    ```

    SMN触发器数据说明如[表4](#table46683704143627)所示。

    **表 4**  SMN触发器数据说明表

    <a name="table46683704143627"></a>
    <table><thead align="left"><tr id="row4308221"><th class="cellrowborder" valign="top" width="25.25%" id="mcps1.2.3.1.1"><p id="p13421600"><a name="p13421600"></a><a name="p13421600"></a>字段名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="74.75%" id="mcps1.2.3.1.2"><p id="p13407787"><a name="p13407787"></a><a name="p13407787"></a>字段说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row12288967"><td class="cellrowborder" valign="top" width="25.25%" headers="mcps1.2.3.1.1 "><p id="p55882267"><a name="p55882267"></a><a name="p55882267"></a>topic_urn</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.75%" headers="mcps1.2.3.1.2 "><p id="p30169808"><a name="p30169808"></a><a name="p30169808"></a>SMN服务的topic_urn，创建时必填。</p>
    </td>
    </tr>
    <tr id="row3092822"><td class="cellrowborder" valign="top" width="25.25%" headers="mcps1.2.3.1.1 "><p id="p49192063"><a name="p49192063"></a><a name="p49192063"></a>subscription_status</p>
    </td>
    <td class="cellrowborder" valign="top" width="74.75%" headers="mcps1.2.3.1.2 "><p id="p25134172"><a name="p25134172"></a><a name="p25134172"></a>topic_urn的订阅状态：Unconfirmed / Confirmed。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   DMS触发器实例

    DMS触发器数据如下。

    ```
    { 
        "queue_id":"string", 
        "consumer_group_id":"string", 
        "polling_interval":"int" 
    }
    ```

    DMS触发器数据说明如[表5](#table0558183404)所示。

    **表 5**  DMS触发器数据说明表

    <a name="table0558183404"></a>
    <table><thead align="left"><tr id="row1762131834012"><th class="cellrowborder" valign="top" width="26.26%" id="mcps1.2.3.1.1"><p id="p864191824013"><a name="p864191824013"></a><a name="p864191824013"></a>字段名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="73.74000000000001%" id="mcps1.2.3.1.2"><p id="p87091854019"><a name="p87091854019"></a><a name="p87091854019"></a>字段说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row472201811401"><td class="cellrowborder" valign="top" width="26.26%" headers="mcps1.2.3.1.1 "><p id="p187401814409"><a name="p187401814409"></a><a name="p187401814409"></a>queue_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="73.74000000000001%" headers="mcps1.2.3.1.2 "><p id="p77511810408"><a name="p77511810408"></a><a name="p77511810408"></a>DMS队列名，创建时必填。</p>
    </td>
    </tr>
    <tr id="row207601894017"><td class="cellrowborder" valign="top" width="26.26%" headers="mcps1.2.3.1.1 "><p id="p2791618134010"><a name="p2791618134010"></a><a name="p2791618134010"></a>consumer_group_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="73.74000000000001%" headers="mcps1.2.3.1.2 "><p id="p37991810403"><a name="p37991810403"></a><a name="p37991810403"></a>DMS消费组名，创建时必填。</p>
    </td>
    </tr>
    <tr id="row168114183401"><td class="cellrowborder" valign="top" width="26.26%" headers="mcps1.2.3.1.1 "><p id="p08491844011"><a name="p08491844011"></a><a name="p08491844011"></a>polling_interval</p>
    </td>
    <td class="cellrowborder" valign="top" width="73.74000000000001%" headers="mcps1.2.3.1.2 "><p id="p48614183409"><a name="p48614183409"></a><a name="p48614183409"></a>检查消息间隔，以秒为单位，缺省为30秒，创建时必填。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   OBS触发器实例

    OBS触发器数据如下。

    ```
    { 
       "bucket": "yourBucketName", 
       "events": ["s3:ObjectCreated:Put"], 
       "prefix": "yourPrefix", 
       "suffix": "yourSuffix" 
    }
    ```

    **表 6**  OBS触发器数据说明表

    <a name="table17999413154914"></a>
    <table><thead align="left"><tr id="row9791414495"><th class="cellrowborder" valign="top" width="19.59%" id="mcps1.2.3.1.1"><p id="p1190615309493"><a name="p1190615309493"></a><a name="p1190615309493"></a>字段名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="80.41%" id="mcps1.2.3.1.2"><p id="p6906230194916"><a name="p6906230194916"></a><a name="p6906230194916"></a>字段说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row187181424918"><td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.3.1.1 "><p id="p14906133034914"><a name="p14906133034914"></a><a name="p14906133034914"></a>bucket</p>
    </td>
    <td class="cellrowborder" valign="top" width="80.41%" headers="mcps1.2.3.1.2 "><p id="p1690623094916"><a name="p1690623094916"></a><a name="p1690623094916"></a>OBS桶名，必填。</p>
    </td>
    </tr>
    <tr id="row17714145497"><td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.3.1.1 "><p id="p1091413084918"><a name="p1091413084918"></a><a name="p1091413084918"></a>events</p>
    </td>
    <td class="cellrowborder" valign="top" width="80.41%" headers="mcps1.2.3.1.2 "><p id="p9814510443"><a name="p9814510443"></a><a name="p9814510443"></a>OBS触发事件集合，取值有如下情况：["s3:ObjectCreated:*","s3:ObjectCreated:Put","s3:ObjectCreated:Post","s3:ObjectCreated:Copy","s3:ObjectCreated:CompleteMultipartUpload","s3:ObjectRemoved:*","s3:ObjectRemoved:DeleteMarkerCreated","s3:ObjectRemoved:Delete"]，必填。</p>
    <p id="p1738125614214"><a name="p1738125614214"></a><a name="p1738125614214"></a>其中"s3:objectcreated:*"包含所有其他以"s3:objectcreated"开头的所有事件，"s3:objectremoved:*"包含所有以"s3:objectremoved"开头的所有事件。</p>
    </td>
    </tr>
    <tr id="row5731419493"><td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.3.1.1 "><p id="p4914830114910"><a name="p4914830114910"></a><a name="p4914830114910"></a>prefix</p>
    </td>
    <td class="cellrowborder" valign="top" width="80.41%" headers="mcps1.2.3.1.2 "><p id="p1992153064918"><a name="p1992153064918"></a><a name="p1992153064918"></a>OBS对象的前缀，选填。</p>
    </td>
    </tr>
    <tr id="row15701484910"><td class="cellrowborder" valign="top" width="19.59%" headers="mcps1.2.3.1.1 "><p id="p10921203034914"><a name="p10921203034914"></a><a name="p10921203034914"></a>suffix</p>
    </td>
    <td class="cellrowborder" valign="top" width="80.41%" headers="mcps1.2.3.1.2 "><p id="p19921153010497"><a name="p19921153010497"></a><a name="p19921153010497"></a>OBS对象的后缀，选填。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   DIS触发器实例

    DIS触发器数据如下。

    ```
    {
    "stream_name": "dis-qYPJ",
    "polling_interval": 30,
    "batch_size": 100,
    "sharditerator_type": "TRIM_HORIZON"
    }
    ```

    DIS触发器数据说明如[表7](#table797218531255)所示。

    **表 7**  DIS触发器数据说明表

    <a name="table797218531255"></a>
    <table><thead align="left"><tr id="row19754535259"><th class="cellrowborder" valign="top" width="21.21%" id="mcps1.2.3.1.1"><p id="p297719537257"><a name="p297719537257"></a><a name="p297719537257"></a>字段名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="78.79%" id="mcps1.2.3.1.2"><p id="p18978453192513"><a name="p18978453192513"></a><a name="p18978453192513"></a>字段说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row129791453122512"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p89807536259"><a name="p89807536259"></a><a name="p89807536259"></a>stream_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p17982105311252"><a name="p17982105311252"></a><a name="p17982105311252"></a>通道名称，必填。</p>
    </td>
    </tr>
    <tr id="row698325318255"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p19984115314255"><a name="p19984115314255"></a><a name="p19984115314255"></a>polling_interval</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p698715322511"><a name="p698715322511"></a><a name="p698715322511"></a>拉取周期，取值1-60，选填（不填会取默认值30）。</p>
    </td>
    </tr>
    <tr id="row1898812530258"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p17989175315253"><a name="p17989175315253"></a><a name="p17989175315253"></a>batch_size</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p16991153122517"><a name="p16991153122517"></a><a name="p16991153122517"></a>每次拉取的记录数量，取值1-10000，选填（不填会取默认值100）。</p>
    </td>
    </tr>
    <tr id="row29918538254"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p1099275332511"><a name="p1099275332511"></a><a name="p1099275332511"></a>sharditerator_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p99931053142515"><a name="p99931053142515"></a><a name="p99931053142515"></a>取值TRIM_HORIZON（从头开始拉取）/LATEST（从当前位置开始拉取），必填。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   APIG触发器实例

    APIG触发器数据如下。

    ```
    { 
        "group_id":"string", 
        "env_id":"string", 
        "auth":"string", 
        "protocol":"string", 
        "name":"string", 
        "path":"string", 
        "match_mode":"string",  
        "req_method":"string" , 
        "backend_type":"string" , 
        "type": int , 
        "sl_domain":"string" 
    }
    ```

    APIG触发器数据说明如<u>[表8](#table18282101120468)</u>所示。

    **表 8**  APIG触发器数据说明表

    <a name="table18282101120468"></a>
    <table><thead align="left"><tr id="row1329061113469"><th class="cellrowborder" valign="top" width="21.21%" id="mcps1.2.3.1.1"><p id="p2029110111467"><a name="p2029110111467"></a><a name="p2029110111467"></a>字段名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="78.79%" id="mcps1.2.3.1.2"><p id="p72931811104613"><a name="p72931811104613"></a><a name="p72931811104613"></a>字段说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row02953117466"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p11296191116463"><a name="p11296191116463"></a><a name="p11296191116463"></a>group_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p14298311164618"><a name="p14298311164618"></a><a name="p14298311164618"></a>API分组，必填。</p>
    </td>
    </tr>
    <tr id="row102999111469"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p8300121144610"><a name="p8300121144610"></a><a name="p8300121144610"></a>env_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p1030231120460"><a name="p1030231120460"></a><a name="p1030231120460"></a>API发布环境，必填。</p>
    </td>
    </tr>
    <tr id="row123046117468"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p83051311204610"><a name="p83051311204610"></a><a name="p83051311204610"></a>auth</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p143061811104616"><a name="p143061811104616"></a><a name="p143061811104616"></a>API认证方式，三种可选模式： NONE/IAM/APP，必填。</p>
    </td>
    </tr>
    <tr id="row0307101174618"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p73081411124617"><a name="p73081411124617"></a><a name="p73081411124617"></a>protocol</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p0309111164616"><a name="p0309111164616"></a><a name="p0309111164616"></a>访问协议，HTTP或HTTPS，必填。</p>
    </td>
    </tr>
    <tr id="row11310611144616"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p831121116465"><a name="p831121116465"></a><a name="p831121116465"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p1444712591014"><a name="p1444712591014"></a><a name="p1444712591014"></a>API名称，必填。</p>
    </td>
    </tr>
    <tr id="row1731351124610"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p131419110466"><a name="p131419110466"></a><a name="p131419110466"></a>path</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p59913371628"><a name="p59913371628"></a><a name="p59913371628"></a>API访问地址，需要服从URL规范，如/a/b，必填。</p>
    </td>
    </tr>
    <tr id="row14316111154616"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p1831711116467"><a name="p1831711116467"></a><a name="p1831711116467"></a>match_mode</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p21651512414"><a name="p21651512414"></a><a name="p21651512414"></a>匹配模式，SWA（前缀匹配）或NORMAL（普通匹配），必填。</p>
    </td>
    </tr>
    <tr id="row456035604913"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p175611356184915"><a name="p175611356184915"></a><a name="p175611356184915"></a>req_method</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p1856117563497"><a name="p1856117563497"></a><a name="p1856117563497"></a>API请求方式，枚举如：GET、POST、PUT，必填。</p>
    </td>
    </tr>
    <tr id="row11626645145012"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p10626134575015"><a name="p10626134575015"></a><a name="p10626134575015"></a>backend_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p14627104515509"><a name="p14627104515509"></a><a name="p14627104515509"></a>后端类型：FUNCTION，必填。</p>
    </td>
    </tr>
    <tr id="row175011402512"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p9501180205111"><a name="p9501180205111"></a><a name="p9501180205111"></a>type</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p2501140175118"><a name="p2501140175118"></a><a name="p2501140175118"></a>API类型：开放API为1，私有API为2，必填。</p>
    </td>
    </tr>
    <tr id="row1350103175112"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p45043155116"><a name="p45043155116"></a><a name="p45043155116"></a>sl_domain</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p2050836519"><a name="p2050836519"></a><a name="p2050836519"></a>子域名，必填.</p>
    </td>
    </tr>
    </tbody>
    </table>

-   TIMER触发器实例

    TIMER触发器数据如下。

    ```
    {
    	"name": "string",
    	"schedule_type": "string",
    	"schedule": "string",
    	"user_event": "string"
    }
    ```

    TIMER触发器数据说明如<u>[表9](#table169831625017)</u>所示。

    **表 9**  TIMER触发器数据说明表

    <a name="table169831625017"></a>
    <table><thead align="left"><tr id="row1598213251719"><th class="cellrowborder" valign="top" width="21.21%" id="mcps1.2.3.1.1"><p id="p89827251818"><a name="p89827251818"></a><a name="p89827251818"></a>字段名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="78.79%" id="mcps1.2.3.1.2"><p id="p12982925913"><a name="p12982925913"></a><a name="p12982925913"></a>字段说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row19982192519119"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p698214252018"><a name="p698214252018"></a><a name="p698214252018"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p39820252119"><a name="p39820252119"></a><a name="p39820252119"></a>触发器名称，必填。</p>
    </td>
    </tr>
    <tr id="row1698272511116"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p20982325113"><a name="p20982325113"></a><a name="p20982325113"></a>schedule_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p1198222510112"><a name="p1198222510112"></a><a name="p1198222510112"></a>调度类型，两种可选模式：Rate/Cron，必填。</p>
    </td>
    </tr>
    <tr id="row179821725415"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p998217257117"><a name="p998217257117"></a><a name="p998217257117"></a>schedule</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p1898214252113"><a name="p1898214252113"></a><a name="p1898214252113"></a>调度配置，分别根据不同的调度类型填写，必填。</p>
    <p id="p12279183214273"><a name="p12279183214273"></a><a name="p12279183214273"></a>当选择Rate模式时，格式为数字加上m(分钟)，h(小时)，d(天)，如3分钟为3m。</p>
    </td>
    </tr>
    <tr id="row6983182514115"><td class="cellrowborder" valign="top" width="21.21%" headers="mcps1.2.3.1.1 "><p id="p59838252012"><a name="p59838252012"></a><a name="p59838252012"></a>user_event</p>
    </td>
    <td class="cellrowborder" valign="top" width="78.79%" headers="mcps1.2.3.1.2 "><p id="p79835258114"><a name="p79835258114"></a><a name="p79835258114"></a>调用附加信息，作为调用函数时的参数，可选。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   LTS触发器实例

    LTS触发器数据如下：

    ```
    {
    	"trigger_type_code": "LTS",
    	"event_type_code": "MessageCreated",
    	"trigger_status": "ACTIVE",
    	"event_data": {
    		"log_group_id": "3e4d3bf7-7bad-11e9-92c5-fa163e6216be",
    		"log_topic_id": "41d90375-7bad-11e9-8bcf-fa163ea23ac3",
    		"log_group_name": "lts-group-5b42",
    		"log_topic_name": "lts-topic-5f3e"
    	}
    }
    ```

    LTS数据说明如所[表10](#table866014421545)示。

    **表 10**  LTS触发器数据说明表

    <a name="table866014421545"></a>
    <table><thead align="left"><tr id="row156603421411"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.3.1.1"><p id="p86601842542"><a name="p86601842542"></a><a name="p86601842542"></a>字段名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="75%" id="mcps1.2.3.1.2"><p id="p966044214410"><a name="p966044214410"></a><a name="p966044214410"></a>字段说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row126607423419"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p126605421415"><a name="p126605421415"></a><a name="p126605421415"></a>group_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p116603421048"><a name="p116603421048"></a><a name="p116603421048"></a>LTS日志组，创建时必选。</p>
    </td>
    </tr>
    <tr id="row266064212412"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.3.1.1 "><p id="p1266024218416"><a name="p1266024218416"></a><a name="p1266024218416"></a>topic_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="75%" headers="mcps1.2.3.1.2 "><p id="p166607429412"><a name="p166607429412"></a><a name="p166607429412"></a>LTS日志主题，创建时必选。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   CTS触发器实例

    CTS触发器数据如下。

    ```
    {
    	"name": "eqwrwe",
    	"operations": ["AAD:addprotocolrule:addProtocolRule", "BCS:baas-apiserver:scalePeers", "ARS:ars:setConfigArs"]
    }
    ```

    CTS触发器数据说明如[表11](#table15406140191011)所示。

    **表 11**  CTS触发器数据说明表

    <a name="table15406140191011"></a>
    <table><thead align="left"><tr id="row9408840151010"><th class="cellrowborder" valign="top" width="24%" id="mcps1.2.3.1.1"><p id="p19408144012100"><a name="p19408144012100"></a><a name="p19408144012100"></a>字段名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="76%" id="mcps1.2.3.1.2"><p id="p540854051015"><a name="p540854051015"></a><a name="p540854051015"></a>字段说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row194083408109"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.3.1.1 "><p id="p194083401104"><a name="p194083401104"></a><a name="p194083401104"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="76%" headers="mcps1.2.3.1.2 "><p id="p6408154011015"><a name="p6408154011015"></a><a name="p6408154011015"></a>关键通知名称。</p>
    </td>
    </tr>
    <tr id="row10408104021011"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.3.1.1 "><p id="p9408104015100"><a name="p9408104015100"></a><a name="p9408104015100"></a>operations</p>
    </td>
    <td class="cellrowborder" valign="top" width="76%" headers="mcps1.2.3.1.2 "><p id="p17408134051018"><a name="p17408134051018"></a><a name="p17408134051018"></a>操作列表，(服务类型:资源类型A;资源类型B:操作名称1;操作名称2)["ECS:ecs;server:restartServer;deleteServer",...]。</p>
    </td>
    </tr>
    </tbody>
    </table>


