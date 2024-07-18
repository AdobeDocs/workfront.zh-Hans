---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 计算数据表达式概述
description: 您可以使用数据表达式在Adobe Workfront中定义计算的自定义数据字段。 计算表达式将生成新字段的语句中的现有Workfront字段连接在一起。
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '2165'
ht-degree: 0%

---

# 计算数据表达式概述

<!--Audited: 12/2023-->

您可以使用数据表达式在Adobe Workfront中定义计算的自定义字段。 计算表达式将生成新字段的语句中的现有Workfront字段连接在一起。

您可以在以下位置使用计算数据表达式：

* 自定义表单上的计算自定义字段

  有关在Workfront中的自定义表单中创建计算自定义字段的更多信息，请参阅[将计算字段添加到表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。

* 使用文本模式时，报表或列表中的计算自定义列

  有关在报表和视图中使用文本模式的详细信息，请参阅[文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

## 计算自定义字段与计算自定义列的语法

尽管使用的函数相同，但在计算自定义字段中构建表达式的语法可能与构建计算自定义列的语法不同。

两种语法的区别在于：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>计算的自定义字段</strong></td> 
   <td><strong>计算的自定义报表元素</strong></td> 
  </tr> 
   <td>用大括号括住字段名称</td> 
   <td>在中使用字段名称时，请勿将其括在方括号或圆括号中 <p><code>valuefield </code></p>行。 <p>在中使用字段名称时，用大括号括住字段名称 <p><code>valueexpression</code></p> 行。</p> </td> 
  </tr> 
  <tr> 
   <td>按句点分隔字段</td> 
   <td> <p>在中使用字段时，请用冒号分隔这些字段 <p><code>valuefield </code></p>折线图</p> <p>在中使用字段时，按句点分隔字段 <p><code>valueexpression </code></p>行。 </p> </td> 
  </tr> 
 </tbody> 
</table>

例如：

* 在自定义字段中，在任务的自定义表单上，使用以下内容生成附加自定义表单的任务的父级项目的名称：


  ` {project}.{name}`


* 在报表的自定义列中，您将使用以下内容在任务报表中添加“项目名称”自定义列：


  `valuefield=project:name`


  或

  `valueexpression={project}.{name}`


  >[!TIP]
  >
  >相同的语法适用于使用计算表达式的所有文本模式报表元素：视图、筛选器、分组、提示。

有关计算自定义列中必须使用的语法的详细信息，请参阅[文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

## 您可以使用的数据表达式

以下列表定义了在Workfront中构建3种不同类型的计算自定义字段之一时可以使用的可用表达式：

* [已计算的日期和时间自定义字段](#date-time-calculated-custom-fields)
* [数学计算的自定义字段](#mathematical-calculated-custom-fields)
* [文本计算的自定义字段](#text-calculated-custom-fields)

您可以使用下面列出的表达式来构建计算的自定义列。 但是，必须对计算自定义列使用正确的语法，如本文中计算自定义字段与计算自定义列的语法[一节中所述](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns)。

### 日期和时间计算的自定义字段 {#date-time-calculated-custom-fields}

>[!NOTE]
>
>如果创建的日期和时间计算不包括时间部分，或者使用日期通配符$$TODAY或$$NOW，则系统将根据协调世界时(UTC)区域使用日期，而不是根据您的本地时区。 这可能会导致意外的日期结果。

您可以使用以下表达式创建日期或时间计算自定义字段：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>表达式</th> 
   <th>说明和示例</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ADDDAYS</strong> </td> 
   <td> <p>向日期添加天数。 数值可包含部分天数。 例如，1.5会向日期添加一个半天。</p> <p>表达式的格式如下所示：</p>

<p><code>ADDDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>将工作日数添加到日期。 此表达式只将整整数值添加到日期，向下舍入。 </p> <p>表达式的格式如下所示：</p>

<p><code>ADDWEEKDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>将月数添加到日期，格式如下：

</p><p><code>ADDMONTHS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>将年数添加到日期中，格式如下：</p>

<p><code>ADDYEARS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>清除日期的时间部分，格式如下。 在本例中，日期是工作对象的“输入日期”。</p>

<p><code>CLEARTIME({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>日期</strong> </td> 
   <td> <p>将字符串转换为日期，格式如下：</p>

<p><code>DATE(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>返回两个日期之间的天数，并会考虑所选时段的开始和结束日期以及这些日期的时间戳。 例如，如果开始日期的开始时间为下午3点，则开始日期不会计为全天。</p> <p>表达式的格式如下所示：</p>

<p><code>DATEDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>按数值返回日期的月中日，介于1和31之间。</p> <p>表达式的格式如下所示。 在本例中，日期是工作对象的“输入日期”。</p>

<p><code>DAYOFMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>按数值返回日期的周内日，在1 （星期日）和7 （星期六）之间。</p> <p>表达式的格式如下所示。 在本例中，日期是工作对象的“输入日期”。</p>

<p><code>DAYOFWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>按数值返回日期月内的总天数，格式如下。 在本例中，日期是工作对象的“输入日期”。</p>

<p><code>DAYSINMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>返回日期与周末或月末（以先到者为准）之间的总工作日。 在本例中，日期是工作对象的“输入日期”。</p> <p>表达式的格式如下所示：</p>

<p><code>DAYSINSPLITWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>按数值返回日期年内的总天数，格式如下。 在本例中，日期是工作对象的“输入日期”。</p>

<p><code>DAYSINYEAR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>返回列表中最新的日期，格式如下：</p>

<p><code>DMAX(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>分钟</strong> </td> 
   <td> <p>返回列表中最早的日期，格式如下：</p>

<p><code>DMIN(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>小时</strong> </td> 
   <td> <p>以0到23之间的数字返回日期的小时数。</p> <p>表达式的格式如下所示。 在本例中，日期是工作对象的“输入日期”。</p>

<p><code>HOUR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>分钟</strong> </td> 
   <td> <p>以0到60之间的数字返回日期的分钟数，格式如下。 在本例中，日期是工作对象的“输入日期”。</p>

<p><code>MINUTE({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>个月</strong> </td> 
   <td> <p>按1到12之间的数字返回日期的月份，格式如下。 在本例中，日期是工作对象的“输入日期”。</p>

<p><code>MONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>秒</strong> </td> 
   <td> <p>以0到60之间的数字返回日期的秒数，格式如下。 在本例中，日期是工作对象的“输入日期”。</p>

<p><code>SECOND({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>返回两个日期之间的工作日数，同时考虑到所选时段的开始和结束日期以及这些日期的时间戳。 例如，如果开始日期的开始时间为下午3点，则开始日期将不会计为全天。</p> <p>表达式的格式如下所示：</p>

<p><code>WEEKDAYDIFF(date2, date1)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>根据默认计划返回日期之间的计划分钟数。</p> <p>表达式的格式如下所示：</p>

<p><code>WORKMINUTESDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>年</strong> </td> 
   <td> <p>以4位数字返回日期的年份，格式如下。 在本例中，日期是工作对象的“输入日期”。</p>

<p><code>YEAR({entryDate})</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### 数学计算的自定义字段 {#mathematical-calculated-custom-fields}

您可以创建使用以下某些数学表达式的计算自定义字段：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>表达式</th> 
   <th>说明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ABS</strong> </td> 
   <td>返回该数字的绝对值，格式如下。 此示例使用附加自定义表单的对象下的对象数。

<p><code>ABS({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>平均</strong> </td> 
   <td>返回数字的平均值，格式如下：

<p><code>AVERAGE(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>将数字四舍五入到最接近的整数，格式如下。 此示例使用附加自定义表单的对象下的对象数。

<p><code>CEIL({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>按照提供的顺序除以所有数字，格式如下：

<p><code>DIV(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>楼层</strong> </td> 
   <td>将数字下调到最接近的整数，格式如下。 此示例使用附加自定义表单的对象下的对象数。

<p><code>FLOOR({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>返回该数字的自然对数值，格式如下：

<p><code>LN({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>日志</strong> </td> 
   <td>将数值2的对数值返回至基数1，格式如下：

<p><code>LOG(number1, number2)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>返回列表中的最大项目，格式如下：

<p><code>MAX(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>分钟</strong> </td> 
   <td>返回列表中的最小项目，格式如下：

<p><code>MIN(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>数字</strong> </td> 
   <td>将字符串转换为数字，格式如下：<p><code>NUMBER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>电源</strong> </td> 
   <td>返回提升为次幂的数字，格式如下：

<p><code>POWER(number, power)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>生产</strong> </td> 
   <td>将所有数字相乘，格式如下：

<p><code>PROD(number1, number2, ....)</code></p>
   <p><b>注释</b></p>

<p>将包含小时数的字段相乘时，请确保您了解数据库是将所选字段中的小时数保存为分钟、小时还是秒。 如果小时以分钟或秒保存，但在Workfront界面中以小时显示，则在使用此计算编写表达式时，您可能需要考虑从分钟或秒到小时的转换。 </p>
   </td> 
  </tr> 
  <tr> 
   <td><strong>轮</strong> </td> 
   <td>将数字四舍五入到指定的小数位精度，格式如下：

<p><code>ROUND(number, precision)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> 对数字进行升序排序，格式如下：</p>

<p><code>SORTASCNUM(number1,number2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>对数字进行降序排序，格式如下：

<p><code>SORTDESCNUM(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>返回一个数字的平方根，格式如下。 此示例使用附加自定义表单的对象下的对象数。</p>

<p><code>SQRT({numberOfChildren})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>按提供的顺序减去所有数字，格式如下：

<p><code>SUB(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>总和</strong> </td> 
   <td>将所有数字相加，格式如下：

<p><code>SUM(number1, number2, ...)</code></p></td> 
  </tr> 
 </tbody> 
</table>

### 文本计算的自定义字段 {#text-calculated-custom-fields}

您可以创建计算自定义字段，该字段使用以下表达式显示文本格式的值：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>表达式</th> 
   <th>说明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>案例</strong> </td> 
   <td> <p>与其他表达式一起使用，根据索引号从列表中选择值。 </p>
   <p>索引号是返回数值（通常在已知范围内）的字段或函数。</p> 
   <p>表达式的格式如下所示：</p>
   <p><code>CASE(indexNumber, value1, value2, ...)</code></p>

<p>例如，以下表达式在计算列中返回一周中某天的名称，其中1=周日，2=周一，依此类推：</p>

<p><code>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</code></p>

<p>最适合用于返回数字的其他表达式，例如DAYOFWEEK、DAYOFMONTH和MONTH。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>连接字符串，其格式如下：</p><p><code>CONCAT(string1,"separator", string2)</code></p> <p>以下是您可以包括的分隔符示例：</p> 
    <ul> 
     <li>空格：“ ”</li> 
     <li>短划线：“ — ”</li> 
     <li>斜杠： "/"</li> 
     <li>逗号：“，”</li> 
     <li>单词：“或”、“和”</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>包含</strong> </td> 
   <td>如果在withinText字符串中找到findText字符串并且其格式如下所示，则返回真：

<p><code>CONTAINS(findText, withinText)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>去除字符串中的任何特殊字符，使其可被包含在URL参数中。<p>表达式的格式如下所示：</p>

<p><code>ENCODEURL(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>评估指定的条件，如果为true，则返回trueExpression的值；如果为false，则返回falseExpression的值。</p>

<p>表达式的格式如下所示：</p>

<p><code>IF(condition, trueExpression, falseExpression)</code></p>

<p>例如，您可以比较两个不同的日期字段，后跟一个True/False结果作为数据字符串：</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</code></p>

<p>在日常讲话中，此语句表示：“如果我的对象的预计完成日期大于”同一对象的计划完成日期，则在此字段中显示“偏离轨道”一词；否则，显示“正在轨道”一词。”</p>

<p>如果不希望为true或false表达式添加标签，则必须在语句中插入一个空白标签，例如：</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</code></p> 
   <p>或</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</code></p>

<p>有关生成“IF”语句的详细信息，请参阅<a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">“IF”语句概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>允许您在可能值的字符串中查找特定值。 如果您要查找的值等于所提供的值之一，则表达式将返回trueExpression；否则，将返回falseExpression。</p> 
   <p>表达式的格式如下所示：</p>

<p><code>IFIN(value, value1, value2,..., trueExpression, falseExpression)</code></p>

<p>例如，您可以查找特定的项目所有者，并在项目视图中使用指定标记标记标记这些项目： <br><p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")
   </code></p>
    <p> 在日常演讲中，此声明的意思是：“如果项目所有者是Jennifer Campbell或Rick Kuvec，则使用‘营销团队’标记此项目；否则，使用‘其他团队’标记此项目。”</p> 
    <p> 如果不希望为true或false表达式添加标签，则必须在语句中插入一个空白标签，例如： </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> 
    <p>或 </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","")</code></p> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>位于</strong> </td> 
   <td> <p>如果值与提供的值之一相等，则返回true；否则，表达式返回false。</p> <p>表达式的格式如下所示：

</p><p><code>IN(value, value1[, value2...])</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>如果值为null或空，则返回true；否则，表达式返回false。</p> <p>表达式的格式如下所示：

</p><p><code>ISBLANK(value)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>已离开</strong> </td> 
   <td> <p>从字符串的左侧返回指定数目的字符，格式如下：</p>

<p><code>LEFT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>返回字符串的长度，其格式如下：</p>

<p><code>LEN(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>返回小写的字符串，其格式如下：

<p><code>LOWER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>替换</strong> </td> 
   <td> <p>在string1中，将所有出现的string2替换为string3。</p> <p>表达式的格式如下所示：</p>

<p><code>REPLACE(string1, string2, string3)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>右</strong> </td> 
   <td> <p>从字符串的右侧返回指定数目的字符，格式如下：</p>

<p><code>RIGHT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>搜索</strong> </td> 
   <td> <p>返回字符串withinText中findText第一次出现的索引，从给定的起始位置开始；如果找不到文本，则返回–1。</p> <p>表达式的格式如下所示：</p>

<p><code>SEARCH(findText, withinText, start)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>字符串</strong> </td> 
   <td> <p>将数字转换为字符串，其格式如下：</p>

<p><code>STRING(number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>以升序排序一个字符串列表，格式如下：</p>

<p><code>SORTASCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> 以降序排序一个字符串列表，格式如下：</p>

<p><code>SORTDESCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>根据指定的开始索引和结束索引返回字符串的字符，其格式如下：</p>

<p><code>SUBSTR({string}, number of start position, number of end position)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>修剪</strong> </td> 
   <td> <p>删除字符串开头和结尾的空格，格式如下：</p>

<p><code>TRIM(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>返回大写的字符串，格式如下：</p>

<p><code>UPPER(string)</code></p> </td> 
  </tr> 
 </tbody> 
</table>
