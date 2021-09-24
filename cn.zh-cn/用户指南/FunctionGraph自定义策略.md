# FunctionGraph自定义策略<a name="ZH-CN_TOPIC_0215517245"></a>

如果系统预置的FunctionGraph权限，不满足您的授权要求，可以创建自定义策略。

目前华为云支持以下两种方式创建自定义策略：

-   可视化视图创建自定义策略：无需了解策略语法，按可视化视图导航栏选择云服务、操作、资源、条件等策略内容，可自动生成策略。
-   JSON视图创建自定义策略：可以在选择策略模板后，根据具体需求编辑策略内容；也可以直接在编辑框内编写JSON格式的策略内容。

具体创建步骤请参见：[创建自定义策略](https://support.huaweicloud.com/usermanual-iam/iam_01_0605.html)。本章为您介绍常用的FunctionGraph自定义策略样例。

## FunctionGraph自定义策略样例<a name="section198210477557"></a>

-   示例1：授权用户查询函数代码和配置

    ```
    {     
        "Version": "1.1",     
        "Statement": [         
            {             
                "Effect": "Allow",            
                "Action": [
                   "functiongraph:function:list",
                   "functiongraph:function:getConfig",
                   "funcitongraph:function:getCode"             
                ]        
             }     
        ] 
    }
    ```

-   示例2：拒绝用户删除函数

    拒绝策略需要同时配合其他策略使用，否则没有实际作用。用户被授予的策略中，一个授权项的作用如果同时存在Allow和Deny，则遵循Deny优先。

    如果您给用户授予FunctionGraph FullAccess的系统策略，但不希望用户拥有FunctionGraph FullAccess中定义的删除函数权限，您可以创建一条拒绝删除函数的自定义策略，然后同时将FunctionGraph FullAccess和拒绝策略授予用户，根据Deny优先原则，则用户可以对FunctionGraph执行除了删除函数外的所有操作。拒绝策略示例如下：

    ```
    {
        "Version": "1.1",
        "Statement": [
            "Effect": "Deny",
            "Action": [
                "functiongraph:function:delete" 
            ] 
        ]
    }
    ```

-   示例3：特定资源权限配置

    特定资源：授予IAM用户特定资源的相应权限。例如授予IAM用户所属应用Default下函数functionname的相应权限，需将函数functionname设置为指定资源路径，添加资源路径：FUNCTIONGRAPH:\*:\*:function:Default/functionname。

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >指定函数资源：
    >【格式】FUNCTIONGRAPH:\*:\*:function:所属应用/函数名称
    >对于函数资源，IAM自动生成资源路径前缀“FUNCTIONGRAPH:\*:\*:function:”。通过所属应用和函数名称指定具体的资源路径，支持通配符\*。例如：FUNCTIONGRAPH:\*:\*:function:Default/\*表示Default应用下的任意函数。

    ```
    {
        "Version": "1.1",
        "Statement": [
            {
                "Effect": "Allow",
                "Action": [
                    "functiongraph:function:list"
                ]
            },
            {
                "Effect": "Allow",
                "Action": [
                    "functiongraph:function:listAlias",
                    "functiongraph:function:listVersion",
                    "functiongraph:function:getConfig",
                    "functiongraph:function:getCode",
                    "functiongraph:function:updateCode",
                    "functiongraph:function:invoke",
                    "functiongraph:function:updateConfig",
                    "functiongraph:function:createVersion",
                    "functiongraph:function:updateAlias",
                    "functiongraph:function:createAlias"
                ],
                "Resource": [
                    "FUNCTIONGRAPH:*:*:function:Default/*"
                ]
            }
        ]
    }
    ```


