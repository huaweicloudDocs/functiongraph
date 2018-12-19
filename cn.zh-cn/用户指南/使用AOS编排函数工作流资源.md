# 使用AOS编排函数工作流资源<a name="functiongraph_01_0405"></a>

应用编排服务（Application Orchestration Service，简称AOS）可以帮助您将应用一键式部署到华为云上，简化相关云服务管理操作。AOS通过模板来描述和编排应用及相关云服务，实现自动化部署应用、创建云服务，提供E2E应用全生命周期运维管控能力。

FunctionGraph工作流实现了华为应用编排服务AOS的对接，可以通过AOS编排服务将云资源一键式部署到华为云上，实现业务流程自动化。

使用AOS编排服务编排FunctionGraph资源，可以实现以下功能：

-   通过AOS模板创建堆栈来管理函数资源。
-   通过AOS模板创建堆栈来管理触发器资源。
-   结合其他华为云服务，编排复杂云资源集合。

## 场景介绍<a name="section83889103414"></a>

本案例所示图片处理后端应用是基于函数工作流FunctionGraph实现图片打水印功能的无服务系统。通过OBS触发器，对每个上传到OBS桶中的图片打水印，再将水印图片存储到另一个OBS桶中。

本案例通过AOS编排服务的设计器编排部署图片处理后端应用所需的FunctionGraph资源和OBS桶资源，实现快速构建图片处理后端应用。设计器编排完成后，可以生成一个模板，基于该模板可一键创建多个图片处理后端应用。

创建图片处理后端应用，需要编排的云资源包括：

-   FunctionGraph工作流函数资源
-   FunctionGraph工作流OBS触发器资源
-   OBS桶资源

## 准备<a name="section19845154719231"></a>

AOS编排函数资源，函数的代码上传支持在线编辑和OBS上传文件两种方式，本案例以OBS上传文件方式为例，先将函数代码上传至OBS桶，并获取代码在OBS桶中的地址。

1、创建OBS桶

用户登录华为云控制台，进入“[对象存储服务](https://storage.huaweicloud.com/obs/)”，单击“创建桶”，进入“创建桶”界面。

在“创建桶”界面，填写存储桶信息，如[图1](#fig1774412644714)所示。

区域选择：“华北-北京一”

桶名称输入：“obs-mycode”

存储别选择：“标准存储”

桶策略选择："私有"

**图 1**  创建桶<a name="fig1774412644714"></a>  
![](figures/创建桶.png "创建桶")

单击“立即创建“，完成桶的创建。

2、上传函数代码至OBS桶

选择上一步骤创建的OBS桶，将ZIP格式的[函数代码](https://functionstage-examples.obs.myhwclouds.com/fss_examples_image_watermark.zip)上传至该OBS桶中，记录下函数代码在OBS桶中的地址。本例ZIP格式的函数代码文件名称为“fss\_examples\_image\_watermark.zip”。

**图 2**  上传函数代码<a name="fig3263163455510"></a>  
![](figures/上传函数代码.png "上传函数代码")

**图 3**  OBS桶中函数代码的地址<a name="fig1516442316019"></a>  
![](figures/OBS桶中函数代码的地址.png "OBS桶中函数代码的地址")

3、配置函数委托

因为函数需要访问OBS服务，所以需要给予函数访问OBS的权限，为函数设置OBS的委托。同样，在函数中需要获取IAM提供的用户AK、SK，所以也需要设置IAM的委托，配置的委托名称需填入后续配置模板参数中。具体操作请参考[创建委托](https://support.huaweicloud.com/bestpractice-functiongraph/functiongraph_05_0401.html)。

## 导入AOS模板<a name="section33649418811"></a>

建议通过导入现有的AOS模板来编排函数工作流服务资源。我们将提供一些典型应用场景的AOS公共模板来帮助您快速创建堆栈，您可将AOS模板直接导入AOS设计器，然后根据业务情况修改AOS模板的具体配置。如您需要自行通过AOS设计器设计AOS模板，可参考AOS服务[帮助文档](https://support.huaweicloud.com/usermanual-aos/aos_01_0000.html)。

本例的完整AOS模板可[点此下载](https://functionstage-examples.obs.cn-north-1.myhwclouds.com/blueprint-function-watermark.yaml)，在AOS设计器中点击页面顶部的“打开”按钮，将下载的AOS模板导入AOS设计器，然后单击设计器页面顶部的“保存”按钮，输入以下参数，单击“保存”。

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   保存模板前，您可单击![](figures/icon-check.png)进行模板校验。若模板正确，在“操作日志”中会提示校验模板成功。  
>-   模板名称：自定义模板名称，需确保全局唯一，例如设置为blueprint-function-watermark。  
>-   版本：1.0，保持默认。  

**图 4**  保存AOS模板<a name="fig845494641813"></a>  
![](figures/保存AOS模板.png "保存AOS模板")

## 部署云资源<a name="section1065818226204"></a>

1.  单击设计器页面右上侧的![](figures/icon-delete.png)，进入AOS控制台首页。
2.  在左侧导航栏中，选择“我的模板”。在模板列表中可查看到保存成功的模板blueprint-function-watermark。
3.  单击blueprint-function-watermark模板后的“部署堆栈”。
4.  设置堆栈信息。
    -   堆栈名称：输入堆栈名称，例如**image-watermark**，需确保该值唯一。
    -   描述：可选。
    -   配置输入参数，如[表1](#table14183337372)。

        **表 1**  配置输入参数

        <a name="table14183337372"></a>
        <table><thead align="left"><tr id="row171801934375"><th class="cellrowborder" valign="top" width="24%" id="mcps1.2.3.1.1"><p id="p318011313717"><a name="p318011313717"></a><a name="p318011313717"></a><strong id="b181803316379"><a name="b181803316379"></a><a name="b181803316379"></a>参数</strong></p>
        </th>
        <th class="cellrowborder" valign="top" width="76%" id="mcps1.2.3.1.2"><p id="p21808383718"><a name="p21808383718"></a><a name="p21808383718"></a><strong id="b1180234379"><a name="b1180234379"></a><a name="b1180234379"></a>说明</strong></p>
        </th>
        </tr>
        </thead>
        <tbody><tr id="row818020353714"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.3.1.1 "><p id="p3180123143718"><a name="p3180123143718"></a><a name="p3180123143718"></a>codeUrl</p>
        </td>
        <td class="cellrowborder" valign="top" width="76%" headers="mcps1.2.3.1.2 "><p id="p518017315378"><a name="p518017315378"></a><a name="p518017315378"></a>函数代码包在OBS上的地址，需手动输入</p>
        </td>
        </tr>
        <tr id="row1018053153717"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.3.1.1 "><p id="p1118043183719"><a name="p1118043183719"></a><a name="p1118043183719"></a>handler</p>
        </td>
        <td class="cellrowborder" valign="top" width="76%" headers="mcps1.2.3.1.2 "><p id="p1318015316372"><a name="p1318015316372"></a><a name="p1318015316372"></a>函数执行入口，采用默认值index.handler即可</p>
        </td>
        </tr>
        <tr id="row1418033163717"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.3.1.1 "><p id="p918013315373"><a name="p918013315373"></a><a name="p918013315373"></a>memorySize</p>
        </td>
        <td class="cellrowborder" valign="top" width="76%" headers="mcps1.2.3.1.2 "><p id="p2180031371"><a name="p2180031371"></a><a name="p2180031371"></a>函数消耗的内存，默认128MB</p>
        </td>
        </tr>
        <tr id="row19180834373"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.3.1.1 "><p id="p4180203103712"><a name="p4180203103712"></a><a name="p4180203103712"></a>name</p>
        </td>
        <td class="cellrowborder" valign="top" width="76%" headers="mcps1.2.3.1.2 "><p id="p11808315376"><a name="p11808315376"></a><a name="p11808315376"></a>函数名称，默认image_watermark，可自行配置</p>
        </td>
        </tr>
        <tr id="row141823383714"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.3.1.1 "><p id="p318211312375"><a name="p318211312375"></a><a name="p318211312375"></a>runtime</p>
        </td>
        <td class="cellrowborder" valign="top" width="76%" headers="mcps1.2.3.1.2 "><p id="p218218303718"><a name="p218218303718"></a><a name="p218218303718"></a>函数的执行环境，选择Python2.7</p>
        </td>
        </tr>
        <tr id="row618214315371"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.3.1.1 "><p id="p218214315377"><a name="p218214315377"></a><a name="p218214315377"></a>xrole</p>
        </td>
        <td class="cellrowborder" valign="top" width="76%" headers="mcps1.2.3.1.2 "><p id="p141825393720"><a name="p141825393720"></a><a name="p141825393720"></a>函数委托名称，输入前面步骤创建的委托名称</p>
        </td>
        </tr>
        <tr id="row20182638377"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.3.1.1 "><p id="p2018273113716"><a name="p2018273113716"></a><a name="p2018273113716"></a>timeout</p>
        </td>
        <td class="cellrowborder" valign="top" width="76%" headers="mcps1.2.3.1.2 "><p id="p1018218315374"><a name="p1018218315374"></a><a name="p1018218315374"></a>函数的超时时间，默认3秒</p>
        </td>
        </tr>
        </tbody>
        </table>

        **图 5**  堆栈参数配置<a name="fig141831735372"></a>  
        ![](figures/堆栈参数配置.png "堆栈参数配置")


5.  单击“下一步”，查看堆栈信息，确认无误后，单击“创建堆栈”。

    系统自动跳转到堆栈详情页面，可查看到当前堆栈为创建中。此处创建了函数、OBS触发器和两个OBS桶。

6.  待堆栈状态为“正常”时，可查看到堆栈元素中已有三个云服务资源。函数、OBS触发器以及OBS桶创建成功。

    **图 6**  堆栈已创建成功<a name="fig2713251193918"></a>  
    ![](figures/堆栈已创建成功.png "堆栈已创建成功")

7.  查看已创建的云服务。
    1.  登录华为云控制台。
    2.  选择“计算 \> 函数工作流FunctionGraph”，可查看到已创建成功一个带OBS触发器的函数。
    3.  选择“存储 \> 对象存储服务OBS”，可查看到自动创建的两个OBS桶。


## 验证<a name="section848572224112"></a>

1、进入OBS页面，向前面步骤创建的用于存储待处理图片的OBS桶中上传图片，本例中上传一张郁金香花的图片。

**图 7**  待上传的图片<a name="fig1044442244315"></a>  
![](figures/待上传的图片.png "待上传的图片")

**图 8**  上传待处理的图片至OBS桶<a name="fig8530202312441"></a>  
![](figures/上传待处理的图片至OBS桶.png "上传待处理的图片至OBS桶")

2、上传完成后，进入存储水印图片的OBS桶，查看图片打水印的结果。

**图 9**  处理后的带水印图片<a name="fig1912214421463"></a>  
![](figures/处理后的带水印图片.png "处理后的带水印图片")

**图 10**  处理后OBS桶<a name="fig22948584465"></a>  
![](figures/处理后OBS桶.png "处理后OBS桶")

