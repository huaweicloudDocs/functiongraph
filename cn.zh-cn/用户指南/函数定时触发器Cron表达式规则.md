# 函数定时触发器Cron表达式规则<a name="ZH-CN_TOPIC_0149027394"></a>

函数Cron表达式下支持如下几种配置方式。

-   @every格式

    @every  _**N**_Unit，其中N表示一个正整数，Unit可以为ns, µs, ms, s, m, h，表示每隔N个Unit时间触发一次函数如[表1](#table7363243105610)所示。

    **表 1**  表达式示例

    <a name="table7363243105610"></a>
    <table><thead align="left"><tr id="row153631343175610"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p114656577565"><a name="p114656577565"></a><a name="p114656577565"></a><strong id="b6465105795612"><a name="b6465105795612"></a><a name="b6465105795612"></a>表达式</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p846535705617"><a name="p846535705617"></a><a name="p846535705617"></a><strong id="b14658573568"><a name="b14658573568"></a><a name="b14658573568"></a>含义</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1636319436563"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p1946555795610"><a name="p1946555795610"></a><a name="p1946555795610"></a>@every 30m</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p204650576563"><a name="p204650576563"></a><a name="p204650576563"></a>每隔30分钟触发一次函数</p>
    </td>
    </tr>
    <tr id="row1136344345610"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p124650571569"><a name="p124650571569"></a><a name="p124650571569"></a>@every 1.5h</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p14651357205618"><a name="p14651357205618"></a><a name="p14651357205618"></a>每隔1.5小时触发一次函数</p>
    </td>
    </tr>
    <tr id="row736344395611"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p34651457195619"><a name="p34651457195619"></a><a name="p34651457195619"></a>@every 2h30m</p>
    </td>
    <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p3465125714565"><a name="p3465125714565"></a><a name="p3465125714565"></a>每隔2小时30分钟触发一次函数</p>
    </td>
    </tr>
    </tbody>
    </table>

-   标准cron表达式

    cron表达式格式要求“秒 分 时 日 月 周\(可选\)”，每个字段间以空格隔开，其中各字段说明如[表2](#table5859105445813)所示。

    **表 2**  cron表达式字段说明

    <a name="table5859105445813"></a>
    <table><thead align="left"><tr id="row108590549589"><th class="cellrowborder" valign="top" width="25.05%" id="mcps1.2.5.1.1"><p id="p46291113595"><a name="p46291113595"></a><a name="p46291113595"></a><strong id="b15627115595"><a name="b15627115595"></a><a name="b15627115595"></a>字段</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="24.95%" id="mcps1.2.5.1.2"><p id="p1962141155919"><a name="p1962141155919"></a><a name="p1962141155919"></a><strong id="b1362211135912"><a name="b1362211135912"></a><a name="b1362211135912"></a>说明</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="p562201185912"><a name="p562201185912"></a><a name="p562201185912"></a><strong id="b1262191113591"><a name="b1262191113591"></a><a name="b1262191113591"></a>取值范围</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="p96217117591"><a name="p96217117591"></a><a name="p96217117591"></a><strong id="b17621311135914"><a name="b17621311135914"></a><a name="b17621311135914"></a>允许的特殊字符</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2859554165811"><td class="cellrowborder" valign="top" width="25.05%" headers="mcps1.2.5.1.1 "><p id="p962811145915"><a name="p962811145915"></a><a name="p962811145915"></a>秒</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.2.5.1.2 "><p id="p136213114591"><a name="p136213114591"></a><a name="p136213114591"></a>必选</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p1762311205910"><a name="p1762311205910"></a><a name="p1762311205910"></a>0-59</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p26215114599"><a name="p26215114599"></a><a name="p26215114599"></a>, - * /</p>
    </td>
    </tr>
    <tr id="row185915413583"><td class="cellrowborder" valign="top" width="25.05%" headers="mcps1.2.5.1.1 "><p id="p196216111592"><a name="p196216111592"></a><a name="p196216111592"></a>分钟</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.2.5.1.2 "><p id="p7626117591"><a name="p7626117591"></a><a name="p7626117591"></a>必选</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p10635116598"><a name="p10635116598"></a><a name="p10635116598"></a>0-59</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p76341113591"><a name="p76341113591"></a><a name="p76341113591"></a>, - * /</p>
    </td>
    </tr>
    <tr id="row1785945405810"><td class="cellrowborder" valign="top" width="25.05%" headers="mcps1.2.5.1.1 "><p id="p863161112592"><a name="p863161112592"></a><a name="p863161112592"></a>时</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.2.5.1.2 "><p id="p96321165915"><a name="p96321165915"></a><a name="p96321165915"></a>必选</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p56381112599"><a name="p56381112599"></a><a name="p56381112599"></a>0-23</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p16321116591"><a name="p16321116591"></a><a name="p16321116591"></a>, - * /</p>
    </td>
    </tr>
    <tr id="row18593548586"><td class="cellrowborder" valign="top" width="25.05%" headers="mcps1.2.5.1.1 "><p id="p1963511185917"><a name="p1963511185917"></a><a name="p1963511185917"></a>日(Day of month)</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.2.5.1.2 "><p id="p263101119598"><a name="p263101119598"></a><a name="p263101119598"></a>必选</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p06351118592"><a name="p06351118592"></a><a name="p06351118592"></a>1-31</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p1063011135911"><a name="p1063011135911"></a><a name="p1063011135911"></a>, - * ? /</p>
    </td>
    </tr>
    <tr id="row1085913547581"><td class="cellrowborder" valign="top" width="25.05%" headers="mcps1.2.5.1.1 "><p id="p563121116599"><a name="p563121116599"></a><a name="p563121116599"></a>月</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.2.5.1.2 "><p id="p663191135910"><a name="p663191135910"></a><a name="p663191135910"></a>必选</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p1063101195917"><a name="p1063101195917"></a><a name="p1063101195917"></a>1-12或者Jan-Dec（英文不区分大小写）如<a href="#table19718122644217">表3</a>所示。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p126331125920"><a name="p126331125920"></a><a name="p126331125920"></a>, - * /</p>
    </td>
    </tr>
    <tr id="row1985955405817"><td class="cellrowborder" valign="top" width="25.05%" headers="mcps1.2.5.1.1 "><p id="p136371155920"><a name="p136371155920"></a><a name="p136371155920"></a>星期几(Day of week)</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.95%" headers="mcps1.2.5.1.2 "><p id="p176381112595"><a name="p176381112595"></a><a name="p176381112595"></a>可选</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p13638119593"><a name="p13638119593"></a><a name="p13638119593"></a>0-6或者Sun-Sat（0表示星期天，英文不区分大小写），如<a href="#table1559918575415">表4</a>所示。</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p16315115595"><a name="p16315115595"></a><a name="p16315115595"></a>, - * ? /</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 3**  月份字段取值说明

    <a name="table19718122644217"></a>
    <table><thead align="left"><tr id="row14718826114210"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p57181926104211"><a name="p57181926104211"></a><a name="p57181926104211"></a>月份</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p071802664215"><a name="p071802664215"></a><a name="p071802664215"></a>数字</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p67181026124216"><a name="p67181026124216"></a><a name="p67181026124216"></a>英文简写</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row18718112684217"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p18718182618424"><a name="p18718182618424"></a><a name="p18718182618424"></a>1月</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p1371822694216"><a name="p1371822694216"></a><a name="p1371822694216"></a>1</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p5718162613423"><a name="p5718162613423"></a><a name="p5718162613423"></a>Jan</p>
    </td>
    </tr>
    <tr id="row1871802644213"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p37181426124211"><a name="p37181426124211"></a><a name="p37181426124211"></a>2月</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p2071816265426"><a name="p2071816265426"></a><a name="p2071816265426"></a>2</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p127188269429"><a name="p127188269429"></a><a name="p127188269429"></a>Feb</p>
    </td>
    </tr>
    <tr id="row07181226134214"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p1471812611426"><a name="p1471812611426"></a><a name="p1471812611426"></a>3月</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p19718426164213"><a name="p19718426164213"></a><a name="p19718426164213"></a>3</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p471852618426"><a name="p471852618426"></a><a name="p471852618426"></a>Mar</p>
    </td>
    </tr>
    <tr id="row57181326154214"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p8718112664216"><a name="p8718112664216"></a><a name="p8718112664216"></a>4月</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p47181026124213"><a name="p47181026124213"></a><a name="p47181026124213"></a>4</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p197180265429"><a name="p197180265429"></a><a name="p197180265429"></a>Apr</p>
    </td>
    </tr>
    <tr id="row18718152615425"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p18718202684215"><a name="p18718202684215"></a><a name="p18718202684215"></a>5月</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p1718132612425"><a name="p1718132612425"></a><a name="p1718132612425"></a>5</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p3718126124220"><a name="p3718126124220"></a><a name="p3718126124220"></a>May</p>
    </td>
    </tr>
    <tr id="row18718202619425"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p17187267427"><a name="p17187267427"></a><a name="p17187267427"></a>6月</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p11719192615423"><a name="p11719192615423"></a><a name="p11719192615423"></a>6</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p14719026174217"><a name="p14719026174217"></a><a name="p14719026174217"></a>Jun</p>
    </td>
    </tr>
    <tr id="row671942611423"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p87192262429"><a name="p87192262429"></a><a name="p87192262429"></a>7月</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p137191126184217"><a name="p137191126184217"></a><a name="p137191126184217"></a>7</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p1471915261421"><a name="p1471915261421"></a><a name="p1471915261421"></a>Jul</p>
    </td>
    </tr>
    <tr id="row87199267425"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p4719172619428"><a name="p4719172619428"></a><a name="p4719172619428"></a>8月</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p971902613426"><a name="p971902613426"></a><a name="p971902613426"></a>8</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p1771942694216"><a name="p1771942694216"></a><a name="p1771942694216"></a>Aug</p>
    </td>
    </tr>
    <tr id="row7719142684216"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p197191226114216"><a name="p197191226114216"></a><a name="p197191226114216"></a>9月</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p6719132664210"><a name="p6719132664210"></a><a name="p6719132664210"></a>9</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p9719182613426"><a name="p9719182613426"></a><a name="p9719182613426"></a>Sep</p>
    </td>
    </tr>
    <tr id="row97191626204218"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p971972613425"><a name="p971972613425"></a><a name="p971972613425"></a>10月</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p147191026194214"><a name="p147191026194214"></a><a name="p147191026194214"></a>10</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p1719122612425"><a name="p1719122612425"></a><a name="p1719122612425"></a>Oct</p>
    </td>
    </tr>
    <tr id="row19719102674219"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p9719226184213"><a name="p9719226184213"></a><a name="p9719226184213"></a>11月</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p67191826164215"><a name="p67191826164215"></a><a name="p67191826164215"></a>11</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p10719132610426"><a name="p10719132610426"></a><a name="p10719132610426"></a>Nov</p>
    </td>
    </tr>
    <tr id="row7719182620425"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p87195264423"><a name="p87195264423"></a><a name="p87195264423"></a>12月</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p1671952618426"><a name="p1671952618426"></a><a name="p1671952618426"></a>12</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p207191326154216"><a name="p207191326154216"></a><a name="p207191326154216"></a>Dec</p>
    </td>
    </tr>
    </tbody>
    </table>

    **表 4**  星期字段取值说明

    <a name="table1559918575415"></a>
    <table><thead align="left"><tr id="row196077555412"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p8610659542"><a name="p8610659542"></a><a name="p8610659542"></a>星期</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p661115205413"><a name="p661115205413"></a><a name="p661115205413"></a>数字</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p361411525417"><a name="p361411525417"></a><a name="p361411525417"></a>英文简写</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row9615145165413"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p7618135155411"><a name="p7618135155411"></a><a name="p7618135155411"></a>星期一</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p46201575412"><a name="p46201575412"></a><a name="p46201575412"></a>1</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p16212535415"><a name="p16212535415"></a><a name="p16212535415"></a>Mon</p>
    </td>
    </tr>
    <tr id="row562117545420"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p1562318516545"><a name="p1562318516545"></a><a name="p1562318516545"></a>星期二</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p1162516510546"><a name="p1162516510546"></a><a name="p1162516510546"></a>2</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p116261505411"><a name="p116261505411"></a><a name="p116261505411"></a>Tue</p>
    </td>
    </tr>
    <tr id="row36265519547"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p46281051542"><a name="p46281051542"></a><a name="p46281051542"></a>星期三</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p116301555419"><a name="p116301555419"></a><a name="p116301555419"></a>3</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p1763175145410"><a name="p1763175145410"></a><a name="p1763175145410"></a>Wed</p>
    </td>
    </tr>
    <tr id="row10633185135411"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p1563413555411"><a name="p1563413555411"></a><a name="p1563413555411"></a>星期四</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p263515115414"><a name="p263515115414"></a><a name="p263515115414"></a>4</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p063745105414"><a name="p063745105414"></a><a name="p063745105414"></a>Thu</p>
    </td>
    </tr>
    <tr id="row2637175105413"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p36404515412"><a name="p36404515412"></a><a name="p36404515412"></a>星期五</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p76401157541"><a name="p76401157541"></a><a name="p76401157541"></a>5</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p964210510546"><a name="p964210510546"></a><a name="p964210510546"></a>Fri</p>
    </td>
    </tr>
    <tr id="row15642958549"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p8644556542"><a name="p8644556542"></a><a name="p8644556542"></a>星期六</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p16460511546"><a name="p16460511546"></a><a name="p16460511546"></a>6</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p106481855548"><a name="p106481855548"></a><a name="p106481855548"></a>Sat</p>
    </td>
    </tr>
    <tr id="row565095165410"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p0652135205412"><a name="p0652135205412"></a><a name="p0652135205412"></a>星期日</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p2654175205413"><a name="p2654175205413"></a><a name="p2654175205413"></a>0</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p7656145175410"><a name="p7656145175410"></a><a name="p7656145175410"></a>Sun</p>
    </td>
    </tr>
    </tbody>
    </table>

    cron表达式字段特殊字符说明如[表5](#table161351329175920)所示。

    **表 5**  特殊字符说明

    <a name="table161351329175920"></a>
    <table><thead align="left"><tr id="row101351229105918"><th class="cellrowborder" valign="top" width="15.201520152015203%" id="mcps1.2.4.1.1"><p id="p1302479599"><a name="p1302479599"></a><a name="p1302479599"></a><strong id="b40154716595"><a name="b40154716595"></a><a name="b40154716595"></a>特殊字符</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="28.012801280128013%" id="mcps1.2.4.1.2"><p id="p6004710595"><a name="p6004710595"></a><a name="p6004710595"></a><strong id="b50144775919"><a name="b50144775919"></a><a name="b50144775919"></a>含义</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="56.78567856785678%" id="mcps1.2.4.1.3"><p id="p140154720597"><a name="p140154720597"></a><a name="p140154720597"></a><strong id="b120154710591"><a name="b120154710591"></a><a name="b120154710591"></a>说明</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row141351829195912"><td class="cellrowborder" valign="top" width="15.201520152015203%" headers="mcps1.2.4.1.1 "><p id="p1502477598"><a name="p1502477598"></a><a name="p1502477598"></a>*</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.2.4.1.2 "><p id="p15014476592"><a name="p15014476592"></a><a name="p15014476592"></a>表示该字段中的所有值</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.78567856785678%" headers="mcps1.2.4.1.3 "><p id="p1501247155917"><a name="p1501247155917"></a><a name="p1501247155917"></a>在“分钟”字段中表示每一分钟都执行。</p>
    </td>
    </tr>
    <tr id="row19135429125913"><td class="cellrowborder" valign="top" width="15.201520152015203%" headers="mcps1.2.4.1.1 "><p id="p18024745915"><a name="p18024745915"></a><a name="p18024745915"></a>,</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.2.4.1.2 "><p id="p110154717595"><a name="p110154717595"></a><a name="p110154717595"></a>指定多个值（可以不连续）</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.78567856785678%" headers="mcps1.2.4.1.3 "><p id="p150134716595"><a name="p150134716595"></a><a name="p150134716595"></a>在“月”字段中指定“Jan,Apr,Jul,Oct”或者“1,4,7,10”，表示1月，4月，7月和10月，在“星期几”字段中指定“Sat,Sun”或者“6,0”表示周六，周日。</p>
    </td>
    </tr>
    <tr id="row161351029205914"><td class="cellrowborder" valign="top" width="15.201520152015203%" headers="mcps1.2.4.1.1 "><p id="p601147205911"><a name="p601147205911"></a><a name="p601147205911"></a>-</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.2.4.1.2 "><p id="p18054719591"><a name="p18054719591"></a><a name="p18054719591"></a>指定一个范围</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.78567856785678%" headers="mcps1.2.4.1.3 "><p id="p140447145917"><a name="p140447145917"></a><a name="p140447145917"></a>在“分钟”字段中使用0-3，表示从0分到3分</p>
    </td>
    </tr>
    <tr id="row12135152955914"><td class="cellrowborder" valign="top" width="15.201520152015203%" headers="mcps1.2.4.1.1 "><p id="p1921747175912"><a name="p1921747175912"></a><a name="p1921747175912"></a>?</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.2.4.1.2 "><p id="p329479599"><a name="p329479599"></a><a name="p329479599"></a>指定一个或另一个</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.78567856785678%" headers="mcps1.2.4.1.3 "><p id="p192847205920"><a name="p192847205920"></a><a name="p192847205920"></a>仅“日”和“星期几”字段可以指定。例如，如果指定了一个特定的日期，但你不关心该日期对应星期几，那么“星期几”字段就可以使用该特殊字符。</p>
    </td>
    </tr>
    <tr id="row113592913591"><td class="cellrowborder" valign="top" width="15.201520152015203%" headers="mcps1.2.4.1.1 "><p id="p62647115920"><a name="p62647115920"></a><a name="p62647115920"></a>/</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.012801280128013%" headers="mcps1.2.4.1.2 "><p id="p921047145915"><a name="p921047145915"></a><a name="p921047145915"></a>表示起步和步幅，n/m表示从n开始，每次增加m</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.78567856785678%" headers="mcps1.2.4.1.3 "><p id="p19294713598"><a name="p19294713598"></a><a name="p19294713598"></a>在“分钟”字段1/3表示在满足其它字段情况下的绝对时间1分（例如00:01:00）开始，每隔3分钟触发一次。</p>
    </td>
    </tr>
    </tbody>
    </table>

    cron表达式配置示例如[表6](#table20546153220011)所示。

    **表 6**  cron表达式配置示例

    <a name="table20546153220011"></a>
    <table><thead align="left"><tr id="row115474321503"><th class="cellrowborder" valign="top" width="42.24%" id="mcps1.2.3.1.1"><p id="p454716329015"><a name="p454716329015"></a><a name="p454716329015"></a>配置示例</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.76%" id="mcps1.2.3.1.2"><p id="p154703218019"><a name="p154703218019"></a><a name="p154703218019"></a>示例说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row145471329013"><td class="cellrowborder" valign="top" width="42.24%" headers="mcps1.2.3.1.1 "><p id="p9117113513019"><a name="p9117113513019"></a><a name="p9117113513019"></a>0 15 2 * * ?</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.76%" headers="mcps1.2.3.1.2 "><p id="p161170357019"><a name="p161170357019"></a><a name="p161170357019"></a>每天凌晨02:15:00执行</p>
    </td>
    </tr>
    <tr id="row754710321802"><td class="cellrowborder" valign="top" width="42.24%" headers="mcps1.2.3.1.1 "><p id="p1711713352017"><a name="p1711713352017"></a><a name="p1711713352017"></a>0 30 8 ? * Mon-Fri</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.76%" headers="mcps1.2.3.1.2 "><p id="p1211793517013"><a name="p1211793517013"></a><a name="p1211793517013"></a>周一到周五上午08:30:00执行</p>
    </td>
    </tr>
    <tr id="row45473326018"><td class="cellrowborder" valign="top" width="42.24%" headers="mcps1.2.3.1.1 "><p id="p1611714357012"><a name="p1611714357012"></a><a name="p1611714357012"></a>0 45 7 1-3 * ?</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.76%" headers="mcps1.2.3.1.2 "><p id="p711718351010"><a name="p711718351010"></a><a name="p711718351010"></a>每月1, 2, 3号上午07:45:00执行</p>
    </td>
    </tr>
    <tr id="row2054712321205"><td class="cellrowborder" valign="top" width="42.24%" headers="mcps1.2.3.1.1 "><p id="p111171635907"><a name="p111171635907"></a><a name="p111171635907"></a>0 0/3 * ? * Mon,Wed,Fri,Sun</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.76%" headers="mcps1.2.3.1.2 "><p id="p4117163518015"><a name="p4117163518015"></a><a name="p4117163518015"></a>周一、三、五、日，每隔三分钟执行一次</p>
    </td>
    </tr>
    <tr id="row9547153215010"><td class="cellrowborder" valign="top" width="42.24%" headers="mcps1.2.3.1.1 "><p id="p121171835305"><a name="p121171835305"></a><a name="p121171835305"></a>0 0/3 9-18 ? * Mon-Fri</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.76%" headers="mcps1.2.3.1.2 "><p id="p51175351409"><a name="p51175351409"></a><a name="p51175351409"></a>周一到周五09:00-18:00之间每隔三分钟执行一次</p>
    </td>
    </tr>
    <tr id="row14547632502"><td class="cellrowborder" valign="top" width="42.24%" headers="mcps1.2.3.1.1 "><p id="p111178351012"><a name="p111178351012"></a><a name="p111178351012"></a>0 0/30 * * * ?</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.76%" headers="mcps1.2.3.1.2 "><p id="p3117535606"><a name="p3117535606"></a><a name="p3117535606"></a>每30分钟执行一次</p>
    </td>
    </tr>
    </tbody>
    </table>


