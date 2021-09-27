# 使用GaussDB\(for Mongo\)触发器<a name="ZH-CN_TOPIC_0000001162435507"></a>

本节介绍创建GaussDB\(for Mongo\)触发器，供用户了解GaussDB\(for Mongo\)触发器的使用方法。

使用GaussDB\(for Mongo\)触发器，每次更新数据库中的表时，都可以触发FunctionGraph函数以执行额外的工作，关于GaussDB\(for Mongo\)触发器事件源具体介绍请参见[支持的事件源](https://support.huaweicloud.com/devg-functiongraph/functiongraph_02_0102.html)。

>![](public_sys-resources/icon-note.gif) **说明：** 
>该功能当前仅支持以下区域：华北-北京四，华北-乌兰察布二零一，华东-上海一，华南-广州，中国-香港，亚太-新加坡。

## 前提条件<a name="section134592267445"></a>

进行操作之前，需要做好以下准备。

-   已经创建函数，创建过程请参考[创建并初始化函数](创建并初始化函数.md)。
-   创建GaussDB\(for Mongo\)触发器，必须开启函数工作流VPC访问，请参考[函数配置VPC](函数配置VPC.md)。
-   已经创建GaussDB\(for Mongo\)云数据库实例，创建过程请参考[云数据库GaussDB NoSQL 实例](https://support.huaweicloud.com/mongoug-nosql/nosql_02_0107.html)。

## 创建GaussDB触发器<a name="section3956183013126"></a>

1.  登录FunctionGraph控制台，进入“函数”界面。
2.  在“函数”界面，选择“函数列表”，单击HelloWorld函数名称，进入HelloWorld函数详情界面。
3.  在HelloWorld函数详情界面，单击“触发器”页签。
4.  在“触发器”页签，单击“创建触发器”，弹出“创建触发器”对话框。
5.  设置以下信息。
    -   触发器类型：选择“云数据库GaussDB\(for Mongo\)”。
    -   GaussDB\(for Mongo\)：选择已创建的GaussDB实例。
    -   密码：GaussDB数据库实例管理员rwuser的密码。
    -   数据库：输入GaussDB\(for Mongo\)实例数据库名称。admin、local、config为保留数据库，不能使用。
    -   集合：数据库集合名称。
    -   批处理大小：每批从数据库读取的记录的数量。

6.  单击“确定“，完成GaussDB触发器的创建。

## 配置GaussDB事件触发函数<a name="section8958730121211"></a>

1.  登录FunctionGraph控制台，进入“函数”界面。
2.  在“函数”界面，选择“函数列表”，单击HelloWorld函数名称，进入HelloWorld函数详情界面。
3.  在HelloWorld函数详情页，选择函数版本，单击“请选择测试事件 \> 配置测试事件”，弹出“配置测试事件”对话框。
4.  填写如[表1](#table195851947133114)所示测试信息后，单击“保存”。

    **表 1**  测试信息

    <a name="table195851947133114"></a>
    <table><thead align="left"><tr id="row11584124753120"><th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.2.3.1.1"><p id="p1358414733114"><a name="p1358414733114"></a><a name="p1358414733114"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="72%" id="mcps1.2.3.1.2"><p id="p115840477317"><a name="p115840477317"></a><a name="p115840477317"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1758414783114"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.3.1.1 "><p id="p18584154714315"><a name="p18584154714315"></a><a name="p18584154714315"></a>配置测试事件</p>
    </td>
    <td class="cellrowborder" valign="top" width="72%" headers="mcps1.2.3.1.2 "><p id="p1558454715316"><a name="p1558454715316"></a><a name="p1558454715316"></a>可创建新的测试事件也可编辑已有的测试事件。</p>
    <p id="p15584104713314"><a name="p15584104713314"></a><a name="p15584104713314"></a>选择默认值：“创建新的测试事件”。</p>
    </td>
    </tr>
    <tr id="row1558444712317"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.3.1.1 "><p id="p17584134743116"><a name="p17584134743116"></a><a name="p17584134743116"></a>事件模板</p>
    </td>
    <td class="cellrowborder" valign="top" width="72%" headers="mcps1.2.3.1.2 "><p id="p1058494763117"><a name="p1058494763117"></a><a name="p1058494763117"></a>选择"gaussmongo-event-template"模板，使用系统内置GaussDB(for Mongo)事件模板。</p>
    </td>
    </tr>
    <tr id="row158404716313"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.3.1.1 "><p id="p1858434719318"><a name="p1858434719318"></a><a name="p1858434719318"></a>事件名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="72%" headers="mcps1.2.3.1.2 "><p id="p1843184212400"><a name="p1843184212400"></a><a name="p1843184212400"></a>事件名称必须以大写或小写字母开头，支持字母（大写或小写），数字和下划线“_”（或中划线“-”），并以字母或数字结尾，长度为1-25个字符，例如gaussmongo-123test。</p>
    </td>
    </tr>
    <tr id="row19584184713114"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.3.1.1 "><p id="p85846473314"><a name="p85846473314"></a><a name="p85846473314"></a>测试事件</p>
    </td>
    <td class="cellrowborder" valign="top" width="72%" headers="mcps1.2.3.1.2 "><p id="p18584134753112"><a name="p18584134753112"></a><a name="p18584134753112"></a>自动加载系统内置GaussDB(for Mongo)事件模板，本例不做修改。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >测试事件模板示例如下：
    >```
    >{
    >	"records": [{
    >		"event_name": "\"insert\"",
    >		"event_version": "1.0",
    >		"event_source": "gauss_mongo",
    >		"region": "cn-north-1",
    >		"gauss_mongo": {
    >			"full_document": "{\"_id\": {\"$oid\":\"5f61de944778db5fcded3f87\"},\"zhangsan\": \"zhangsan\"}",
    >			"ns": "{\"db\": \"zhangsan\",\"coll\": \"zhangsan\"}",
    >			"size_bytes": "100",
    >			"token": "{\"_data\": \"825F61DE940000000129295A1004A2D9AE61206C43A5AF47CAF7C5C00C5946645F696400645F61DE944778DB5FCDED3F870004\"}"
    >		},
    >		"event_source_id": "51153d19-2b7d-402c-9a79-757163258a36"
    >	}],
    >	"vernier": "{\"_data\": \"825F61DE940000000129295A1004A2D9AE61206C43A5AF47CAF7C5C00C5946645F696400645F61DE944778DB5FCDED3F870004\"}"
    >}
    >```

5.  单击“测试”，可以得到函数运行结果，函数会返回输入GaussDB\(for Mongo\)数据。如[图1](#fig89541826201)所示。

    **图 1**  GaussDB\(for Mongo\)触发器测试结果<a name="fig89541826201"></a>  
    ![](figures/GaussDB(for-Mongo)触发器测试结果.png "GaussDB(for-Mongo)触发器测试结果")


