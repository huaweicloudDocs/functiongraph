# 示例1：创建函数和Timer触发器实现定时从OBS桶中下载文件<a name="ZH-CN_TOPIC_0251707988"></a>

## 场景描述<a name="section11773144817815"></a>

本章节以Python 2.7为例，指导您通过API创建FunctionGraph函数和Timer触发器，实现定时从OBS桶中下载文件。

API的调用方法请参见[如何调用API](如何调用API.md)。

## 前提条件<a name="section1835181812285"></a>

-   已在OBS服务中上传文件，并记录文件名、文件所在的OBS桶名，以及OBS地址的链接。
-   已配置具有OBS服务访问权限的委托，并记录委托名。

## 总体思路<a name="section780392783814"></a>

创建FunctionGraph函数和Timer触发器，实现定时从OBS桶中下载文件，步骤如下：

1.  [创建函数](创建函数.md)：创建下载文件的函数。
2.  [修改函数的metadata信息](修改函数的metadata信息.md)：修改函数配置信息中的OBS地址、OBS桶名和文件名。
3.  [同步执行函数](同步执行函数.md)：确认函数能够成功从OBS桶中下载文件。
4.  [创建触发器](创建触发器.md)：创建Timer触发器，实现定时下载文件。

## 步骤1：创建下载文件的函数<a name="section14318132594418"></a>

URI：POST /v2/\{project\_id\}/fgs/functions

API文档详情请参见：[创建函数](创建函数.md)

-   请求示例

    ```
    POST  https://{Endpoint}/v2/{project_id}/fgs/functions
    {
     "code_filename": "index.zip",
     "code_type": "inline",
     "func_code": {
      "file": "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"
     },
     "func_name": "download_file_from_obs",
     "handler": "index.handler",
     "memory_size": 256,
     "package": "default",
     "runtime": "Python2.7",
     "timeout": 30
    }
    ```

-   响应示例

    ```
    {
     "func_urn": "urn:fss:{project_name}:{project_id}:function:default:download_file_from_obs:latest",
     "func_name": "download_file_from_obs",
     "domain_id": "89fexxxd636",
     "namespace": "{project_id}",
     "project_name": "xxx",
     "package": "default",
     "runtime": "Python2.7",
     "timeout": 30,
     "handler": "index.handler",
     "memory_size": 256,
     "cpu": 400,
     "code_type": "inline",
     "code_filename": "index.zip",
     "code_size": 1707,
     "digest": "68891a6778848a78bd37a8c0798c91d75a5c87aee6e901303047a52edf05bf2170aac4149d79b3f6a40efe78406a83bf6d8683e7b25da4f0c07e7493aa4ccdcd",
     "version": "latest",
     "image_name": "latest-200603162219@zr2ym",
     "last_modified": "2020-06-03T16:22:19+08:00",
     "strategy_config": {
      "concurrency": -1
     },
     "StrategyConfig": {},
     "enterprise_project_id": "0"
    }
    ```

    记录函数的URN，即响应示例中的“func\_urn”信息。


## 步骤2：修改函数配置信息中的OBS地址、OBS桶名和文件名<a name="section399354318306"></a>

URI：PUT /v2/\{project\_id\}/fgs/functions/\{function\_urn\}/config

API文档详情请参见：[修改函数的metadata信息](修改函数的metadata信息.md)

-   请求示例

    ```
    PUT  https://{Endpoint}/v2/{project_id}/fgs/functions/{function_urn}/config
    {
     "func_name": "download_file_from_obs",
     "handler": "index.handler",
     "memory_size": 256,
     "runtime": "Python2.7",
     "timeout": 30,
     "user_data": "{\"obs_address\":\" obs.xxx.xxx.com\",\"srcBucket\":\" xxx\",\"srcObjName\":\"xxx\"}",
     "xrole": "xxx"
    }
    ```

    function\_urn为[步骤1：创建下载文件的函数](#section14318132594418)中记录的函数URN，obs\_address为OBS地址，srcBucket为OBS桶名，srcObjName为文件名，xrole为委托名。

-   响应示例

    ```
    {
     "func_urn": "urn:fss:{project_name}:{project_id}:function:default:download_file_from_obs:latest",
     "func_name": "download_file_from_obs",
     "domain_id": "89fexxxd636",
     "namespace": "{project_id}",
     "project_name": "xxx",
     "package": "default",
     "runtime": "Python2.7",
     "timeout": 30,
     "handler": "index.handler",
     "memory_size": 256,
     "cpu": 400,
     "code_type": "inline",
     "code_filename": "index.zip",
     "code_size": 1707,
     "user_data": "{\"obs_address\":\"obs.xxx.xxx.com\",\"srcBucket\":\"xxx\",\"srcObjName\":\"xxx\"}",
     "digest": "68891a6778848a78bd37a8c0798c91d75a5c87aee6e901303047a52edf05bf2170aac4149d79b3f6a40efe78406a83bf6d8683e7b25da4f0c07e7493aa4ccdcd",
     "version": "latest",
     "image_name": "latest-200603165355@varrp",
     "xrole": "xxx",
     "app_xrole": "xxx",
     "last_modified": "2020-06-03T17:25:03+08:00",
     "strategy_config": {
      "concurrency": -1
     },
     "StrategyConfig": {},
     "enterprise_project_id": "0"
    }
    ```


## 步骤3：确认函数能够成功从OBS桶中下载文件<a name="section16598919223"></a>

URI：POST /v2/\{project\_id\}/fgs/functions/\{function\_urn\}/invocations

API文档详情请参见：[同步执行函数](同步执行函数.md)

-   请求示例

    ```
    POST  https://{Endpoint}/v2/{project_id}/fgs/functions/{function_urn}/invocations
    {
     "message": "download file"
    }
    ```

    function\_urn为[步骤1：创建下载文件的函数](#section14318132594418)中记录的函数URN。

-   响应示例

    ```
    "The object downloaded successfully from OBS, and the size is 14 KB"
    ```


## 步骤4：创建Timer触发器，实现定时下载文件<a name="section1644694317390"></a>

URI：POST /v2/\{project\_id\}/fgs/triggers/\{function\_urn\}

API文档详情请参见：[创建触发器](创建触发器.md)

-   请求示例

    ```
    POST  https://{Endpoint}/v2/{project_id}/fgs/triggers/{function_urn}
    {
     "event_data": {
      "name": "Timer-download",
      "schedule_type": "Rate",
      "schedule": "1d"
     },
     "event_type_code": "MessageCreated",
     "trigger_status": "ACTIVE",
     "trigger_type_code": "TIMER"
    }
    ```

    function\_urn为[步骤1：创建下载文件的函数](#section14318132594418)中记录的函数URN。

    上述请求示例表示每天从OBS桶中下载文件。

-   响应示例

    ```
    {
     "trigger_id": "461bbe95-c85b-4dc9-a306-9701e77f1d66",
     "trigger_type_code": "TIMER",
     "trigger_status": "ACTIVE",
     "event_data": {
      "name": "Timer-download",
      "schedule": "1d",
      "schedule_type": "Rate"
     },
     "last_updated_time": "2020-06-04T10:33:30+08:00",
     "created_time": "2020-06-04T10:33:30+08:00"
    }
    ```


