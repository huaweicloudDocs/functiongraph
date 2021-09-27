# 使用OBS触发器<a name="ZH-CN_TOPIC_0149027251"></a>

本节介绍创建OBS触发器，上传图片压缩包至存储桶，产生事件触发函数运行，供用户了解OBS触发器的使用方法。

关于OBS触发器事件源具体介绍请参见[支持的事件源](https://support.huaweicloud.com/devg-functiongraph/functiongraph_02_0102.html)。

## 前提条件<a name="section76949209512"></a>

进行操作之前，需要做好以下准备。

-   已经在函数工作流服务创建函数，创建过程请参考[创建并初始化函数](创建并初始化函数.md)。
-   已创建OBS存储桶，此处以obs\_cff桶为例。创建过程请参考[创建存储桶](https://support.huaweicloud.com/usermanual-obs/obs_03_0306.html)。

## 创建OBS触发器<a name="section128720471905"></a>

1.  登录FunctionGraph控制台，进入“函数”界面。
2.  在“函数”界面，选择“函数列表”，单击HelloWorld函数名称，进入HelloWorld函数详情界面。
3.  在HelloWorld函数详情界面，单击“触发器”页签。
4.  在“触发器”页签，单击“创建触发器”，弹出“创建触发器”对话框。
5.  设置以下信息。
    -   触发器类型：选择“存储 \(OBS\)”。
    -   桶：用作事件源的OBS存储桶，例如：obs-cff。
    -   事件：选择触发函数的事件。此处以选择“Put”、“Post”和“Delete”为例，当对obs\_cff桶中的文件进行更新、上传和删除操作时触发函数运行。
    -   事件通知名称：您自定义的事件通知名称，用于在事件发生时，SMN给您推送消息。
    -   前缀：用来限制以此关键字开头的对象的事件通知，该限制可以实现对OBS对象名的过滤。
    -   后缀：用来限制以此关键字结尾的对象的事件通知，该限制可以实现对OBS对象名的过滤。

6.  单击“确定”，完成OBS触发器的创建。

## 触发函数<a name="section717210616119"></a>

在“对象存储服务”控制台，将需要处理的图片ZIP包上传至“obs-cff”存储桶，具体上传步骤请参考[上传文件](https://support.huaweicloud.com/usermanual-obs/zh-cn_topic_0045829661.html)。

>![](public_sys-resources/icon-note.gif) **说明：** 
>上传ZIP文件至“obs-cff”存储桶，会触发HelloWorld函数运行。

## 查看函数运行结果<a name="section192251225017"></a>

1.  登录FunctionGraph控制台，进入“函数”界面。
2.  在“函数”界面，选择“函数列表”，单击HelloWorld函数名称，进入HelloWorld函数详情界面。
3.  在HelloWorld函数详情界面，单击“日志”页签，查询函数运行日志。
4.  单击操作栏的“查看上下文”，查看日志详细信息。

