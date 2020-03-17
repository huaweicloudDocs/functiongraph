# 使用Kafka触发器<a name="ZH-CN_TOPIC_0214164330"></a>

本节介绍创建Kafka触发器，供用户了解Kafka触发器的使用方法。

使用Kafka触发器，当向Kafka实例的Topic生产消息时，FunctionGraph会消费消息，触发函数以执行额外的工作，关于Kafka触发器的事件源介绍请参见[支持的事件源](http://support.huaweicloud.com/devg-functiongraph/functiongraph_02_0102.html)。

## 前提条件<a name="section134592267445"></a>

进行操作之前，需要做好以下准备。

-   已经创建函数，创建过程请参考[代码上传方式创建运行和初始化函数](代码上传方式创建运行和初始化函数.md)。
-   创建Kafka触发器，必须开启函数工作流VPC访问，请参考[函数配置VPC](函数配置VPC.md)。
-   已经Kafka触发器实例，请参考[购买Kafka专享版实例](https://support.huaweicloud.com/usermanual-kafka/kafka-ug-180604013.html)。
-   在Kafka触发器下创建主题，请参考[Kafka实例创建Topic](https://support.huaweicloud.com/usermanual-kafka/kafka-ug-180604018.html)。

## 创建Kafka触发器<a name="section3956183013126"></a>

1.  登录FunctionGraph控制台，进入“函数”界面。
2.  在“函数”界面，选择“函数列表”，单击HelloWorld函数名称，进入HelloWorld函数详情界面。
3.  在HelloWorld函数详情界面，单击“触发器”页签。
4.  在“触发器”页签，单击“创建触发器”，如[图1](#fig1779716147018)所示，弹出“创建触发器”界面。

    **图 1**  创建kafka触发器<a name="fig1779716147018"></a>  
    ![](figures/创建kafka触发器.png "创建kafka触发器")

5.  在“创建触发器“界面，触发器类型选择“分布式消息服务（Kafka）”填写触发器信息，如[表1](#table15529346278)所示，带\*参数为必填项。

    创建Kafka触发器，必须开启函数工作流VPC访问，请参考[函数配置VPC](函数配置VPC.md)。

    **表 1**  Kafka触发器信息表

    <a name="table15529346278"></a>
    <table><thead align="left"><tr id="row2051123452719"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p12501134182719"><a name="p12501134182719"></a><a name="p12501134182719"></a>字段</p>
    </th>
    <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p17511334132714"><a name="p17511334132714"></a><a name="p17511334132714"></a>填写说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row451134102713"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p17514348275"><a name="p17514348275"></a><a name="p17514348275"></a>*实例</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p12518347279"><a name="p12518347279"></a><a name="p12518347279"></a>选择已创建专享版Kafka实例。</p>
    </td>
    </tr>
    <tr id="row55133414278"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p25114345272"><a name="p25114345272"></a><a name="p25114345272"></a>*主题</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p16511734152715"><a name="p16511734152715"></a><a name="p16511734152715"></a>选择专享版Kafka实例的Topic。</p>
    </td>
    </tr>
    <tr id="row145118346272"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p95193452713"><a name="p95193452713"></a><a name="p95193452713"></a>*批处理大小</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1651734192712"><a name="p1651734192712"></a><a name="p1651734192712"></a>每次从Topic消费的消息数量。</p>
    <p id="p6514340274"><a name="p6514340274"></a><a name="p6514340274"></a>取值范围1-1000。</p>
    </td>
    </tr>
    <tr id="row55133416274"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p451103418277"><a name="p451103418277"></a><a name="p451103418277"></a>用户名</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p751183492713"><a name="p751183492713"></a><a name="p751183492713"></a>连接Kafka专享版实例的用户名。</p>
    <p id="p18511334152715"><a name="p18511334152715"></a><a name="p18511334152715"></a>Kafka实例开启ssl时需要填写。</p>
    </td>
    </tr>
    <tr id="row175217342274"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p17511034162716"><a name="p17511034162716"></a><a name="p17511034162716"></a>密码</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1352183412718"><a name="p1352183412718"></a><a name="p1352183412718"></a>连接Kafka专享版实例的密码。</p>
    <p id="p11521034122719"><a name="p11521034122719"></a><a name="p11521034122719"></a>Kafka实例开启ssl时需要填写。</p>
    </td>
    </tr>
    </tbody>
    </table>

6.  单击“确定“，完成触发器创建。

## 配置Kafka事件触发函数<a name="section8958730121211"></a>

1.  登录FunctionGraph控制台，进入“函数”界面。
2.  在“函数”界面，选择“函数列表”，单击HelloWorld函数名称，进入HelloWorld函数详情界面。
3.  在HelloWorld函数详情页，选择函数版本，单击“请选择测试事件\>配置测试事件”，如[图2](#fig12868111714416)所示，弹出“配置测试事件”页。

    **图 2**  配置Kafka测试事件<a name="fig12868111714416"></a>  
    ![](figures/配置Kafka测试事件.png "配置Kafka测试事件")

4.  在“配置测试事件”界面填写如[表2](#table15199135171812)所示测试信息后单击“保存”，带\*参数为必填项。

    **表 2**  测试信息

    <a name="table15199135171812"></a>
    <table><thead align="left"><tr id="row31976510182"><th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.2.3.1.1"><p id="p71977514187"><a name="p71977514187"></a><a name="p71977514187"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="72%" id="mcps1.2.3.1.2"><p id="p8197165171812"><a name="p8197165171812"></a><a name="p8197165171812"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row219735171814"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.3.1.1 "><p id="p3197850189"><a name="p3197850189"></a><a name="p3197850189"></a>配置测试事件</p>
    </td>
    <td class="cellrowborder" valign="top" width="72%" headers="mcps1.2.3.1.2 "><p id="p819718513189"><a name="p819718513189"></a><a name="p819718513189"></a>可创建新的测试事件也可编辑已有的测试事件。</p>
    <p id="p019785141810"><a name="p019785141810"></a><a name="p019785141810"></a>选择默认值：“创建新的测试事件”。</p>
    </td>
    </tr>
    <tr id="row019845151817"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.3.1.1 "><p id="p1619715519182"><a name="p1619715519182"></a><a name="p1619715519182"></a>事件模板</p>
    </td>
    <td class="cellrowborder" valign="top" width="72%" headers="mcps1.2.3.1.2 "><p id="p519812511182"><a name="p519812511182"></a><a name="p519812511182"></a>选择"kafka-event-template"模板，使用系统内置Kafka事件模板。</p>
    </td>
    </tr>
    <tr id="row01981653188"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.3.1.1 "><p id="p619865201814"><a name="p619865201814"></a><a name="p619865201814"></a>*事件名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="72%" headers="mcps1.2.3.1.2 "><p id="p2019825121816"><a name="p2019825121816"></a><a name="p2019825121816"></a>事件名称必须仅包含字母和数字，且最大长度为 25 个字符。</p>
    <p id="p171981253182"><a name="p171981253182"></a><a name="p171981253182"></a>输入“kafka-test”。</p>
    </td>
    </tr>
    <tr id="row71991752189"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.3.1.1 "><p id="p81983518186"><a name="p81983518186"></a><a name="p81983518186"></a>测试事件</p>
    </td>
    <td class="cellrowborder" valign="top" width="72%" headers="mcps1.2.3.1.2 "><p id="p1419810515185"><a name="p1419810515185"></a><a name="p1419810515185"></a>自动加载系统内置kafka事件模板，本例不做修改。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >测试事件模板示例如下：  
    >```  
    >{  
    >    "event_version": "v1.0",  
    >    "event_time": 1576737962,  
    >    "trigger_type": "KAFKA",  
    >    "region": "xx-xxxx-1",  
    >    "messages": [  
    >        "kafka message1",  
    >        "kafka message2",  
    >        "kafka message3",  
    >        "kafka message4",  
    >        "kafka message5"  
    >    ],  
    >    "instance_id": "81335d56-b9fe-4679-ba95-7030949cc76b",  
    >    "topic_id": "topic-test"  
    >}  
    >```  

5.  单击“测试”，可以得到函数运行结果，函数会返回输入kafka消息数据。

