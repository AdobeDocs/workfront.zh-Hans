---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 计算的数据表达式
description: 您可以使用数据表达式在Adobe Workfront中定义计算的自定义数据字段。 它们连接语句中的现有Workfront字段，从而生成新字段。
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 18f26f976a47af003817f2f82f8550bdfbc0ab90
workflow-type: tm+mt
source-wordcount: '2368'
ht-degree: 7%

---

# 计算的数据表达式

您可以使用数据表达式在Adobe Workfront中定义计算的自定义数据字段。 它们连接语句中的现有Workfront字段，从而生成新字段。

您可以在以下位置使用计算的数据表达式：

* 自定义表单

   有关在Workfront中的自定义表单中创建计算的自定义数据字段的更多信息，请参阅 [将计算的数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* 使用文本模式时，报表或列表中的计算自定义列

   有关在报表和视图中使用文本模式的更多信息，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 计算自定义字段与计算自定义列的语法

虽然您使用的函数相同，但在计算自定义字段中构建表达式的语法可能与构建计算自定义列的语法不同。

例如：

* 在自定义字段中，在任务的自定义表单上，您可以使用以下内容生成附加自定义表单的任务的父项目名称：

   ```
   {project}.{name}
   ```

* 在报表的自定义列中，您将使用以下内容在任务报表中添加“项目名称”自定义列：

   ```
   valuefield=project:name
   ```

   或

   ```
   valueexpression={project}.{name}
   ```

   >[!TIP]
   >
   >相同的语法适用于使用计算表达式的所有文本模式报表元素：视图、筛选器、分组、提示。

两种语法之间的差异如下：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>计算的自定义字段</strong></td> 
   <td><strong>计算的自定义报表元素</strong></td> 
  </tr> 
   <td>用大括号括住字段名称。</td> 
   <td>在中使用字段名称时，不要用括号或圆括号括住字段名称 <code>valuefield </code>行。 <p>在中使用字段名称时，请用大括号括住字段名称 <code>valueexpression</code> 行。</p> </td> 
  </tr> 
  <tr> 
   <td>按句点分隔字段。</td> 
   <td> <p>在中使用字段时，请用冒号分隔这些字段 <code>valuefield </code>折线图</p> <p>在中使用字段时，按句点分隔字段 <code>valueexpression </code>行。 </p> </td> 
  </tr> 
 </tbody> 
</table>

有关必须在计算自定义列中使用的语法的更多信息，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 您可以使用的数据表达式

以下列表定义了在Workfront中构建3种不同类型的计算自定义字段之一时可以使用的可用表达式：

* [日期和时间计算的自定义字段](#date-time-calculated-custom-fields)
* [数学计算的自定义字段](#mathematical-calculated-custom-fields)
* [文本计算自定义字段](#text-calculated-custom-fields)

### 日期和时间计算的自定义字段 {#date-time-calculated-custom-fields}

>[!NOTE]
>
>如果创建的日期和时间计算不包括时间部分，或使用日期通配符$$TODAY或$$NOW，则系统将根据协调世界时(UTC)区域而不是您的本地时区使用日期。 这可能会导致出现意外的日期结果。

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
   <td> <p>此表达式将天数添加到日期。 数字值可以包括部分天数（例如，1.5会为日期添加一天半的时间）。</p> <p>表达式的格式如下：</p><pre>ADDDAYS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>此表达式将工作日数添加到日期。 此表达式只将整整数值添加到日期，向下舍入。 </p> <p>表达式的格式如下：</p><pre>ADDWEEKDAYS(日期，数量）</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>此表达式将月数添加到日期，格式如下：</p><pre>ADDMONTHS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>此表达式将年数添加到日期中，格式如下：</p><pre>ADDYEARS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>此表达式清除日期的时间部分，格式如下。 在此示例中，日期是工作对象的输入日期。</p><pre>CLEARTIME({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>日期</strong> </td> 
   <td> <p>此表达式将字符串转换为日期，格式如下：</p><pre>DATE(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>此表达式返回两个日期之间的天数，并会考虑所选时段的开始和结束天数以及这些天的时间戳。 例如，如果开始日期的开始时间为下午3点，则开始日期将不会计为全天。</p> <p>表达式的格式如下：</p><pre>DATEDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>此表达式以数字返回日期的月中日，介于1和31之间。</p> <p>表达式的格式如下。 在此示例中，日期是工作对象的输入日期。</p><pre>DAYOFMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>此表达式以数字返回日期的周内日，在1 （星期日）和7 （星期六）之间。</p> <p>表达式的格式如下。 在此示例中，日期是工作对象的输入日期。</p><pre>DAYOFWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>此表达式按数字返回日期所在月份的总天数，格式如下。 在此示例中，日期是工作对象的输入日期。</p><pre>DAYSINMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>此表达式返回日期与周末或月末（以先到者为准）之间的总工作日。 在此示例中，日期是工作对象的输入日期。</p> <p>表达式的格式如下：</p><pre>DAYSINSPLITWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>此表达式按数字返回日期年份中的总天数，格式如下。 在此示例中，日期是工作对象的输入日期。</p><pre>DAYSINYEAR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>此表达式返回列表中的最新日期，格式如下：</p><pre>DMAX(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>此表达式返回列表中最早的日期，格式如下：</p><pre>DMIN(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>HOUR</strong> </td> 
   <td> <p>此表达式以0到23之间的数字返回日期的小时数。</p> <p>表达式的格式如下。 在此示例中，日期是工作对象的输入日期。</p><pre>HOUR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>此表达式以0到60之间的数字返回日期的分钟数，格式如下。 在此示例中，日期是工作对象的输入日期。</p><pre>MINUTE({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>月</strong> </td> 
   <td> <p>此表达式以1到12之间的数字返回日期的月份，格式如下。 在此示例中，日期是工作对象的输入日期。</p><pre>MONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>此表达式以0到60之间的数字返回日期的秒数，格式如下。 在此示例中，日期是工作对象的输入日期。</p><pre>SECOND({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>此表达式返回两个日期之间的工作日数，同时考虑到所选时段的开始和结束天数以及这些天的时间戳。 例如，如果开始日期的开始时间为下午3点，则开始日期将不会计为全天。</p> <p>表达式的格式如下：</p><pre>WEEKDAYDIFF(date2, date1)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>此表达式根据默认计划返回日期之间计划的分钟数。</p> <p>表达式的格式如下：</p><pre>WORKMINUTESDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>年</strong> </td> 
   <td> <p>此表达式以4位数的形式返回日期的年份，格式如下。 在此示例中，日期是工作对象的输入日期。</p><pre>YEAR({entryDate})</pre> </td> 
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
   <td>此表达式返回数字的绝对值，格式如下。 此示例使用附加了自定义表单的对象下的对象数。<pre>ABS({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>AVERAGE</strong> </td> 
   <td>此表达式返回数字的平均值，格式如下：<pre>AVERAGE(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>此表达式将数字四舍五入到最接近的整数，格式如下。 此示例使用附加了自定义表单的对象下的对象数。<pre>CEIL({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>此表达式按提供的顺序除以所有数字，格式如下：<pre>DIV(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>此表达式将数字向下舍入到最接近的整数，格式如下。 此示例使用附加了自定义表单的对象下的对象数。<pre>FLOOR({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>此表达式返回数字的自然对数值，格式如下：<pre>LN({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>此表达式将数字2的对数值返回到基数number1，格式如下：<pre>LOG(数值1，数值2)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>最大值</strong> </td> 
   <td>此表达式返回列表中最大的项目，格式如下：<pre>MAX(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>最小值</strong> </td> 
   <td>此表达式返回列表中的最小项，格式如下：<pre>MIN(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>数字</strong> </td> 
   <td>此表达式将字符串转换为数字，其格式如下：<pre>NUMBER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>此表达式返回一个以幂为单位的数字，格式如下：<pre>POWER(number, power)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>此表达式将所有数字相乘，格式如下：<pre>PROD(number1, number2, ....)</pre>
   <b>注释</b>

将包含小时数的字段相乘时，请确保您了解所选字段中的小时数是以分钟、小时还是秒的形式保存在数据库中。 如果小时以分钟或秒保存，但在Workfront界面中以小时显示，则在使用此计算编写表达式时，您可能需要考虑从分钟或秒到小时的转换。
</td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>此表达式将数字四舍五入到指定的小数位精度，格式如下：<p>ROUND(number， precision)</p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> 此表达式对数字进行升序排序，格式如下：</p><pre>SORTASCNUM(number1, number2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>此表达式对数字进行降序排序，格式如下：<pre>SORTDESCNUM(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>此表达式返回一个数字的平方根，格式如下。 此示例使用附加了自定义表单的对象下的对象数。</p><pre>SQRT({numberOfChildren})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>此表达式按提供的顺序减去所有数字，格式如下：<pre>SUB(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>总和</strong> </td> 
   <td>此表达式将添加所有数字，格式如下：<pre>SUM(number1, number2, ...)</pre></td> 
  </tr> 
 </tbody> 
</table>

### 文本计算自定义字段 {#text-calculated-custom-fields}

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
   <td> <p>此表达式与其他表达式一起使用，以根据索引号从列表中选择值。 索引号是返回数值（通常在已知范围内）的字段或函数。</p> <p>表达式的格式如下：</p><pre>CASE(indexNumber， value1， value2， ...)</pre> <p>例如，以下表达式在计算列中返回一周中某天的名称，其中1=周日，2=周一，依此类推：</p><pre>CASE(DAYOFWEEK({entryDate})，"星期日"，"星期一"，"星期二"，"星期三"，"星期四"，"星期五"，"星期六")</pre> <p>此表达式最适合用于返回数字的其他表达式，例如DAYOFWEEK、DAYOFMONTH和MONTH。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>此表达式连接字符串，其格式如下：</p><pre>CONCAT(string1，"separator"， string2)</pre> <p>以下是可以包含的分隔符示例：</p> 
    <ul> 
     <li>空格：“ ”</li> 
     <li>短划线：“ — ”</li> 
     <li>斜杠： "/"</li> 
     <li>逗号：“，”</li> 
     <li>单词：“or”、“and”</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>CONTAINS</strong> </td> 
   <td>如果在withinText字符串中找到findText字符串并且其格式如下所示，则此表达式将返回true：<pre>CONTAINS(findText, withinText)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>此表达式可转义字符串中的任何特殊字符，以便将它们包含在URL参数中。<p>表达式的格式如下：</p><pre>ENCODEURL(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>此表达式对指定的条件求值，如果为true，则返回trueExpression的值；如果为false，则返回falseExpression的值。</p> <p>表达式的格式如下：</p><pre>IF(condition, trueExpression, falseExpression)</pre> <p>例如，您可以比较两个不同的日期字段，后跟一个True/False结果作为数据字符串：</p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate}，"Off Track"，"On Track")</pre> <p>在日常讲话中，此语句表示：“如果我的对象的预计完成日期大于”同一对象的计划完成日期，则在此字段中显示“偏离轨道”一词；否则，显示“正在轨道”一词。”</p> <p>如果不希望为true或false表达式添加标签，则必须在语句中插入一个空白标签，例如：</p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate}，"，"On Track")</pre> <p>或</p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate}，"Off Track"，")</pre> <p>有关构建“IF”语句的详细信息，请参见 <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">“IF”语句概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>此表达式允许您在可能值的字符串中查找特定值。 如果您要查找的值等于所提供的值之一，则表达式将返回trueExpression；否则，将返回falseExpression。</p> <p>表达式的格式如下：</p><pre>IFIN(value， value1， value2，...， trueExpression， falseExpression)</pre> <p>例如，您可以找到特定的项目所有者，并在项目视图中使用指定的标记标记标记这些项目： <br><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")</code></p> <p> 在日常演讲中，此声明的意思是：“如果项目所有者是Jennifer Campbell或Rick Kuvec，则使用‘营销团队’标记此项目；否则，使用‘其他团队’标记此项目。”</p> <p> 如果不希望为true或false表达式添加标签，则必须在语句中插入一个空白标签，例如： </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> <p>或 </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team",""</code> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>位于‍</strong> </td> 
   <td> <p>如果该值等于所提供的值之一，则此表达式将返回true；否则，该表达式将返回false。</p> <p>表达式的格式如下：</p><pre>IN(值，值1[，值2...])</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>如果值为null或空，则此表达式返回true；否则，表达式返回false。</p> <p>表达式的格式如下：</p><pre>ISBLANK(value)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>左</strong> </td> 
   <td> <p>此表达式从字符串的左侧返回指定数目的字符，格式如下：</p><pre>LEFT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>此表达式返回字符串的长度，格式如下：</p><pre>LEN(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>此表达式返回小写的字符串，其格式如下：<pre>LOWER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>替换</strong> </td> 
   <td> <p>此表达式在string1中将string2的所有匹配项替换为string3。</p> <p>表达式的格式如下：</p><pre>REPLACE(string1, string2, string3)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>右</strong> </td> 
   <td> <p>此表达式从字符串的右侧返回指定数目的字符，格式如下：</p><pre>RIGHT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SEARCH</strong> </td> 
   <td> <p>此表达式返回字符串withinText中findText第一次出现的索引，从给定的起始位置开始，如果找不到文本，则返回–1。</p> <p>表达式的格式如下：</p><pre>SEARCH(findText， withinText， start)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>字符串</strong> </td> 
   <td> <p>此表达式将数字转换为字符串，其格式如下：</p><pre>STRING(number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>此表达式对字符串列表进行升序排序，格式如下：</p><pre>SORTASCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> 此表达式对字符串列表进行降序排序，格式如下：</p><pre>SORTDESCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>此表达式根据指定的开始索引和结束索引返回字符串的字符，格式如下：</p><pre>SUBSTR（{string}，起始位置数，结束位置数）</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>此表达式用于去除字符串开头和结尾的空格，格式如下：</p><pre>TRIM(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>此表达式返回一个大写字符串，其格式如下：</p><pre>UPPER(string)</pre> </td> 
  </tr> 
 </tbody> 
</table>
