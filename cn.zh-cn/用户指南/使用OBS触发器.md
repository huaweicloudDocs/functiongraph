# 使用OBS触发器<a name="ZH-CN_TOPIC_0149027251"></a>

本节介绍创建OBS触发器，上传图片压缩包至存储桶，产生事件触发函数运行，供用户了解OBS触发器的使用方法。

关于OBS触发器事件源具体介绍请参见[支持的事件源](http://support.huaweicloud.com/devg-functiongraph/functiongraph_02_0102.html)。

## 前提条件<a name="section76949209512"></a>

进行操作之前，需要做好以下准备。

-   已经在函数工作流服务创建函数，创建过程请参考[代码上传方式创建运行和初始化函数](代码上传方式创建运行和初始化函数.md)。
-   已创建OBS存储桶，此处以obs\_cff桶为例。创建过程请参考[创建存储桶](https://support.huaweicloud.com/usermanual-obs/zh-cn_topic_0045829050.html)。

## 创建OBS触发器<a name="section128720471905"></a>

1.  登录FunctionGraph控制台，进入“函数”界面。
2.  在“函数”界面，选择“函数列表”，单击HelloWorld函数名称，进入HelloWorld函数详情界面。
3.  在HelloWorld函数详情界面，单击“触发器”页签。
4.  在“触发器”页签，单击“创建触发器”，如[图1](#fig19176131502019)所示，弹出“创建触发器”界面。

    **图 1**  创建OBS触发器<a name="fig19176131502019"></a>  
    ![](figures/创建OBS触发器.png "创建OBS触发器")

5.  在“创建触发器”界面，触发器类型选择“存储 \(OBS\)”，填写触发器信息，如[表1](#table24155858113256)所示，带\*参数为必填项。

    **表 1**  OBS触发器信息表

    <a name="table24155858113256"></a>
    <table><thead align="left"><tr id="row24918708113256"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p20123023113339"><a name="p20123023113339"></a><a name="p20123023113339"></a>字段</p>
    </th>
    <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p19352141113339"><a name="p19352141113339"></a><a name="p19352141113339"></a>填写说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row30021527113256"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p15824598113256"><a name="p15824598113256"></a><a name="p15824598113256"></a>*桶</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p6724050113256"><a name="p6724050113256"></a><a name="p6724050113256"></a>用作事件源的OBS存储桶。</p>
    <p id="p13574750113452"><a name="p13574750113452"></a><a name="p13574750113452"></a>选择创建的obs-cff存储桶。</p>
    </td>
    </tr>
    <tr id="row60516450113256"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p2885379113256"><a name="p2885379113256"></a><a name="p2885379113256"></a>*事件</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p32389141113256"><a name="p32389141113256"></a><a name="p32389141113256"></a>要使其触发函数的事件。</p>
    <p id="p50102754113611"><a name="p50102754113611"></a><a name="p50102754113611"></a>此处以选择“Put”、“Post”和“Delete”为例，当对obs_cff桶中的文件进行更新、上传和删除操作时触发函数运行。</p>
    </td>
    </tr>
    <tr id="row23066815113256"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p56472765113256"><a name="p56472765113256"></a><a name="p56472765113256"></a>前缀</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p10891263113256"><a name="p10891263113256"></a><a name="p10891263113256"></a>用来限制以此关键字开头的对象的事件通知，该限制可以实现对OBS对象名的过滤，本例不设置。</p>
    </td>
    </tr>
    <tr id="row30912510113256"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p20885345113256"><a name="p20885345113256"></a><a name="p20885345113256"></a>后缀</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p13991422113256"><a name="p13991422113256"></a><a name="p13991422113256"></a>用来限制以此关键字结尾的对象的事件通知。该限制可以实现对OBS对象名的过滤，本例不设置。</p>
    </td>
    </tr>
    </tbody>
    </table>

6.  单击“确定”，完成触发器创建，如[图2](#fig17618154116211)所示。

    **图 2**  OBS触发器<a name="fig17618154116211"></a>  
    ![](figures/OBS触发器.png "OBS触发器")


## 触发函数<a name="section717210616119"></a>

1.  用户登录“对象存储服务”，单击“桶列表”中的“obs-cff”存储桶，进入obs-cff桶详情页。
2.  单击左侧的“对象”，进入“obs-cff”存储桶对象页。
3.  在“对象”页签，单击“上传文件”，弹出“上传文件”框。
4.  在“上传文件”框中单击“...” ，选择需要处理的图片ZIP包上传至平台。
5.  单击“确定”，完成上传ZIP包完成，如[图3](#fig17104220153625)所示。

    **图 3**  对象列表<a name="fig17104220153625"></a>  
    ![](figures/对象列表.png "对象列表")

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >上传ZIP文件至“obs-cff”存储桶，会触发HelloWorld函数运行。  


## 查看函数运行结果<a name="section192251225017"></a>

1.  登录FunctionGraph控制台，进入“函数”界面。
2.  在“函数”界面，选择“函数列表”，单击HelloWorld函数名称，进入HelloWorld函数详情界面。
3.  在HelloWorld函数详情界面，单击“日志”页签，查询函数运行日志。
4.  单击操作栏的“查看上下文”，查看日志详细信息。

