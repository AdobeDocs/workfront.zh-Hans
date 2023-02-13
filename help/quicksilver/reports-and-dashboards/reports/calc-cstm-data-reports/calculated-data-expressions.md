---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 计算数据表达式
description: 您可以在Adobe Workfront中使用数据表达式定义计算的自定义数据字段。 它们将现有的Workfront字段连接到生成新字段的语句中。
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 22438c38727f5cc36b07b3530818f5bda2b0bacf
workflow-type: tm+mt
source-wordcount: '2270'
ht-degree: 7%

---

# 计算数据表达式

您可以在Adobe Workfront中使用数据表达式定义计算的自定义数据字段。 它们将现有的Workfront字段连接到生成新字段的语句中。

您可以在以下位置使用计算数据表达式：

* 自定义表单

   有关在Workfront中的自定义表单上创建计算自定义数据字段的更多信息，请参阅 [将计算数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* 使用文本模式时，报表或列表中的计算自定义列

   有关在报表和视图中使用文本模式的更多信息，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 计算自定义字段与计算自定义列的语法

尽管您使用的函数相同，但在计算自定义字段中构建表达式的语法可能与在构建计算自定义列时所用的语法不同。

例如：

* 在自定义字段中，对于任务的自定义表单，您可以使用以下方法生成附加了自定义表单的任务的父项目的名称：

   ```
   {project}.{name}
   ```

* 在报表的自定义列中，您可以使用以下方法在任务报表中添加项目名称自定义列：

   ```
   valuefield=project:name
   ```

   或

   ```
   valueexpression={project}.{name}
   ```

   >[!TIP]
   >
   >相同的语法适用于使用计算表达式的所有文本模式报表元素：视图、过滤器、分组、提示。

这两种语法的区别是：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>计算的自定义字段</strong></td> 
   <td><strong>计算的自定义报表元素</strong></td> 
  </tr> 
   <td>用大括号括住字段名称。</td> 
   <td>在 <code>valuefield </code>行。 <p>在 <code>valueexpression</code> 行。</p> </td> 
  </tr> 
  <tr> 
   <td>按句点分隔字段。</td> 
   <td> <p>在 <code>valuefield </code>行</p> <p>在 <code>valueexpression </code>行。 </p> </td> 
  </tr> 
 </tbody> 
</table>

有关在计算自定义列中必须使用的语法的更多信息，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 您可以使用的数据表达式

以下列表定义了在Workfront中构建3种不同类型的计算自定义字段之一时可以使用的可用表达式：

* [日期和时间计算的自定义字段](#date-time-calculated-custom-fields)
* [数学计算的自定义字段](#mathematical-calculated-custom-fields)
* [文本计算的自定义字段](#text-calculated-custom-fields)

### 日期和时间计算的自定义字段 {#date-time-calculated-custom-fields}

>[!NOTE]
>
>如果您创建的日期和时间计算不包含时间部分，或者使用日期通配符$$TODAY或$NOW，则系统会根据协调通用时间(UTC)区域来使用日期，而不是根据您的本地时区。 这可能会导致意外的日期结果。

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
   <td> <p>此表达式向日期添加天数，其格式如下：</p><pre>ADDDAYS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>此表达式向日期添加工作日数，其格式如下：</p><pre>ADDWEEKDAYS(日期，数量）</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>此表达式将月数添加到日期，其格式如下：</p><pre>ADDMONTHS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>此表达式向日期添加年数，其格式如下：</p><pre>ADDYEARS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>此表达式清除日期的时间部分，并按照以下方式进行格式设置。 在本例中，日期是工作对象的条目日期。</p><pre>CLEARTIME({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>日期</strong> </td> 
   <td> <p>此表达式将字符串转换为日期，其格式如下：</p><pre>DATE(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>此表达式会返回两个日期之间的天数，同时考虑所选时段的开始和结束天数以及这些日期的时间戳。 例如，如果开始日期的开始时间为下午3点，则开始日期将不会计为一整天。</p> <p>表达式的格式如下：</p><pre>DATEDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>此表达式将日期的月份日期作为数字返回，介于1到31之间。</p> <p>表达式的格式如下。 在本例中，日期是工作对象的条目日期。</p><pre>DAYOFMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>此表达式以数字形式返回日期在一周中的某一天，介于1（星期日）到7（星期六）之间。</p> <p>表达式的格式如下。 在本例中，日期是工作对象的条目日期。</p><pre>DAYOFWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>此表达式将日期月份的总天数作为数字返回，其格式如下。 在本例中，日期是工作对象的条目日期。</p><pre>DAYSINMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>此表达式会返回日期与周末或月末（以先到者为准）之间的总工作日。 在本例中，日期是工作对象的条目日期。</p> <p>表达式的格式如下：</p><pre>DAYSINSPLITWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>此表达式将日期年份中的总天数作为数字返回，其格式如下。 在本例中，日期是工作对象的条目日期。</p><pre>DAYSINYEAR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>此表达式会在列表中返回最新日期，其格式如下：</p><pre>DMAX(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>此表达式返回列表中的最早日期，其格式如下：</p><pre>DMIN(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>HOUR</strong> </td> 
   <td> <p>此表达式会以0到23之间的数字返回日期的小时数。</p> <p>表达式的格式如下。 在本例中，日期是工作对象的条目日期。</p><pre>HOUR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>此表达式会以介于0到60之间的数字返回日期的分钟数，格式如下。 在本例中，日期是工作对象的条目日期。</p><pre>MINUTE({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>月</strong> </td> 
   <td> <p>此表达式将日期的月份作为介于1和12之间的数字返回，格式如下。 在本例中，日期是工作对象的条目日期。</p><pre>MONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>此表达式将日期的第二个值作为介于0和60之间的数字返回，格式如下。 在本例中，日期是工作对象的条目日期。</p><pre>SECOND({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>此表达式会返回两个日期之间的工作日数，同时考虑所选时段的开始和结束日以及这些日期的时间戳。 例如，如果开始日期的开始时间为下午3点，则开始日期将不会计为一整天。</p> <p>表达式的格式如下：</p><pre>WEEKDAYDIFF(date2, date1)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>此表达式会根据默认计划返回日期之间的计划分钟数。</p> <p>表达式的格式如下：</p><pre>WORKMINUTESDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>年</strong> </td> 
   <td> <p>此表达式将日期的年份作为4位数字返回，格式如下。 在本例中，日期是工作对象的条目日期。</p><pre>YEAR({entryDate})</pre> </td> 
  </tr> 
 </tbody> 
</table>

### 数学计算的自定义字段 {#mathematical-calculated-custom-fields}

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
   <td>此表达式返回数字的绝对值，其格式如下。 此示例使用附加了自定义表单的对象下的对象数。<pre>ABS({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>AVERAGE</strong> </td> 
   <td>此表达式返回数字的平均值，其格式如下：<pre>AVERAGE(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>此表达式将数字舍入为最接近的整数，其格式如下。 此示例使用附加了自定义表单的对象下的对象数。<pre>CEIL({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>此表达式按提供的顺序划分所有数字，其格式如下：<pre>DIV(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>此表达式将数字向下舍入为最接近的整数，其格式如下。 此示例使用附加了自定义表单的对象下的对象数。<pre>FLOOR({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>此表达式返回数字的自然对数值，其格式如下：<pre>LN({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>此表达式将number2的对数值返回为基数1，其格式如下：<pre>LOG(数值1，数值2)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>此表达式返回列表中最大的项目，其格式如下：<pre>MAX(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>MIN</strong> </td> 
   <td>此表达式返回列表中最小的项目，其格式如下：<pre>MIN(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>数字</strong> </td> 
   <td>此表达式将字符串转换为数字，其格式如下：<pre>NUMBER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>此表达式会返回一个引号为幂的数字，其格式如下：<pre>POWER(number, power)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>此表达式乘以所有数字，其格式如下：<pre>PROD(number1, number2, ....)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>此表达式会将数字舍入为指定的精度小数，并按照以下方式进行格式设置：<p>ROUND（数字，精度）</p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> 此表达式按升序排列数字，其格式如下：</p><pre>SORTASCNUM(number1, number2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>此表达式按降序排列数字，其格式如下：<pre>SORTDESCNUM(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>此表达式返回数字的平方根，其格式如下。 此示例使用附加了自定义表单的对象下的对象数。</p><pre>SQRT({numberOfChildren})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>此表达式按提供的顺序减去所有数字，格式如下：<pre>SUB(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>此表达式会添加所有数字，其格式如下：<pre>SUM(number1, number2, ...)</pre></td> 
  </tr> 
 </tbody> 
</table>

### 文本计算的自定义字段 {#text-calculated-custom-fields}

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
   <td><strong>CASE</strong> </td> 
   <td> <p>此表达式可与其他表达式结合使用，根据索引编号从列表中选择一个值。 索引编号是返回数值（通常在已知范围内）的字段或函数。</p> <p>表达式的格式如下：</p><pre>CASE(indexNumber， value1, value2, ...)</pre> <p>例如，以下表达式在计算列中返回星期的名称，其中1=Sunday， 2=Monday，依此类推：</p><pre>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","星期二","Weinday","星期四","Friday","Saturday")</pre> <p>此表达式最适合返回数字的其他表达式，如DAYOFWEEK、DAYOFMONTH和MONTH。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>此表达式可连接字符串，其格式如下：</p><pre>CONCAT(string1,"separator", string2)</pre> <p>以下是可以包含的分隔符示例：</p> 
    <ul> 
     <li>空格：" "</li> 
     <li>短划："-"</li> 
     <li>斜杠："/"</li> 
     <li>逗号：","</li> 
     <li>一个词："or"、"and"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>CONTAINS</strong> </td> 
   <td>如果在withinText字符串中找到findText字符串，则此表达式会返回true，其格式如下：<pre>CONTAINS(findText, withinText)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>此表达式会转义字符串中的任何特殊字符，以便将其包含在URL参数中。<p>表达式的格式如下：</p><pre>ENCODEURL(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>此表达式会计算您指定的条件，如果为true，则返回trueExpression的值；如果为false，则返回falseExpression的值。</p> <p>表达式的格式如下：</p><pre>IF(condition, trueExpression, falseExpression)</pre> <p>例如，您可以将两个不同的日期字段后跟一个True/False结果作为数据字符串进行比较：</p><pre>IF({projectedCompletionDate}&gt;{planedCompletionDate},"Off Track","On Track")</pre> <p>在日常讲话中，这句话意味着：“如果我对象的预计完成日期为‘大于’我同一对象的计划完成日期，则在此字段中显示‘偏离轨道’字样；否则，显示“在跟踪”字样。</p> <p>如果不想为true或false表达式添加标签，则必须在语句中插入空白标签，例如：</p><pre>IF({projectedCompletionDate}&gt;{planedCompletionDate},"","On Track")</pre> <p>或</p><pre>IF({projectedCompletionDate}&gt;{planedCompletionDate},"Off Track","")</pre> <p>有关构建“IF”语句的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">“IF”语句概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>此表达式允许您在可能值的字符串中查找特定值。 如果要查找的值等于提供的值之一，则表达式会返回trueExpression;否则，返回falseExpression。</p> <p>表达式的格式如下：</p><pre>IFIN(value， value1, value2,..., trueExpression， falseExpression)</pre> <p>例如，您可以在项目视图中找到特定项目所有者，并使用指定的标记标记这些项目： <br><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")</code></p> <p> 在日常讲话中，这句话意味着：“如果项目所有者是Jennifer Campbell或Rick Kuvec，则使用‘营销团队’标记此项目；否则，使用“其他团队”标记。”</p> <p> 如果不想为true或false表达式添加标签，则必须在语句中插入空白标签，例如： </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> <p>或 </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team",""</code> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>位于‍</strong> </td> 
   <td> <p>如果值等于提供的值之一，则此表达式会返回true;否则，表达式会返回false。</p> <p>表达式的格式如下：</p><pre>IN(值，值1[，值2...])</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>如果值为null或空，则此表达式会返回true;否则，表达式会返回false。</p> <p>表达式的格式如下：</p><pre>ISBLANK(value)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>左</strong> </td> 
   <td> <p>此表达式从字符串左侧返回指定数量的字符，其格式如下：</p><pre>LEFT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>此表达式返回字符串的长度，其格式如下：</p><pre>LEN(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>此表达式以小写形式返回字符串，其格式如下：<pre>LOWER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>替换</strong> </td> 
   <td> <p>此表达式会将string1中字符串2的所有实例替换为string3。</p> <p>表达式的格式如下：</p><pre>REPLACE(string1, string2, string3)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>右</strong> </td> 
   <td> <p>此表达式从字符串右侧返回指定数量的字符，其格式如下：</p><pre>RIGHT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SEARCH</strong> </td> 
   <td> <p>此表达式会从给定的开始位置开始，返回字符串中findText第一个实例的索引，如果未找到文本，则返回–1。</p> <p>表达式的格式如下：</p><pre>SEARCH(findText， withinText， start)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>字符串</strong> </td> 
   <td> <p>此表达式将数字转换为字符串，其格式如下：</p><pre>STRING(number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>此表达式对字符串列表进行升序排序，其格式如下：</p><pre>SORTASCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> 此表达式按降序对字符串列表进行排序，其格式如下：</p><pre>SORTDESCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>此表达式根据指定的开始和结束索引返回字符串的字符，其格式如下：</p><pre>SUBSTR（{string}，开始位置数，结束位置数）</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>此表达式从字符串的开头和结尾删除空格，其格式如下：</p><pre>TRIM(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>此表达式以大写形式返回字符串，其格式如下：</p><pre>UPPER(string)</pre> </td> 
  </tr> 
 </tbody> 
</table>
