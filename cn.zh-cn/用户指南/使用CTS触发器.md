# 使用CTS触发器<a name="ZH-CN_TOPIC_0149027283"></a>

本节介绍创建CTS触发器，通过增加自定义操作，触发函数运行，通过CTS云审计服务获取操作记录，供用户了解CTS触发器的使用方法。

关于CTS触发器事件源具体介绍请参见[支持的事件源](https://support.huaweicloud.com/devg-functiongraph/functiongraph_02_0102.html)。

## 前提条件<a name="section97094317346"></a>

已经在统一身份认证创建委托，创建过程请参考[创建委托](创建委托.md)。

## 创建CTS触发器<a name="section1079628104617"></a>

1.  登录FunctionGraph控制台，在左侧导航栏选择“函数 \> 函数列表”，进入函数列表界面。
2.  单击“创建函数”，进入“创建函数”界面。
3.  设置以下函数信息。
    -   模板：选择“使用空模板”。
    -   函数名称：输入您自定义的函数名称，例如：HelloWorld。
    -   所属应用：选择“default”。
    -   委托名称：选择“不使用任何委托”。
    -   描述：输入对函数的补充信息，可以不填。
    -   运行时语言：选择“Python 2.7”。
    -   函数执行入口：输入“index.handler”。
    -   代码上传方式：选择“在线编辑”，并输入如下所示的代码，代码中的参数请根据实际情况填写。

        ```
        # -*- coding:utf-8 -*-
        '''
        CTS trigger event:
        {
          "cts":  {
                "time": "",
                "user": {
                    "name": "userName",
                    "id": "",
                    "domain": {
                        "name": "domainName",
                        "id": ""
                    }
                },
                "request": {},
                "response": {},
                "code": 204,
                "service_type": "FunctionGraph",
                "resource_type": "",
                "resource_name": "",
                "resource_id": {},
                "trace_name": "",
                "trace_type": "ConsoleAction",
                "record_time": "",
                "trace_id": "",
                "trace_status": "normal"
            }
        }
        '''
        def handler (event, context):
            trace_name = event["cts"]["resource_name"]
            timeinfo = event["cts"]["time"]
        print(timeinfo+' '+trace_name)
        ```

4.  单击“创建函数”，完成函数的创建。
5.  在“触发器”页签，单击“创建触发器”。
6.  设置以下触发器信息。

    **表 1**  触发器信息

    <a name="table1682181464418"></a>
    <table><thead align="left"><tr id="row181914164413"><th class="cellrowborder" valign="top" width="22.34%" id="mcps1.2.3.1.1"><p id="p1381101413445"><a name="p1381101413445"></a><a name="p1381101413445"></a>字段</p>
    </th>
    <th class="cellrowborder" valign="top" width="77.66%" id="mcps1.2.3.1.2"><p id="p9818143441"><a name="p9818143441"></a><a name="p9818143441"></a>填写说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1572625334418"><td class="cellrowborder" valign="top" width="22.34%" headers="mcps1.2.3.1.1 "><p id="p272712538443"><a name="p272712538443"></a><a name="p272712538443"></a>触发器类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="77.66%" headers="mcps1.2.3.1.2 "><p id="p1372735315444"><a name="p1372735315444"></a><a name="p1372735315444"></a>选择“云审计服务（CTS）”。</p>
    </td>
    </tr>
    <tr id="row14815149447"><td class="cellrowborder" valign="top" width="22.34%" headers="mcps1.2.3.1.1 "><p id="p3811214184410"><a name="p3811214184410"></a><a name="p3811214184410"></a>通知名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="77.66%" headers="mcps1.2.3.1.2 "><p id="p13811414134419"><a name="p13811414134419"></a><a name="p13811414134419"></a>输入您自定义的通知名称，例如：Test。</p>
    </td>
    </tr>
    <tr id="row1827147443"><td class="cellrowborder" valign="top" width="22.34%" headers="mcps1.2.3.1.1 "><p id="p3821214174412"><a name="p3821214174412"></a><a name="p3821214174412"></a>服务类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="77.66%" headers="mcps1.2.3.1.2 "><p id="p1382181411440"><a name="p1382181411440"></a><a name="p1382181411440"></a>选择“FunctionGraph”。</p>
    </td>
    </tr>
    <tr id="row482131434413"><td class="cellrowborder" valign="top" width="22.34%" headers="mcps1.2.3.1.1 "><p id="p28241412445"><a name="p28241412445"></a><a name="p28241412445"></a>资源类型</p>
    </td>
    <td class="cellrowborder" valign="top" width="77.66%" headers="mcps1.2.3.1.2 "><p id="p138210145444"><a name="p138210145444"></a><a name="p138210145444"></a>所选服务下对应的资源类型，如触发器、实例、函数等。</p>
    </td>
    </tr>
    <tr id="row1382151411448"><td class="cellrowborder" valign="top" width="22.34%" headers="mcps1.2.3.1.1 "><p id="p158261454420"><a name="p158261454420"></a><a name="p158261454420"></a>操作名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="77.66%" headers="mcps1.2.3.1.2 "><p id="p18271416446"><a name="p18271416446"></a><a name="p18271416446"></a>所选资源类型下对应的操作，如创建、删除触发器等。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >CTS触发器最多支持添加10个服务，每个服务10个操作，总共可添加100个操作，服务及操作详情可参考[支持审计的服务及详细操作列表](https://support.huaweicloud.com/usermanual-cts/cts_03_0030.html)。  

7.  单击“确定”，完成CTS触发器的创建。

## 配置CTS事件触发函数<a name="section1581734219447"></a>

1.  在HelloWorld函数详情页，选择函数版本，单击“请选择测试事件 \> 配置测试事件”，弹出“配置测试事件”对话框。
2.  填写如[表2](#table19101881852)所示测试信息后，单击“保存”。

    **表 2**  测试信息

    <a name="table19101881852"></a>
    <table><thead align="left"><tr id="row18991818517"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p1199882517"><a name="p1199882517"></a><a name="p1199882517"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p1399481516"><a name="p1399481516"></a><a name="p1399481516"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row15991688510"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p99910817514"><a name="p99910817514"></a><a name="p99910817514"></a>配置测试事件</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p699481551"><a name="p699481551"></a><a name="p699481551"></a>可创建新的测试事件也可编辑已有的测试事件。</p>
    <p id="p189928655"><a name="p189928655"></a><a name="p189928655"></a>选择“创建新的测试事件”。</p>
    </td>
    </tr>
    <tr id="row17100881156"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p19988857"><a name="p19988857"></a><a name="p19988857"></a>事件模板</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p3991681155"><a name="p3991681155"></a><a name="p3991681155"></a>选择“cts-event-template”模板，使用系统内置CTS事件模板。</p>
    </td>
    </tr>
    <tr id="row15100481555"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p410058956"><a name="p410058956"></a><a name="p410058956"></a>事件名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p010028051"><a name="p010028051"></a><a name="p010028051"></a>您自定义的事件名称，例如：cts-test。</p>
    </td>
    </tr>
    <tr id="row111012081952"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p14100208953"><a name="p14100208953"></a><a name="p14100208953"></a>测试事件</p>
    </td>
    <td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p14100881055"><a name="p14100881055"></a><a name="p14100881055"></a>自动加载系统内置CTS事件模板，您可以根据实际情况修改。</p>
    </td>
    </tr>
    </tbody>
    </table>

3.  单击“测试”，可以得到函数运行结果记录。

