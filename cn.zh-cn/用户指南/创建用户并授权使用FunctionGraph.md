# 创建用户并授权使用FunctionGraph<a name="ZH-CN_TOPIC_0170683656"></a>

如果您需要对您所拥有的FunctionGraph进行精细的权限管理，您可以使用[统一身份认证服务](https://support.huaweicloud.com/usermanual-iam/iam_01_0001.html)（Identity and Access Management，简称IAM），通过IAM，您可以：

-   根据企业的业务组织，在您的华为云账号中，给企业中不同职能部门的员工创建IAM用户，让员工拥有唯一安全凭证，并使用FunctionGraph资源。
-   根据企业用户的职能，设置不同的访问权限，以达到用户之间的权限隔离。
-   将FunctionGraph资源委托给更专业、高效的其他华为云账号或者云服务，这些账号或者云服务可以根据权限进行代运维。

如果华为云账号已经能满足您的要求，不需要创建独立的IAM用户，您可以跳过本章节，不影响您使用FunctionGraph服务的其它功能。

本章节为您介绍对用户授权的方法，操作流程如[图1](#fig484754213103)所示。

## 前提条件<a name="section0172163995812"></a>

-   “FunctionGraph Invoker”属于策略，请先在IAM控制台中开通基于策略的访问控制公测，开通方法请参见：[申请基于策略的访问控制公测](https://support.huaweicloud.com/usermanual-iam/iam_01_019.html)。
-   给用户组授权之前，请您了解用户组可以添加的FunctionGraph权限，并结合实际需求进行选择，FunctionGraph支持的系统权限，请参见[FunctionGraph系统策略](https://support.huaweicloud.com/productdesc-functiongraph/functiongraph_01_0160.html)。若您需要对除FunctionGraph之外的其它服务授权，IAM支持服务的所有权限请参见[系统权限](https://support.huaweicloud.com/permissions/policy_list.html?product=functiongraph)。

## 示例流程<a name="section73381480"></a>

**图 1**  给用户授权使用FunctionGraph权限的流程<a name="fig484754213103"></a>  
![](figures/给用户授权使用FunctionGraph权限的流程.png "给用户授权使用FunctionGraph权限的流程")

1.  <a name="li1113720874811"></a>[创建用户组并授权](https://support.huaweicloud.com/usermanual-iam/iam_03_0001.html)

    在IAM控制台创建用户组，并授予FunctionGraph查询及调用权限“FunctionGraph Invoker”。

2.  [创建用户并加入用户组](https://support.huaweicloud.com/usermanual-iam/iam_02_0001.html)

    在IAM控制台创建用户，并将其加入[1](#li1113720874811)中创建的用户组。

3.  [用户登录](https://support.huaweicloud.com/usermanual-iam/iam_01_0552.html)并验证权限

    新创建的用户登录控制台，验证FunctionGraph的函数查询权限。

    -   在“服务列表”中选择“函数工作流 FunctionGraph”，进入“函数列表”，单击“创建函数”进入到创建函数界面，发现无法创建函数，表示“FunctionGraph Invoker”已生效。
    -   在“服务列表”中选择除FunctionGraph外的任一服务，若提示权限不足，表示“FunctionGraph Invoker”已生效。


