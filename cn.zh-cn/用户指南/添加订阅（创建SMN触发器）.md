# 添加订阅（创建SMN触发器）<a name="functiongraph_01_0560"></a>

用户可以在函数详情页触发器页签创建触发器，也可以在消息主题添加FunctionGraph（函数）协议的订阅，生成SMN触发器。

添加订阅（创建SMN触发器）步骤如下。

1.  用户登录“消息通知服务”，单击“主题管理\>主题”，进入“主题”界面。
2.  在“主题”界面，单击“SMN-Test”消息主题名称，进入“主题详情页”。
3.  在“主题详情页”，单击“添加订阅”，弹出“添加订阅”界面。
4.  在“添加订阅”界面，填写订阅信息，如[表1](#table4277812911123)所示，带\*参数为必填项。

    **表 1**  订阅信息表

    <a name="table4277812911123"></a>
    <table><thead align="left"><tr id="row6452289411123"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p10222672111212"><a name="p10222672111212"></a><a name="p10222672111212"></a>字段</p>
    </th>
    <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p22730128111212"><a name="p22730128111212"></a><a name="p22730128111212"></a>填写说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3775359111123"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p29066614111212"><a name="p29066614111212"></a><a name="p29066614111212"></a>*协议</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p1753551895938"><a name="p1753551895938"></a><a name="p1753551895938"></a>从下列列表中选择“FunctionGraph（函数）”。</p>
    </td>
    </tr>
    <tr id="row1040996411123"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p4604418102450"><a name="p4604418102450"></a><a name="p4604418102450"></a>*订阅终端</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p23438155104255"><a name="p23438155104255"></a><a name="p23438155104255"></a>操作步骤如下。</p>
    <a name="ol63784051104119"></a><a name="ol63784051104119"></a><ol id="ol63784051104119"><li>单击“<a name="image12851510163510"></a><a name="image12851510163510"></a><span><img id="image12851510163510" src="figures/icon-add.png"></span>”，弹出“选择订阅终端”界面。</li><li>在“选择订阅终端”界面，选择<a href="代码上传方式创建HelloWorld函数.md">代码上传方式创建HelloWorld函数</a>中创建的HelloWorld函数。</li><li>单击“确定”。</li></ol>
    </td>
    </tr>
    <tr id="row38401286103746"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p10067254103746"><a name="p10067254103746"></a><a name="p10067254103746"></a>*版本</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p10141218103746"><a name="p10141218103746"></a><a name="p10141218103746"></a>从下拉列表中选择HelloWorld函数的版本，选择“latest”。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >添加订阅具体参数说明请参见[添加订阅](http://support.huaweicloud.com/usermanual-smn/zh-cn_topic_0043961402.html)。  

5.  单击“确定”，完成添加订阅。

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >为消息主题添加订阅时选择FunctionGraph类型协议，订阅终端选择HelloWorld函数，也就是为HelloWorld创建了SMN触发器。  


