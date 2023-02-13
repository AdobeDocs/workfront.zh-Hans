---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion中的日期和时间函数
description: 以下日期和时间函数在Adobe Workfront Fusion映射面板中可用。
author: Becky
feature: Workfront Fusion
exl-id: 76c63afc-4bb6-4895-9bba-6b3913ecbcf6
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '1867'
ht-degree: 1%

---

# 中的日期和时间函数 [!DNL Adobe Workfront Fusion]

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL formatDate(日期；格式； [时区])]

当您具有日期值(例如 `12-10-2021 20:30`，以将其格式设置为文本值，例如 `Dec 10, 2021 8:30 PM`.

例如，当您需要在同一情景中将一个应用程序或Web服务的日期格式更改为连接的应用程序或Web服务的日期格式时，这非常有用。

有关更多信息，请参阅 [日期](../../workfront-fusion/mapping/item-data-types.md#date) 和 [文本](../../workfront-fusion/mapping/item-data-types.md#text) 在文章中 [Adobe Workfront Fusion中的项目数据类型](../../workfront-fusion/mapping/item-data-types.md).

### 参数

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>参数</th> 
   <th>预期数据类型* </th> 
   <th>它的作用</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL日期] </td> 
   <td>日期 </td> 
   <td> <p>将日期值转换为文本值。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL格式] </td> 
   <td>文本 </td> 
   <td> <p>允许您使用日期/时间格式令牌指定格式。 有关更多信息，请参阅 <a href="../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md" class="MCXref xref">中用于日期和时间格式的令牌 [!DNL Adobe Workfront Fusion]</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>DD.MM.YYYY HH:mm</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL时区] </td> 
   <td>文本 </td> 
   <td> <p>（可选）用于指定用于转化的时区。 </p> <p>有关已识别时区的列表，请参阅Wikipedia中的“TZ数据库名称”列 <a href="https://en.wikipedia.org/wiki/List_of_tz_database_time_zones">tz数据库时区列表</a>. 只有此列中列出的值会被函数识别为有效时区。 任何其他值都将被忽略，并将改用配置文件中指定的方案时区。 有关更多信息，请参阅文章中的 <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">更改 [!DNL Adobe Workfront Fusion]</a>.</p> <p>如果忽略此参数，则会应用“配置文件”设置中指定的方案时区。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>Europe/Prague</code>, <code>UTC</code></p> </td> 
  </tr> 
 </tbody> 
</table>

如果提供不同类型，则应用类型强制。 有关更多信息，请参阅 [在中键入强制 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

### 返回值和类型

的 `formatDate` 函数会根据指定的格式和时区返回给定日期值的文本表示形式。 数据类型为文本。

>[!INFO]
>
>**示例：** 方案和Web时区均设置为 `Europe/Prague` 在这些示例中。
>
>![](assets/date&time-functions-examples-350x61.png)
>
>* `formatDate(1. Date created;MM/DD/YYYY)`
   >
   >    返回10/01/2018
>
>* `formatDate(1. Date created; YYYY-MM-DD hh:mm A)`
   >
   >   返回2018-10-01 09:32 AM
>
>* `formatDate(1. Date created;DD.MM.YYYY HH:mm;UTC)`
   >
   >    返回01.10.2018 07:32
>
>* `formatDate(now;DD.MM.YYYY HH:mm)`
   >
   >    返回19.03.2019 15:30


## [!UICONTROL parseDate(text;格式； [时区])]

当您具有表示日期的文本值(例如 `12-10-2019 20:30` 或 `Aug 18, 2019 10:00 AM`)并将其转换为日期值（二进制机器可读的表示形式）。 有关更多信息，请参阅 [日期](../../workfront-fusion/mapping/item-data-types.md#date) 和 [文本](../../workfront-fusion/mapping/item-data-types.md#text) 在文章中 [中的项目数据类型 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

### 参数

第二列表示预期的类型。 如果提供不同类型，则应用类型强制。 有关更多信息，请参阅 [在中键入强制 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>参数</th> 
   <th>预期数据类型* </th> 
   <th>它的作用</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL text] </td> 
   <td>文本 </td> 
   <td> <p>将日期值转换为文本值。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL格式] </td> 
   <td>文本 </td> 
   <td> <p>允许您使用日期/时间格式令牌指定格式。 有关更多信息，请参阅 <a href="../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md" class="MCXref xref">Adobe Workfront Fusion中日期和时间格式的令牌</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>DD.MM.YYYY HH:mm</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL时区] </td> 
   <td>文本 </td> 
   <td> <p>（可选）用于指定用于转化的时区。 </p> <p>有关已识别时区的列表，请参阅Wikipedia中的“TZ数据库名称”列 <a href="https://en.wikipedia.org/wiki/List_of_tz_database_time_zones">tz数据库时区列表</a>. 只有此列中列出的值会被函数识别为有效时区。 任何其他值都将被忽略，并将改用配置文件中指定的方案时区。 有关更多信息，请参阅文章中的 <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">在Adobe Workfront Fusion中更改配置文件设置</a>.</p> <p>如果忽略此参数，则会应用“配置文件”设置中指定的方案时区。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>Europe/Prague</code>, <code>UTC</code></p> </td> 
  </tr> 
 </tbody> 
</table>

如果提供不同类型，则应用类型强制。 有关更多信息，请参阅 [在中键入强制 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

### 返回值和类型

此函数会根据您指定的格式和时区，将文本字符串转换为日期。 该值的数据类型为Date。

>[!INFO]
>
>**示例：** 在以下示例中，返回的日期值根据ISO 8601表示，但结果的数据类型是日期。
>
>* `parseDate(2016-12-28;YYYY-MM-DD)`
   >
   >    返回2016-12-28T00:00:00.000Z
>
>* `parseDate(2016-12-28 16:03;YYYY-MM-DD HH:mm)`
   >
   >    返回2016-12-28T16:03:00.000Z
>
>* `parseDate(2016-12-28 04:03 pm; YYYY-MM-DD hh:mm a)`
   >
   >    返回2016-12-28T16:03:06.000Z
>
>* `parseDate(1482940986;X)`
>
>  返回2016-12-28T16:03:06.000Z

## [!UICONTROL addDays(日期；number)] {#adddays-date-number}

返回新日期，以作为向日期添加给定天数的结果。 要减去天数，请输入负数。

>[!INFO]
>
>**示例:**
>
>* `addDays(2016-12-08T15:55:57.536Z;2)`
   >
   >    返回2016-12-10T15:55:57.536Z
>
>* `addDays(2016-12-08T15:55:57.536Z;-2)`
   >
   >    返回2016-12-6T15:55:57.536Z


## [!UICONTROL addHours(日期；number)] {#addhours-date-number}

返回新日期，以作为向日期添加给定小时数的结果。 要减去小时数，请输入负数。

>[!INFO]
>
>**示例:**
>
>* `addHours(2016-12-08T15:55:57.536Z; 2)`
   >
   >    返回2016-12-08T17:55:57.536Z
>
>* `addHours(2016-12-08T15:55:57.536Z;-2)`
   >
   >    返回2016-12-08T13:55:57.536Z


## [!UICONTROL addMinutes(日期；number)] {#addminutes-date-number}

返回新日期，以作为向日期添加给定分钟数的结果。 要减去分钟数，请输入负数。

>[!INFO]
>
>**示例:**
>
>* `addMinutes(2016-12-08T15:55:57.536Z;2)`
   >
   >    返回2016-12-08T15:57:57.536Z
>
>* `addMinutes(2016-12-08T15:55:57.536Z;-2)`
   >
   >    返回2016-12-08T15:53:57.536Z


## [!UICONTROL addMonths(日期；number)] {#addseconds-date-number}

返回新日期，以便向日期添加给定月数。 要减去月份，请输入负数。

>[!INFO]
>
>**示例:**
>
>* `addMonths(2016-08-08T15:55:57.536Z;2)`
   >
   >    返回2016-10-08T15:55:57.536Z
>
>* `addMonths(2016-08-08T15:55:57.536Z;-2)`
   >
   >    返回2016-06-08T15:55:57.536Z


## [!UICONTROL addSeconds(date;number)]

返回新日期，以作为向日期添加给定秒数的结果。 要减去秒数，请输入负数。

>[!INFO]
>
>**示例:**
>
>* `addSeconds(2016-12-08T15:55:57.536Z;2)`
   >
   >   返回2016-12-08T15:55:59.536Z
>
>* `addSeconds(2016-12-08T15:55:57.536Z;-2)`
   >
   >   返回2016-12-08T15:55:55.536Z


## [!UICONTROL addYears(日期；number)]

返回将给定年数添加到日期后的新日期。 要减去年数，请输入负数。

>[!INFO]
>
>**示例:**
>
>* `addYears(2016-08-08T15:55:57.536Z;2)`
   >
   >    返回2018-08-08T15:55:57.536Z
>
>* `addYears(2016-12-08T15:55:57.536Z; -2)`
   >
   >    返回2014-08-08T15:55:57.536Z


## [!UICONTROL setSecond(日期；number)]

此函数会返回一个新日期，其中包含参数中指定的秒数。

指定从0到59的数字。 如果数字在该范围之外，则函数会从前一分钟（对于负数）或后续分钟（对于正数）返回一秒。

如果您需要指定范围外的数字，我们建议您使用[!UICONTROL  addSeconds]，如上节中所述 [addSeconds(date;number)](#addseconds-date-number).

>[!INFO]
>
>**示例:**
>
>* `setSecond(2015-10-07T11:36:39.138Z;10)`
   >
   >    返回2015-10-07T11:36:10.138Z
>
>* `setSecond(2015-10-07T11:36:39.138Z; 6)`
   >
   >    返回2015-10-07T11:37:01.138Z


## [!UICONTROL setMinute(日期；number)]

此函数会返回一个新日期，其中包含参数中指定的分钟数。

指定从0到59的数字。 如果数字超出该范围，则函数会从前一小时（对于负数）或后续小时（对于正数）返回一分钟。

如果您需要指定范围外的数字，我们建议您使用addMinutes，如 [addMinutes(日期；number)](#addminutes-date-number).

>[!INFO]
>
>**示例:**
>
>* `setMinute(2015-10-07T11:36:39.138Z;10)`
   >
   >    返回2015-10-07T11:10:39.138Z
>
>* `setMinute(2015-10-07T11:36:39.138Z;61)`
   >
   >    返回2015-10-07T12:01:39.138Z


## [!UICONTROL setHour(日期；number)]

此函数会返回一个新日期，其中包含参数中指定的小时数。

指定从0到23的数字。 如果数字在此范围之外，则函数会从前一天（对于负数）或后天（对于正数）返回一小时。

如果您需要指定范围外的数字，我们建议您使用addHours，如 [addHours(日期；number)](#addhours-date-number).

>[!INFO]
>
>**示例:**
>
>* `setHour(2015-08-07T11:36:39.138Z;6)`
   >
   >   返回2015-08-07T06:36:39.138Z
>
>* `setHour(2015-08-07T11:36:39.138;-6)`
   >
   >    返回2015-08-06T18:36:39.138Z


## [!UICONTROL setDay(日期；日期编号/名称（英文）]

此函数通过参数中指定的日期返回新日期。

您可以使用此函数将星期设置为1，将星期日设置为1，将星期六设置为7。 如果您指定的数字介于1到7之间，则结果日期在当前（星期日到星期六）周内。 如果数字超出该范围，则函数将返回从前一周（对于负数）或后续周（对于正数）开始的一天。

如果您需要指定范围外的数字，我们建议您使用addDays，如 [addDays(日期；number)](#adddays-date-number).

>[!INFO]
>
>**示例:**
>
>* `setDay(2018-06-27T11:36:39.138Z;Monday)`
   >
   >   返回2018-06-25T11:36:39.138Z
>
>* `setDay(2018-06-27T11:36:39.138Z;1)`
   >
   >   返回2018-06-24T11:36:39.138Z
>
>* `setDay(2018-06-27T11:36:39.138Z;7)`
   >
   >   返回2018-06-30T11:36:39.138Z


## [!UICONTROL setDate(日期；number)]

此函数通过参数中指定的月份日期返回新日期。

指定从1到31的数字。 如果数字超出此范围，则函数将返回上个月（对于负数）或后续月份（对于正数）起的一天。

>[!INFO]
>
>**示例:**
>
>* `setDate(2015-08-07T11:36:39.138Z;5)`
   >
   >   返回2015-08-05T11:36:39.138Z
>
>* `setDate(2015-08-07T11:36:39.138Z;32)`
   >
   >   返回2015-09-01T11:36:39.138Z


## [!UICONTROL setMonth(日期；月份编号/名称（以英语）]

此函数通过参数中指定的月份返回新日期。

指定从1到12的数字。 如果数字超出此范围，则函数将返回上一年（对于负数）或下一年（对于正数）中的月份。

>[!INFO]
>
>**示例:**
>
>* `setMonth(2015-08-07T11:36:39.138Z;5)`
   >
   >   返回2015-05-07T11:36:39.138Z
>
>* `setMonth(2015-08-07T11:36:39.138Z;17)`
   >
   >   返回2016-05-07T11:36:39.138Z
>
>* `setMonth(2015-08-07T11:36:39.138Z;january)`
   >
   >   返回2015-01-07T12:36:39.138Z


## [!UICONTROL setYear(日期；number)]

返回具有参数中指定年份的新日期。

>[!INFO]
>
>**示例:**
>
>* `setYear(2015-08-07T11:36:39.138Z;2017)`
   >
   >   返回2017-08-07T11:36:39.138Z


## [!UICONTROL dateDifference(Date1;日期2;Unit)]

返回一个数字，表示两个日期之间的差异，以指定的单位表示。

日期2从日期1中减去。

对 `unit` 参数：

* 毫秒
* 秒
* 分钟
* 小时
* 天数
* 星期
* 月

如果未指定任何单位，则函数将返回以毫秒为单位的差值。

>[!INFO]
>
>**示例:**
>
>* `dateDifference(2021-05-11T18:10:00.000Z;2021-05-11T18:00:00.000Z)`
   >
   >    返回结果 `600,000`
>
>* `dateDifference(2021-05-11T18:10:00.000Z;2021-05-11T18:00:00.000Z;hours)`
   >
   >    返回结果 `4`
>
>* `dateDifference2021-06-11T18:10:00.000Z;2021-05-11T18:00:00.000Z;months)`
   >
   >    返回结果 `1`


## 其他示例

### 如何计算月中第n天

本节适用于 [!DNL Workfront Fusion] 从 [!DNL Exceljet] 一个网页，该网页说明如何获得一个月内的第n天。

如果您需要计算与月中第n周日（例如，第一个星期二、第三个星期五等）对应的日期，可以使用以下公式：

![](assets/date&time-functions-calc-nth-day-350x31.png)

```
{{addDays(setDate(1.date; 1); 1.n * 7 - formatDate(addDays(setDate(1.date; 1); "-" + 1.dow); "E"))}}
```

公式包含以下项目：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>1.n</code> </td> 
   <td> <p> 第n天：</p> 
    <ul> 
     <li><code>1</code> （第1个星期二）</li> 
     <li><code>2</code> （第2个星期二）</li> 
     <li><code>3</code> 3号星期二，等等</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><code>2.dow</code> </td> 
   <td> <p> 星期：</p> 
    <ul> 
     <li><code>1</code> 表示星期一</li> 
     <li><code>2</code> 表示星期二</li> 
     <li><code>3</code> 表示星期三</li> 
     <li><code>4</code> （星期四）</li> 
     <li><code>5</code> （星期五）</li> 
     <li><code>6</code> 表示星期六</li> 
     <li><code>7</code> 表示星期日</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><code>1.date</code> </td> 
   <td> <p> 日期决定月份。 要计算当月第n天的星期，请使用 <code>now</code> 变量。</p> </td> 
  </tr> 
 </tbody> 
</table>

如果只想计算一个特定情况（例如，每周三一秒），则可以替换这些项目 `1.n` 和 `2.dow` 在公式中具有相应数字。 对于当月的第二个星期三，您将使用以下值：

* `1.n` = `2`
* `1.dow` = `3`
* `1.date` = `now`

![](assets/nth-day-variable-value-350x33.png)

### 解释：

* `setDate(now;1)` 返回当前月份的首个月份
* `formatDate(....;E)` 返回星期(1、2、... 6)

## 如何计算日期之间的天数

一种可能是使用以下表达式：

![](assets/calculate-days-between-dates-350x68.png)

```
{{round((2.value - 1.value) / 1000 / 60 / 60 / 24)}}
```

>[!NOTE]
>
>* 值 `D1`和 `D2` 为日期类型值。 如果它们是字符串类型值(例如20.10.2018)，则使用 `parseDate()` 函数将其转换为日期类型值。
>
>* 的 `round()` 函数用于当其中一个日期在夏令时时间段内，而另一个日期则不在时。 在这些情况下，小时数的差异为小于或大于1小时。 对于非整数结果，可以将其除以24。 您会损失一个小时夏令时。 倒圆角会拼合它，因此您没有百分比


### 如何计算每月的最后一天/毫秒

当您指定日期范围（例如在搜索模块中）时，如果该范围以关闭的间隔（包括其限制点的间隔）跨越整个上个月，则需要计算当月的最后一天。

2019-09-01 ≤ D ≤ 2019-09-30

以下公式显示了计算上个月最后一天的一种方法：

![](assets/last-day-prev-month.png)

```
{{addDays(setDate(now; 1); -1)}}
```

在某些情况下，您不仅需要计算每月的最后一天，还需要计算其最后一毫秒：

2019-09-01T00:00:00.000Z ≤ D ≤ 2019-09-30T23:59:59.999Z

此公式显示了计算上个月最后一毫秒的一种方法：

![](assets/last-millisecond-prev-month-350x45.png)

```
{{parseDate(parseDate(formatDate(now; "YYYYMM01"); "YYYYMMDD"; "UTC") - 1; "x")}}
```

如果需要结果才能使用时区设置，请忽略UTC参数：

![](assets/omit-utc-argument-350x45.png)

`{{parseDate(parseDate(formatDate(now; "YYYYMM01"); "YYYYMMDD") - 1; "x")}}`

但是，最好改用半开间隔（排除其中一个限制点的间隔），改为指定下个月的第一天，并将“小于或等于”运算符替换为“小于”，如下所示：

`2019-09-01 ≤ D < 2019-10-01`

`2019-09-01T00:00:00.000Z ≤ D < 2019-10-01T00:00:00.000Z`
