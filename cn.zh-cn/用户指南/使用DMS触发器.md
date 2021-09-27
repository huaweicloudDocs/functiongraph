# 使用DMS触发器<a name="ZH-CN_TOPIC_0149027343"></a>

本节介绍创建DMS触发器，创建消息，触发函数运行。供用户了解DMS触发器的使用方法。

关于DMS触发器事件源具体介绍请参见[支持的事件源](https://support.huaweicloud.com/devg-functiongraph/functiongraph_02_0102.html)。

## 前提条件<a name="section76949209512"></a>

进行操作之前，需要做好以下准备。

-   已经创建消息队列和消费组，此处以队列queue-test、消费组group-dms为例，创建过程请参考[创建队列](https://support.huaweicloud.com/usermanual-dms/dms-ug-0312102.html)、[创建消费组](https://support.huaweicloud.com/usermanual-dms/dms-ug-0312103.html)。
-   已经在函数工作流服务创建函数，创建过程请参考[创建并初始化函数](创建并初始化函数.md)。

## 设置函数委托<a name="section82781591521"></a>

创建DMS触发器时，需要设置函数委托，委托权限需要包括DMS。如果不设置委托，无法加载已创建的DMS消息队列或者消息队列不可用，委托的创建请参考[创建委托](创建委托.md)。

由于创建HelloWorld函数的时候没有设置委托，所以需要先修改函数委托。

1.  登录FunctionGraph控制台，进入“函数”界面。
2.  在“函数”界面，选择“函数列表”，单击HelloWorld函数名称，进入HelloWorld函数详情界面。
3.  在HelloWorld函数详情页，单击“配置”，进入“配置”页签。
4.  在“配置”页签，修改函数委托，将委托修改为[创建委托](创建委托.md)中创建的serverless-trust委托。单击“保存”，完成委托修改。

## 创建DMS触发器<a name="section165781325165412"></a>

1.  登录FunctionGraph控制台，进入“函数”界面。
2.  在“函数”界面，选择“函数列表”，单击HelloWorld函数名称，进入HelloWorld函数详情界面。
3.  在HelloWorld函数详情界面，单击“触发器”页签。
4.  在“触发器”页签，单击“创建触发器”，弹出“创建触发器”对话框。
5.  设置以下信息。
    -   触发器类型：选择“分布式消息服务（DMS）”。
    -   队列：选择创建的队列，例如：queue-test。
    -   消费组：选择创建的消费组，例如：group-dms。
    -   拉取周期：拉取周期为DMS触发器轮询消息的间隔时间。

6.  单击“确定”，完成DMS触发器的创建。

## 创建消息触发函数<a name="section1291123565518"></a>

1.  登录“分布式消息服务”，进入“队列管理”界面。
2.  在“队列管理”界面，单击queue-test队列名称，进入队列详情页。
3.  在队列详情页，单击“生产消息”，弹出“生产消息”界面。
4.  在“生产消息”界面，填写消息信息，如[表1](#table4733472511323)所示。

    **表 1**  消息信息表

    <a name="table4733472511323"></a>
    <table><thead align="left"><tr id="row5730408111323"><th class="cellrowborder" valign="top" width="29.09%" id="mcps1.2.3.1.1"><p id="p1111897111323"><a name="p1111897111323"></a><a name="p1111897111323"></a>字段</p>
    </th>
    <th class="cellrowborder" valign="top" width="70.91%" id="mcps1.2.3.1.2"><p id="p2822147811323"><a name="p2822147811323"></a><a name="p2822147811323"></a>填写说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2397633311323"><td class="cellrowborder" valign="top" width="29.09%" headers="mcps1.2.3.1.1 "><p id="p6303480111323"><a name="p6303480111323"></a><a name="p6303480111323"></a>消息正文</p>
    </td>
    <td class="cellrowborder" valign="top" width="70.91%" headers="mcps1.2.3.1.2 "><p id="p554525011323"><a name="p554525011323"></a><a name="p554525011323"></a>输入以下内容：{"message":"hello"}。</p>
    </td>
    </tr>
    <tr id="row32449835105737"><td class="cellrowborder" valign="top" width="29.09%" headers="mcps1.2.3.1.1 "><p id="p23613064105737"><a name="p23613064105737"></a><a name="p23613064105737"></a>消息标签</p>
    </td>
    <td class="cellrowborder" valign="top" width="70.91%" headers="mcps1.2.3.1.2 "><p id="p33610009105737"><a name="p33610009105737"></a><a name="p33610009105737"></a>本例不填写。</p>
    </td>
    </tr>
    <tr id="row2169467111323"><td class="cellrowborder" valign="top" width="29.09%" headers="mcps1.2.3.1.1 "><p id="p1243788911323"><a name="p1243788911323"></a><a name="p1243788911323"></a>消息属性</p>
    </td>
    <td class="cellrowborder" valign="top" width="70.91%" headers="mcps1.2.3.1.2 "><p id="p83610411323"><a name="p83610411323"></a><a name="p83610411323"></a>本例不填写。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >生产消息具体参数介绍请参见[生产消息](https://support.huaweicloud.com/usermanual-dms/dms-ug-0312104.html)。

5.  单击“确定”，完成消息创建。
6.  在“消费组”栏的group-dms消费组可以查看“可消费消息数”。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >DMS触发器会按照[创建DMS触发器](#section165781325165412)中设置的拉取周期轮询消息，如果轮询到可消费消息，会消费消息，触发函数运行，具体示例事件请参见[支持的事件源](https://support.huaweicloud.com/devg-functiongraph/functiongraph_02_0102.html)。


## 查看函数运行结果<a name="section118763164575"></a>

1.  登录FunctionGraph控制台，进入“函数”界面。
2.  在“函数”界面，选择“函数列表”，单击HelloWorld函数名称，进入HelloWorld函数详情界面。
3.  在HelloWorld函数详情界面，单击“日志”页签，查询函数运行日志。
4.  单击操作栏的“查看上下文”，查看日志详细信息。

