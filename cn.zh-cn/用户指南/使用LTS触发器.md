# 使用LTS触发器<a name="ZH-CN_TOPIC_0149027432"></a>

本节介绍创建LTS触发器，供用户了解LTS触发器的使用方法。

关于LTS触发器事件源具体介绍请参见[支持的事件源](https://support.huaweicloud.com/devg-functiongraph/functiongraph_02_0102.html)。

## 前提条件<a name="section134592267445"></a>

-   已经在函数工作流服务创建函数，创建过程请参考[创建并初始化函数](创建并初始化函数.md)。
-   已经创建日志组，此处以LogGroup1为例，创建过程请参考[创建日志组](https://support.huaweicloud.com/usermanual-lts/lts_04_0003.html)。
-   已经创建日志流，此处以LogTopic1为例，创建过程请参考[创建日志流](https://support.huaweicloud.com/usermanual-lts/lts_04_0004.html)。
-   配置Agent，快速将ECS等服务器上日志采集到指定的日志组，详情请参考[安装Agent](https://support.huaweicloud.com/qs-lts/lts_0829.html)。

## 创建LTS触发器<a name="section198021231234"></a>

1.  登录FunctionGraph控制台，进入“函数”界面。
2.  在“函数”界面，选择“函数列表”，单击HelloWorld函数名称，进入HelloWorld函数详情界面。
3.  在HelloWorld函数详情界面，单击“触发器”页签。
4.  在“触发器”页签，单击“创建触发器”，弹出“创建触发器”对话框。
5.  设置以下信息。
    -   触发器类型：选择“云日志服务（LTS）”。
    -   日志组：选择已创建的日志组，例如：LogGroup1。
    -   日志主题：选择已创建的日志主题，例如：LogTopic1。

6.  单击“确定“，完成LTS触发器的创建。

## 配置LTS事件触发函数<a name="section15586193653118"></a>

1.  登录FunctionGraph控制台，进入“函数”界面。
2.  在“函数”界面，选择“函数列表”，单击HelloWorld函数名称，进入HelloWorld函数详情界面。
3.  在HelloWorld函数详情页，选择函数版本，单击“请选择测试事件 \> 配置测试事件”，弹出“配置测试事件”对话框。
4.  填写如[表1](#table15199135171812)所示测试信息后，单击“保存”。

    **表 1**  测试信息

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
    <td class="cellrowborder" valign="top" width="72%" headers="mcps1.2.3.1.2 "><p id="p519812511182"><a name="p519812511182"></a><a name="p519812511182"></a>选择"lts-event-template"模板，使用系统内置LTS事件模板。</p>
    </td>
    </tr>
    <tr id="row01981653188"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.3.1.1 "><p id="p619865201814"><a name="p619865201814"></a><a name="p619865201814"></a>事件名称</p>
    </td>
    <td class="cellrowborder" valign="top" width="72%" headers="mcps1.2.3.1.2 "><p id="p141661810113715"><a name="p141661810113715"></a><a name="p141661810113715"></a>事件名称必须以大写或小写字母开头，支持字母（大写或小写），数字和下划线“_”（或中划线“-”），并以字母或数字结尾，长度为1-25个字符，例如lts-123test。</p>
    </td>
    </tr>
    <tr id="row71991752189"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.2.3.1.1 "><p id="p81983518186"><a name="p81983518186"></a><a name="p81983518186"></a>测试事件</p>
    </td>
    <td class="cellrowborder" valign="top" width="72%" headers="mcps1.2.3.1.2 "><p id="p1419810515185"><a name="p1419810515185"></a><a name="p1419810515185"></a>自动加载系统内置lts事件模板，本例不做修改。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >测试事件模板示例如下：
    >```
    >{
    >    "lts": {
    >        "data": "ewogICAgICAgICJsb2dzIjpbewogICAgICAgICAgICAgICAgIm1lc3NhZ2UiOiIyMDE4LTA2LTI2LzE4OjQwOjUzIFtJTkZdIFtjb25maWcuZ286NzJdIFN1Y2Nlc3NmdWxseSBsb2FkZWQgZ2VuZXJhbCBjb25maWd1cmF0aW9uIGZpbGVcXHJcXG4iLAogICAgICAgICAgICAgICAgInRpbWUiOjE1MzAwMDk2NTMwNTksCiAgICAgICAgICAgICAgICAiaG9zdF9uYW1lIjoiZWNzLXRlc3RhZ2VudC5ub3ZhbG9jYWwiLAogICAgICAgICAgICAgICAgImlwIjoiMTkyLjE2OC4xLjk4IiwKICAgICAgICAgICAgICAgICJwYXRoIjoidXNyL2xvY2FsL3RlbGVzY29wZS9sb2cvY29tbW9uLmxvZyIsCiAgICAgICAgICAgICAgICAibG9nX3VpZCI6IjY2M2Q2OTMwLTc5MmQtMTFlOC04YjA4LTI4NmVkNDg4Y2U3MCIsCiAgICAgICAgICAgICAgICAibGluZV9ubyI6NjE1CiAgICAgICAgICAgIH0sCiAgICAgICAgICAgIHsKICAgICAgICAgICAgICAgICJtZXNzYWdlIjoiMjAxOC0wNi0yNi8xODo0MDo1MyBbV1JOXSBbY29uZmlnLmdvOjgyXSBUaGUgcHJvamVjdElkIG9yIGluc3RhbmNlSWQgb2YgY29uZmlnLmpzb24gaXMgbm90IGNvbnNpc3RlbnQgd2l0aCBtZXRhZGF0YSwgdXNlIG1ldGFkYXRhLlxcbiIsCiAgICAgICAgICAgICAgICAidGltZSI6MTUzMDAwOTY1MzA1OSwKICAgICAgICAgICAgICAgICJob3N0X25hbWUiOiJlY3MtdGVzdGFnZW50Lm5vdmFsb2NhbCIsCiAgICAgICAgICAgICAgICAiaXAiOiIxOTIuMTY4LjEuOTgiLAogICAgICAgICAgICAgICAgInBhdGgiOiIvdXNyL2xvY2FsL3RlbGVzY29wZS9sb2cvY29tbW9uLmxvZyIsCiAgICAgICAgICAgICAgICAibG9nX3VpZCI6IjY2M2Q2OTMwLTc5MmQtMTFlOC04YjA5LTI4NmVkNDg4Y2U3MCIsCiAgICAgICAgICAgICAgICAibGluZV9ubyI6NjE2CiAgICAgICAgICAgIH0sCiAgICAgICAgICAgIHsKICAgICAgICAgICAgICAgICJtZXNzYWdlIjoiIEluIGNvbmYuanNvbiwgcHJvamVjdElkIGlzIFtdLCBpbnN0YW5jZUlkIGlzIFtdLiBNZXRhRGF0YSBpcyB7NDU0MzI5M2EtNWIyYy00NGM0LWI3YTAtZGUyMThmN2YyZmE2IDYyODBlMTcwYmQ5MzRmNjBhNGQ4NTFjZjVjYTA1MTI5ICB9XFxyXFxuIiwKICAgICAgICAgICAgICAgICJ0aW1lIjoxNTMwMDA5NjUzMDU5LAogICAgICAgICAgICAgICAgImhvc3RfbmFtZSI6ImVjcy10ZXN0YWdlbnQubm92YWxvY2FsIiwKICAgICAgICAgICAgICAgICJpcCI6IjE5Mi4xNjguMS45OCIsCiAgICAgICAgICAgICAgICAicGF0aCI6Ii91c3IvbG9jYWwvdGVsZXNjb3BlL2xvZy9jb21tb24ubG9nIiwKICAgICAgICAgICAgICAgICJsb2dfdWlkIjoiNjYzZDY5MzAtNzkyZC0xMWU4LThiMGEtMjg2ZWQ0ODhjZTcwIiwKICAgICAgICAgICAgICAgICJsaW5lX25vIjo2MTcKICAgICAgICAgICAgfQogICAgICAgICAgICBdLAogICAgICAgICJvd25lciI6ICI2MjgwZTE3MGJkOTM0ZjYwYTRkODUxY2Y1Y2EwNTEyOSIsCiAgICAgICAgImxvZ19ncm91cF9pZCI6ICI5N2E5ZDI4NC00NDQ4LTExZTgtOGZhNC0yODZlZDQ4OGNlNzAiLAogICAgICAgICJsb2dfdG9waWNfaWQiOiAiMWE5Njc1YTctNzg0ZC0xMWU4LTlmNzAtMjg2ZWQ0ODhjZTcwIgogICAgICAgIH0="
    >    }
    >}
    >```

5.  单击“测试”，可以得到函数运行结果，函数会返回输入LTS数据。如[图1](#fig89541826201)所示。

    **图 1**  LTS触发器测试结果<a name="fig89541826201"></a>  
    ![](figures/LTS触发器测试结果.png "LTS触发器测试结果")


