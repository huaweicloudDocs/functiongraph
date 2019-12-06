# 使用APIG触发器<a name="ZH-CN_TOPIC_0149027363"></a>

本节介绍创建APIG触发器，使用API调用函数运行。供用户了解APIG触发器的使用方法。

关于APIG触发器事件源具体介绍请参见[支持的事件源](http://support.huaweicloud.com/devg-functiongraph/functiongraph_02_0102.html)。

## 前提条件<a name="section76949209512"></a>

进行操作之前，需要做好以下准备。

已经创建API分组，此处以function分组为例，创建过程请参考[创建API分组](https://support.huaweicloud.com/usermanual-apig/apig-zh-ug-180307015.html)。

## 创建APIG触发器<a name="section0341823105810"></a>

1.  用户登录FunctionGraph控制台，进入“函数”界面。
2.  在“函数”界面，选择“函数列表”，单击“创建函数”，进入“创建函数”界面。
3.  在“创建函数”界面填写函数信息。
    1.  模板选择“已有模板”。
    2.  选择“APIG触发器使用指导”模板，单击“使用此模板”，加载函数代码及配置信息。
    3.  输入函数名称：read\_apig\_message。

        **图 1**  APIG触发器使用指导模板<a name="fig849514143554"></a>  
        ![](figures/APIG触发器使用指导模板.png "APIG触发器使用指导模板")

    4.  输入APIG触发器配置信息，带\*参数为必填项。

        **表 1**  触发器信息表

        <a name="table4277812911123"></a>
        <table><thead align="left"><tr id="row6452289411123"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p10222672111212"><a name="p10222672111212"></a><a name="p10222672111212"></a>字段</p>
        </th>
        <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p22730128111212"><a name="p22730128111212"></a><a name="p22730128111212"></a>填写说明</p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="row3775359111123"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p29066614111212"><a name="p29066614111212"></a><a name="p29066614111212"></a>*API名称</p>
        </td>
        <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1611005615198"><a name="p1611005615198"></a><a name="p1611005615198"></a>支持汉字，英文，数字，下划线，且只能以英文和汉字开头，3-24字符。</p>
        <p id="p1753551895938"><a name="p1753551895938"></a><a name="p1753551895938"></a>输入read_apig_message。</p>
        </td>
        </tr>
        <tr id="row1040996411123"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p45327539111212"><a name="p45327539111212"></a><a name="p45327539111212"></a>*分组</p>
        </td>
        <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p3270906795938"><a name="p3270906795938"></a><a name="p3270906795938"></a>API分组相当于一个API集合，API提供方以API分组为单位，管理分组内的所有API。</p>
        <p id="p35945817143857"><a name="p35945817143857"></a><a name="p35945817143857"></a>选择创建的function。</p>
        </td>
        </tr>
        <tr id="row593612298329"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p20937182923211"><a name="p20937182923211"></a><a name="p20937182923211"></a>*发布环境</p>
        </td>
        <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p59381329153216"><a name="p59381329153216"></a><a name="p59381329153216"></a>API可以同时提供给不同的场景调用，如生产、测试或开发。API网关服务提供环境管理，在不同的环境定义不同的API调用路径。</p>
        <p id="p3204061314398"><a name="p3204061314398"></a><a name="p3204061314398"></a>选择Release，才能调用。</p>
        </td>
        </tr>
        <tr id="row15723165312323"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p197231153163212"><a name="p197231153163212"></a><a name="p197231153163212"></a>*安全认证</p>
        </td>
        <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p11141193616518"><a name="p11141193616518"></a><a name="p11141193616518"></a>API认证方式：</p>
        <p id="p43523042143943"><a name="p43523042143943"></a><a name="p43523042143943"></a>APP： 采用Appkey&amp;Appsecret认证，安全级别高，推荐使用，详情请参考<a href="https://support.huaweicloud.com/devg-apig/apig-zh-dev-180307002.html" target="_blank" rel="noopener noreferrer">APP认证</a>。</p>
        <p id="p16921958104219"><a name="p16921958104219"></a><a name="p16921958104219"></a>IAM： IAM认证，只允许公有云用户能访问，安全级别中等，详情请参考<a href="https://support.huaweicloud.com/devg-apig/apig-zh-dev-180307020.html" target="_blank" rel="noopener noreferrer">IAM认证</a>。</p>
        <p id="p6365254143945"><a name="p6365254143945"></a><a name="p6365254143945"></a>None： 无认证模式，所有用户均可访问。</p>
        <p id="p55389227143952"><a name="p55389227143952"></a><a name="p55389227143952"></a>选择None。</p>
        </td>
        </tr>
        <tr id="row5329068911123"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p77707145331"><a name="p77707145331"></a><a name="p77707145331"></a>*请求协议</p>
        </td>
        <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p8342198612"><a name="p8342198612"></a><a name="p8342198612"></a>分为两种类型：</p>
        <a name="ul10342591866"></a><a name="ul10342591866"></a><ul id="ul10342591866"><li>HTTP</li><li>HTTPS</li></ul>
        <p id="p2504395514409"><a name="p2504395514409"></a><a name="p2504395514409"></a>选择HTTPS。</p>
        </td>
        </tr>
        <tr id="row185036265474"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p2824122816478"><a name="p2824122816478"></a><a name="p2824122816478"></a>*后端超时(毫秒)</p>
        </td>
        <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1550572654714"><a name="p1550572654714"></a><a name="p1550572654714"></a>输入“5000”。</p>
        </td>
        </tr>
        </tbody>
        </table>

        >![](public_sys-resources/icon-note.gif) **说明：**   
        >发布环境选择Release，创建触发器时，会在API网关生成API，并且将生成的API发布，可以直接调用。  


4.  单击“创建函数”，创建函数及触发器。

    **图 2**  APIG触发器<a name="fig99182432558"></a>  
    ![](figures/APIG触发器.png "APIG触发器")

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >1.  APIG触发器调用地址：https://4e5cb396-e812-42b3-85bf-a7aac3cd6cba.apigw.xx-xxxx-1.xxxxxxxxx.com/read\_apig\_message。  
    >2.  API触发器创建完成后，会在API网关生成名为read\_apig\_message的API，单击API名称，跳转至API网关服务。  


## 调用函数<a name="section5526738175817"></a>

1.  打开浏览器，将APIG触发器调用地址输入地址栏，如[图3](#fig42713216569)所示。

    **图 3**  调用函数<a name="fig42713216569"></a>  
    ![](figures/调用函数.png "调用函数")

2.  根据提示，补充responseType为html，将以下地址输入浏览器地址栏。

    https://4e5cb396-e812-42b3-85bf-a7aac3cd6cba.apigw.xxxx-xxxxx-1.xxxxxxcloud.com/read\_apig\_message?responseType=html。

3.  函数执行完毕，得到返回结果，如[图4 返回结果](#fig640414181488)所示。

    **图 4**  返回结果<a name="fig640414181488"></a>  
    ![](figures/返回结果.png "返回结果")


## 查看函数运行结果<a name="section4315195519585"></a>

1.  登录FunctionGraph控制台，进入“函数”界面。
2.  在“函数”界面，选择“函数列表”，单击read\_apig\_message函数名称，进入read\_apig\_message函数详情界面。
3.  在read\_apig\_message函数详情界面，单击“日志”页签，查询函数运行日志。
4.  单击操作栏的“查看上下文”，查看日志详细信息。

