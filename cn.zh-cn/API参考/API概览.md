# API概览<a name="ZH-CN_TOPIC_0115410420"></a>

FunctionGraph API为开发者、合作伙伴提供开发、部署、托管、运维的开放接口，帮助用户快速、低成本地实现业务创新，缩短应用上线周期。

FunctionGraph API提供的接口有如下几种类型。

**表 1**  接口简介

<a name="table0959420112419"></a>
<table><thead align="left"><tr id="row5959142013241"><th class="cellrowborder" valign="top" width="27%" id="mcps1.2.3.1.1"><p id="p229153662411"><a name="p229153662411"></a><a name="p229153662411"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="73%" id="mcps1.2.3.1.2"><p id="p169592203248"><a name="p169592203248"></a><a name="p169592203248"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row19959820182413"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.3.1.1 "><p id="p1092243442517"><a name="p1092243442517"></a><a name="p1092243442517"></a><a href="#section164721755112711">函数管理域接口</a></p>
</td>
<td class="cellrowborder" valign="top" width="73%" headers="mcps1.2.3.1.2 "><p id="p59223340254"><a name="p59223340254"></a><a name="p59223340254"></a>函数的管理域接口，包括函数获取、创建、修改、发布等。</p>
</td>
</tr>
<tr id="row1695916208243"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.3.1.1 "><p id="p1258153117257"><a name="p1258153117257"></a><a name="p1258153117257"></a><a href="#section16307174753514">函数数据域接口</a></p>
</td>
<td class="cellrowborder" valign="top" width="73%" headers="mcps1.2.3.1.2 "><p id="p1658133192514"><a name="p1658133192514"></a><a name="p1658133192514"></a>函数的数据域接口，包括同步执行函数和异步执行函数。</p>
</td>
</tr>
</tbody>
</table>

## 函数管理域接口<a name="section164721755112711"></a>

**表 2**  管理域接口

<a name="table11301194162420"></a>
<table><thead align="left"><tr id="row1730213432419"><th class="cellrowborder" valign="top" width="26%" id="mcps1.2.3.1.1"><p id="p9302194162419"><a name="p9302194162419"></a><a name="p9302194162419"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="74%" id="mcps1.2.3.1.2"><p id="p1530213422415"><a name="p1530213422415"></a><a name="p1530213422415"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1830264142413"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p430284122410"><a name="p430284122410"></a><a name="p430284122410"></a><a href="获取函数列表.md">获取函数列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p33020412240"><a name="p33020412240"></a><a name="p33020412240"></a>获取函数列表。</p>
</td>
</tr>
<tr id="row430211410244"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p123027414247"><a name="p123027414247"></a><a name="p123027414247"></a><a href="获取函数的metadata.md">获取函数的metadata</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p16302174152416"><a name="p16302174152416"></a><a name="p16302174152416"></a>获取指定函数的metadata。</p>
</td>
</tr>
<tr id="row156934462511"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p55691644172517"><a name="p55691644172517"></a><a name="p55691644172517"></a><a href="获取指定函数代码.md">获取指定函数代码</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p35106503"><a name="p35106503"></a><a name="p35106503"></a>获取指定函数的代码。</p>
</td>
</tr>
<tr id="row5743118172610"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p37439186261"><a name="p37439186261"></a><a name="p37439186261"></a><a href="创建函数.md">创建函数</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p1743121816263"><a name="p1743121816263"></a><a name="p1743121816263"></a>创建指定的函数。</p>
</td>
</tr>
<tr id="row341512810264"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p3415178152619"><a name="p3415178152619"></a><a name="p3415178152619"></a><a href="删除函数-版本.md">删除函数/版本</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p124151887263"><a name="p124151887263"></a><a name="p124151887263"></a>删除指定的函数或者特定的版本（不允许删除latest版本）。</p>
</td>
</tr>
<tr id="row14680111310266"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p116801313102617"><a name="p116801313102617"></a><a name="p116801313102617"></a><a href="修改函数代码.md">修改函数代码</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p15680131372614"><a name="p15680131372614"></a><a name="p15680131372614"></a>修改指定的函数的代码。</p>
</td>
</tr>
<tr id="row09916497250"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p1199124992513"><a name="p1199124992513"></a><a name="p1199124992513"></a><a href="修改函数的metadata信息.md">修改函数的metadata信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p1099154942513"><a name="p1099154942513"></a><a name="p1099154942513"></a>修改指定的函数的metadata信息。</p>
</td>
</tr>
<tr id="row2098311531252"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p7983195312254"><a name="p7983195312254"></a><a name="p7983195312254"></a><a href="发布函数版本.md">发布函数版本</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p2983175332515"><a name="p2983175332515"></a><a name="p2983175332515"></a>发布函数版本。</p>
</td>
</tr>
<tr id="row1647412362610"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p104741236263"><a name="p104741236263"></a><a name="p104741236263"></a><a href="获取指定函数的版本列表.md">获取指定函数的版本列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p84747316265"><a name="p84747316265"></a><a name="p84747316265"></a>获取指定函数的版本列表。</p>
</td>
</tr>
<tr id="row18824458132519"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p2824358142518"><a name="p2824358142518"></a><a name="p2824358142518"></a><a href="创建函数版本别名.md">创建函数版本别名</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p1882413580254"><a name="p1882413580254"></a><a name="p1882413580254"></a>创建函数版本别名。</p>
</td>
</tr>
<tr id="row417314402259"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p7173154013253"><a name="p7173154013253"></a><a name="p7173154013253"></a><a href="修改函数版本别名信息.md">修改函数版本别名信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p5173184072517"><a name="p5173184072517"></a><a name="p5173184072517"></a>修改函数版本别名信息。</p>
</td>
</tr>
<tr id="row145012366254"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p35023612511"><a name="p35023612511"></a><a name="p35023612511"></a><a href="删除函数版本别名.md">删除函数版本别名</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p9506362251"><a name="p9506362251"></a><a name="p9506362251"></a>删除函数版本别名。</p>
</td>
</tr>
<tr id="row193028414248"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p103021419242"><a name="p103021419242"></a><a name="p103021419242"></a><a href="获取函数版本的指定别名信息.md">获取函数版本的指定别名信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p17302144142411"><a name="p17302144142411"></a><a name="p17302144142411"></a>获取函数指定的版本别名信息。</p>
</td>
</tr>
<tr id="row14302124182418"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p130213415245"><a name="p130213415245"></a><a name="p130213415245"></a><a href="获取指定函数所有版本别名列表.md">获取指定函数所有版本别名列表</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p1730211422414"><a name="p1730211422414"></a><a name="p1730211422414"></a>获取函数版本别名列表。</p>
</td>
</tr>
<tr id="row230214472420"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p830214442420"><a name="p830214442420"></a><a name="p830214442420"></a><a href="获取指定函数的所有触发器.md">获取指定函数的所有触发器</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p193021144245"><a name="p193021144245"></a><a name="p193021144245"></a>获取指定函数的所有触发器设置。</p>
</td>
</tr>
<tr id="row1730264132416"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p430294192415"><a name="p430294192415"></a><a name="p430294192415"></a><a href="获取指定触发器的信息.md">获取指定触发器的信息</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p53021246244"><a name="p53021246244"></a><a name="p53021246244"></a>获取特定触发器的信息。</p>
</td>
</tr>
<tr id="row330219419248"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p230284152415"><a name="p230284152415"></a><a name="p230284152415"></a><a href="删除指定函数的所有触发器.md">删除指定函数的所有触发器</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p1830216420249"><a name="p1830216420249"></a><a name="p1830216420249"></a>删除指定函数所有触发器设置。</p>
</td>
</tr>
<tr id="row1447516571333"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p10475357123315"><a name="p10475357123315"></a><a name="p10475357123315"></a><a href="创建触发器.md">创建触发器</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p8475125715339"><a name="p8475125715339"></a><a name="p8475125715339"></a>创建触发器。</p>
</td>
</tr>
<tr id="row107385293411"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.3.1.1 "><p id="p973811212348"><a name="p973811212348"></a><a name="p973811212348"></a><a href="删除触发器.md">删除触发器</a></p>
</td>
<td class="cellrowborder" valign="top" width="74%" headers="mcps1.2.3.1.2 "><p id="p13738122113415"><a name="p13738122113415"></a><a name="p13738122113415"></a>删除触发器。</p>
</td>
</tr>
</tbody>
</table>

## 函数数据域接口<a name="section16307174753514"></a>

**表 3**  数据域接口

<a name="table0701312373"></a>
<table><thead align="left"><tr id="row147019111375"><th class="cellrowborder" valign="top" width="27%" id="mcps1.2.3.1.1"><p id="p1370121183718"><a name="p1370121183718"></a><a name="p1370121183718"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="73%" id="mcps1.2.3.1.2"><p id="p1570614372"><a name="p1570614372"></a><a name="p1570614372"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row370171153715"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.3.1.1 "><p id="p12705115372"><a name="p12705115372"></a><a name="p12705115372"></a><a href="同步执行函数.md">同步执行函数</a></p>
</td>
<td class="cellrowborder" valign="top" width="73%" headers="mcps1.2.3.1.2 "><p id="p107014123710"><a name="p107014123710"></a><a name="p107014123710"></a>同步执行函数。</p>
</td>
</tr>
<tr id="row570161133712"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.2.3.1.1 "><p id="p67010113711"><a name="p67010113711"></a><a name="p67010113711"></a><a href="异步执行函数.md">异步执行函数</a></p>
</td>
<td class="cellrowborder" valign="top" width="73%" headers="mcps1.2.3.1.2 "><p id="p37010113373"><a name="p37010113373"></a><a name="p37010113373"></a>异步执行函数。</p>
</td>
</tr>
</tbody>
</table>

