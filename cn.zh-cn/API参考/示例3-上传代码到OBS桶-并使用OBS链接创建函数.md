# 示例3：上传代码到OBS桶，并使用OBS链接创建函数<a name="ZH-CN_TOPIC_0255589313"></a>

## 场景描述<a name="section11773144817815"></a>

本章节以Python 2.7为例，指导您在本地编码，然后将代码文件上传到OBS桶，实现通过OBS链接创建函数。

API的调用方法请参见[如何调用API](如何调用API.md)。

## 前提条件<a name="section1835181812285"></a>

已在OBS服务中创建OBS桶。

## 总体思路<a name="section780392783814"></a>

在本地进行函数编码后，将代码文件上传到OBS桶，并使用OBS链接创建函数。步骤如下：

1.  创建函数工程：在本地进行编码实现函数功能。
2.  上传工程到OBS桶：将代码文件压缩为zip格式并上传到已创建的OBS桶中，记录代码文件的OBS链接。
3.  [创建函数](创建函数.md)：调用API通过OBS链接创建函数。

## 步骤1：创建函数工程<a name="section14741921773"></a>

1.  编写打印helloworld的代码。

    打开文本编辑器，编写helloworld函数，代码如下，文件命名为“helloworld.py”，保存文件。

    ```
    def printhello(): 
        print 'Hello world!' 
    ```

2.  定义FunctionGraph函数。

    打开文本编辑器，定义函数，代码如下，文件命名为“index.py”，保存文件（与“helloworld.py”保存在同一文件夹下）。

    ```
    import json 
    import helloworld 
     
    def handler (event, context): 
        output =json.dumps(event) 
        helloworld.printhello() 
        return output
    ```


## 步骤2：上传工程到OBS桶<a name="section17199193504710"></a>

1.  在函数工程中，选中“helloworld.py”和“index.py”文件，打包压缩为“fss\_examples\_python2.7.zip”。
2.  <a name="li1966633145116"></a>上传“fss\_examples\_python2.7.zip”到OBS桶，记录OBS链接。

## 步骤3：调用创建函数API，使用OBS链接创建函数<a name="section20413632205210"></a>

URI：POST /v2/\{project\_id\}/fgs/functions

API文档详情请参见：[创建函数](创建函数.md)

-   请求示例

    ```
    POST  https://{Endpoint}/v2/{project_id}/fgs/functions
    {
     "code_type": "obs",
     "code_url": "https://test.obs.xxx.xxx.com/fss_examples_python2.7.zip",
     "func_name": "create_function_from_obs",
     "handler": "index.handler",
     "memory_size": 256,
     "package": "default",
     "runtime": "Python2.7",
     "timeout": 30
    }
    ```

    “code\_url”为[2](#li1966633145116)中记录的OBS链接。

-   响应示例

    ```
    {
     "func_urn": "urn:fss:{project_name}:{project_id}:function:default:create_function_from_obs:latest",
     "func_name": "create_function_from_obs",
     "domain_id": "0503xxxa960",
     "namespace": "{project_id}",
     "project_name": "xxx",
     "package": "default",
     "runtime": "Python2.7",
     "timeout": 30,
     "handler": "index.handler",
     "memory_size": 256,
     "cpu": 400,
     "code_type": "obs",
     "code_url": "https://test.obs.xxx.xxx.com/fss_examples_python2.7.zip",
     "code_filename": "fss_examples_python2.7.zip",
     "code_size": 436,
     "digest": "3af770ada27514564b1a20d964cba4b35f432fa40f9fc4f4f7c1f0d2f42eac6cb4db1358c195235966b05f66b4664e7bf31c3f384a9066b3d1fcc3e96b4c3f65",
     "version": "latest",
     "image_name": "latest-200619100734@gjf4p",
     "last_modified": "2020-06-19T10:07:34+08:00",
     "strategy_config": {
      "concurrency": -1
     },
     "StrategyConfig": {},
     "enterprise_project_id": "0"
    }
    ```


