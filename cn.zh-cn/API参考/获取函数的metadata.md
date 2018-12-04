# 获取函数的metadata<a name="functiongraph_06_0106"></a>

## 功能介绍<a name="section21363070"></a>

获取指定函数的metadata。

## URI<a name="section58049908"></a>

URL：/v1.0/\{project\_id\}/fss/functions/\{function\_urn\}/config

Method：GET

参数说明如[表1](#d0e2233)所示。

**表 1**  参数说明

<a name="d0e2233"></a>
<table><thead align="left"><tr id="row35226659"><th class="cellrowborder" valign="top" width="17.52824717528247%" id="mcps1.2.5.1.1"><p id="p34787141"><a name="p34787141"></a><a name="p34787141"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="12.368763123687629%" id="mcps1.2.5.1.2"><p id="p66295060"><a name="p66295060"></a><a name="p66295060"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="17.52824717528247%" id="mcps1.2.5.1.3"><p id="p1190775"><a name="p1190775"></a><a name="p1190775"></a>必选</p>
</th>
<th class="cellrowborder" valign="top" width="52.57474252574742%" id="mcps1.2.5.1.4"><p id="p29343959"><a name="p29343959"></a><a name="p29343959"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row28050459"><td class="cellrowborder" valign="top" width="17.52824717528247%" headers="mcps1.2.5.1.1 "><p id="p57494700"><a name="p57494700"></a><a name="p57494700"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="12.368763123687629%" headers="mcps1.2.5.1.2 "><p id="p26559089"><a name="p26559089"></a><a name="p26559089"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="17.52824717528247%" headers="mcps1.2.5.1.3 "><p id="p3802578"><a name="p3802578"></a><a name="p3802578"></a>必选</p>
</td>
<td class="cellrowborder" valign="top" width="52.57474252574742%" headers="mcps1.2.5.1.4 "><p id="p39573433"><a name="p39573433"></a><a name="p39573433"></a>Project Id。</p>
</td>
</tr>
<tr id="row20616577"><td class="cellrowborder" valign="top" width="17.52824717528247%" headers="mcps1.2.5.1.1 "><p id="p59330025"><a name="p59330025"></a><a name="p59330025"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="12.368763123687629%" headers="mcps1.2.5.1.2 "><p id="p41002697"><a name="p41002697"></a><a name="p41002697"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="17.52824717528247%" headers="mcps1.2.5.1.3 "><p id="p32884170"><a name="p32884170"></a><a name="p32884170"></a>必选</p>
</td>
<td class="cellrowborder" valign="top" width="52.57474252574742%" headers="mcps1.2.5.1.4 "><p id="p46372115"><a name="p46372115"></a><a name="p46372115"></a>函数的URN，详细解释见<a href="FunctionGraph函数模型.md">FunctionGraph函数模型</a>的描述。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section52687132"></a>

**请求参数**

无

**请求示例**

```
GET /v1.0/7aad83af3e8d42e99ac194e8419e2c9b/fss/functions/urn:fss:cn-north-1:7aad83af3e8d42e99ac194e8419e2c9b:function:default:test:latest/config HTTP/1.1
```

## 响应消息<a name="section4422141"></a>

**响应参数**

函数的metadata信息：JSON对象，表示指定函数的metadata信息。

**响应示例**

成功时的返回格式：

```
HTTP / 1.1 200 OK 
{
	"CodeFileName": "index.js",
	"CodeSize": 272,
	"CodeType": "inline",
	"CodeUrl": "",
	"Cpu": 300,
	"DependencyPkg": "",
	"Description": "111",
	"Digest": "decbce6939297b0b5ec6d1a23bf9c725870f5e69fc338a89a6a4029264688dc26338f56d08b6535de47f15ad538e22ca66613b9a46f807d50b687bb53fded1c6",
	"FuncName": "test",
	"FuncUrn": "urn:fss:cn-north-1:7aad83af3e8d42e99ac194e8419e2c9b:function:default:test:latest",
	"Handler": "test.handler",
	"ImageName": "latest-5qe8e",
	"LastModified": "2018-03-28T11:30:32+08:00",
	"MemorySize": 128,
	"Namespace": "7aad83af3e8d42e99ac194e8419e2c9b",
	"Package": "default",
	"ProjectName": "cn-north-1",
	"Runtime": "Node.js6.10",
	"Timeout": 3,
	"UserData": "",
	"UserDomain": "cff01_hk",
	"Version": "latest",
	"VersionDescription": "",
	"Xrole": "cff"
}
```

```
失败时的返回格式（示例）：
```

```
HTTP / 1.1 404 Not Found
 {
	"error_code": "FSS.1051",
	"error_msg": "Not found the function"
}
```

## 状态码<a name="section39799274"></a>

状态码说明如[表2](#d0e2312)所示。

**表 2**  状态码说明

<a name="d0e2312"></a>
<table><thead align="left"><tr id="row58182238"><th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.3.1.1"><p id="p15140815"><a name="p15140815"></a><a name="p15140815"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="86.87%" id="mcps1.2.3.1.2"><p id="p18446534"><a name="p18446534"></a><a name="p18446534"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row17774248"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p30427999"><a name="p30427999"></a><a name="p30427999"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p48748883"><a name="p48748883"></a><a name="p48748883"></a>InvalidParameterValueException：输入参数错误。</p>
</td>
</tr>
<tr id="row36086767"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p37347016"><a name="p37347016"></a><a name="p37347016"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p5209490"><a name="p5209490"></a><a name="p5209490"></a>UnauthorizedAccess：未授权的访问。</p>
</td>
</tr>
<tr id="row179461988382"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p1694613843812"><a name="p1694613843812"></a><a name="p1694613843812"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p1394612883820"><a name="p1394612883820"></a><a name="p1394612883820"></a>Forbidden：禁止访问。</p>
</td>
</tr>
<tr id="row46885417"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p39622431"><a name="p39622431"></a><a name="p39622431"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p55300313"><a name="p55300313"></a><a name="p55300313"></a>ResourceNotFoundException：函数没有找到。</p>
</td>
</tr>
<tr id="row27940771"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p48609983"><a name="p48609983"></a><a name="p48609983"></a>429</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p45094547"><a name="p45094547"></a><a name="p45094547"></a>TooManyRequestsException：并发请求数太多。</p>
</td>
</tr>
<tr id="row3197746"><td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.3.1.1 "><p id="p57690894"><a name="p57690894"></a><a name="p57690894"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="86.87%" headers="mcps1.2.3.1.2 "><p id="p42450871"><a name="p42450871"></a><a name="p42450871"></a>InternalServerError：服务内部出错。</p>
</td>
</tr>
</tbody>
</table>

