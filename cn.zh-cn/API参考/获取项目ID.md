# 获取项目ID<a name="ZH-CN_TOPIC_0115410424"></a>

## 从控制台获取项目ID<a name="section1554791617113"></a>

在调用接口的时候，部分URL中需要填入项目ID，获取项目ID的步骤如下：

1.  注册并登录管理控制台。
2.  单击用户名，在下拉列表中单击“我的凭证”。

    在“我的凭证”页面，查看项目ID。


## 调用API获取项目ID<a name="section10510161913310"></a>

项目ID还用通过调用[查询指定条件下的项目信息](https://support.huaweicloud.com/api-iam/iam_06_0001.html)API获取。

获取项目ID的接口为“GET https://\{Endpoint\}/v3/projects”，其中\{Endpoint\}为IAM的终端节点，可以从[地区和终端节点](https://developer.huaweicloud.com/dev/endpoint)获取。接口的认证鉴权请参见[认证鉴权](认证鉴权.md)。

响应示例如下，其中projects下的“id”即为项目ID。

```
{
    "projects": [
        { 
            "domain_id": "65382450e8f64ac0870cd180d14e684b",
            "is_domain": false, 
            "parent_id": "65382450e8f64ac0870cd180d14e684b",
            "name": "xxx",
            "description": "",
            "links": {
                "next": null,
                "previous": null,
                "self": "https://www.example.com/v3/projects/a4a5d4098fb4474fa22cd05f897d6b99"
            },
            "id": "a4a5d4098fb4474fa22cd05f897d6b99",
            "enabled": true
        }
    ],
    "links": {
        "next": null,
        "previous": null,
        "self": "https://www.example.com/v3/projects"
    }
}
```

