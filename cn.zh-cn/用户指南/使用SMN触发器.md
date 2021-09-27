# 使用SMN触发器<a name="ZH-CN_TOPIC_0149027257"></a>

本节介绍创建SMN触发器，发布消息，触发函数运行，供用户了解SMN触发器的使用方法。

关于SMN触发器事件源具体介绍请参见[支持的事件源](https://support.huaweicloud.com/devg-functiongraph/functiongraph_02_0102.html)。

## 前提条件<a name="section76949209512"></a>

-   已经创建SMN消息主题，此处以smn-test为例，创建过程请参考[创建消息主题](https://support.huaweicloud.com/usermanual-smn/zh-cn_topic_0043961401.html)。
-   已经在函数工作流服务创建函数，创建过程请参考[创建并初始化函数](创建并初始化函数.md)。

## 创建SMN触发器<a name="section08737499488"></a>

1.  登录FunctionGraph控制台，进入“函数”界面。
2.  在“函数”界面，选择“函数列表”，单击HelloWorld函数名称，进入HelloWorld函数详情界面。
3.  在HelloWorld函数详情界面，单击“触发器”页签。
4.  在“触发器”页签，单击“创建触发器”，弹出“创建触发器”对话框。
5.  设置以下信息。
    -   触发器类型：选择“消息队列服务 \(SMN\)”。
    -   主题名称：选择主题名称，例如：smn-test。

6.  单击“确定”，完成SMN触发器的创建。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >SMN触发器创建完成后，会在SMN消息主题生成消息订阅。


## 触发函数运行<a name="section720713914918"></a>

在“消息通知服务”控制台，为“smn-test”主题发布消息，具体操作步骤请参考[向主题发布文本消息](https://support.huaweicloud.com/usermanual-smn/zh-cn_topic_0043961403.html)。

发布消息的内容参考[表1](#table833644511032)填写。

**表 1**  发布消息

<a name="table833644511032"></a>
<table><thead align="left"><tr id="row289324011032"><th class="cellrowborder" valign="top" width="26.090000000000003%" id="mcps1.2.3.1.1"><p id="p3302586011032"><a name="p3302586011032"></a><a name="p3302586011032"></a>字段</p>
</th>
<th class="cellrowborder" valign="top" width="73.91%" id="mcps1.2.3.1.2"><p id="p5784902911032"><a name="p5784902911032"></a><a name="p5784902911032"></a>填写说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row5525981111032"><td class="cellrowborder" valign="top" width="26.090000000000003%" headers="mcps1.2.3.1.1 "><p id="p4685971711032"><a name="p4685971711032"></a><a name="p4685971711032"></a>消息标题</p>
</td>
<td class="cellrowborder" valign="top" width="73.91%" headers="mcps1.2.3.1.2 "><p id="p3754075611032"><a name="p3754075611032"></a><a name="p3754075611032"></a>输入“SMN-Test”。</p>
</td>
</tr>
<tr id="row232248711032"><td class="cellrowborder" valign="top" width="26.090000000000003%" headers="mcps1.2.3.1.1 "><p id="p5390379611032"><a name="p5390379611032"></a><a name="p5390379611032"></a>消息类型</p>
</td>
<td class="cellrowborder" valign="top" width="73.91%" headers="mcps1.2.3.1.2 "><p id="p3251789511642"><a name="p3251789511642"></a><a name="p3251789511642"></a>选择“文本消息”。</p>
</td>
</tr>
<tr id="row2555605011032"><td class="cellrowborder" valign="top" width="26.090000000000003%" headers="mcps1.2.3.1.1 "><p id="p5677420111032"><a name="p5677420111032"></a><a name="p5677420111032"></a>消息内容</p>
</td>
<td class="cellrowborder" valign="top" width="73.91%" headers="mcps1.2.3.1.2 "><p id="p3530753111032"><a name="p3530753111032"></a><a name="p3530753111032"></a>输入以下内容：{"message":"hello"}。</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>消息发布以后，会自动触发函数运行，具体示例事件请参见[支持的事件源](https://support.huaweicloud.com/devg-functiongraph/functiongraph_02_0102.html)。

## 查看函数运行结果<a name="section21041145184920"></a>

1.  登录FunctionGraph控制台，进入“函数”界面。
2.  在“函数”界面，选择“函数列表”，单击HelloWorld函数名称，进入HelloWorld函数详情界面。
3.  在HelloWorld函数详情界面，单击“日志”页签，查询函数运行日志。
4.  单击操作栏的“查看上下文”，查看日志详细信息。

