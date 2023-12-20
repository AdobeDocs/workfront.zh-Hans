---
product-area: reporting
navigation-topic: text-mode-reporting
title: 使用文本模式编辑视图
description: '注意：在文章中添加章节：/Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html ***此外，在文本模式概述文章中起草此区域)'
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '1639'
ht-degree: 1%

---

# 使用文本模式编辑视图

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Also, draft this area in the Text Mode overview article) </p>
-->

您可以使用文本模式编辑列表或报表中的视图，以访问标准界面中不可用的字段并创建更复杂的视图。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对筛选器、视图、分组的访问权限</p> <p>编辑对报告、功能板和日历的访问权限以编辑报告中的报告元素</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对报告的权限以编辑报告中的视图</p> <p>管理视图的权限以编辑它</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在报表或列表中开始使用文本模式之前，请始终确保您熟悉Workfront文本模式语法。

有关更多信息，请参阅：

* [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [文本模式语法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [自定义视图、筛选器和分组示例：文章索引](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 在视图中编辑文本模式

使用文本模式编辑视图对于报告和列表是相同的。 从报表或列表访问视图的方式有所不同。

>[!TIP]
>
>我们建议您在标准模式下构建尽可能多的视图，然后将其转换为文本模式以进行编辑。

有关生成视图的信息，请参阅 [Adobe Workfront中的视图概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

有关创建报告的信息，请参见 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 执行下列操作之一：

   1. 要从报表访问视图，请转到报表，然后单击 **报表操作** > **编辑** > **列（视图）** 选项卡。
   1. 要从列表访问该视图，请转至该列表，然后从 **视图** 下拉菜单，将鼠标悬停在要修改的视图上，然后单击 **编辑** 图标 ![](assets/edit-icon.png).

      此时将打开视图生成器。

1. 在视图中选择一列。

   或

   选择 **列（视图）** 选项卡，然后选择列。

   >[!TIP]
   >
   >要使用文本模式编辑视图，必须一次编辑一列。

1. 单击 **切换到文本模式** 生成器的右上角。

   >[!NOTE]
   >
   >在文本模式下编辑列时，Workfront会添加 `textmode=true` 到列的代码行。 这表示在文本模式下修改了该列。

   ![](assets/switch-to-text-mode-in-view-nwe-highlighted-350x447.png)

   下表概述了文本模式视图中的关键行：

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make this a snippet and add it to the grouping article too)</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>示例行</th> 
      <th>描述</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>valuefield</strong>=</p> </td> 
      <td> <p>这是对象或字段在数据库中显示的名称。 有关对象和字段如何在数据库中显示的详细信息，请参见 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API资源管理器</a>.</p> <p>存在以下情况：</p> 
       <ol> 
        <li value="1"> <p> 如果显示的字段名称是短语而不是单个名词，则必须使用驼峰式大小写语法作为 <code>valuefield</code>. 例如，对于任务的计划开始日期，代码为： </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>如果要显示自定义字段，请 <code>valuefield</code> value是字段的实际名称，如您在界面中所见。 例如，对于名为“更多信息”的自定义字段，代码为：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>如果要显示与视图中的其他对象相关的对象，请使用 <code>valuefield</code> 代码行对象名称和属性用冒号分隔。 </p> <p>例如，任务视图中显示“任务所有者”名称的一列具有以下valuefield行值：Portfolio</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>这表示您可以从报表（任务）的对象中访问下一个相关对象（项目），从那里，您可以从项目（项目组合），然后依次访问项目组合所有者（所有者）及其名称（名称）中的以下相关对象。 </p> </li> 
       </ol> <p>有关对象如何彼此连接的信息，请参阅部分 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">对象的相互依赖性和层次结构</a> 在 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">了解Adobe Workfront中的对象</a>.</p> <p>注：如果在文本模式下选择的字段在标准界面中无效，则无法切换回列中的标准界面。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>值格式=</strong> </td> 
      <td> <p>此行表示用于显示 <code>valuefield</code>. 此 <code>valueformat</code> 标识对象或字段显示为文本、数字、百分比或日期。</p> <p>我们建议使用 <code>HTML</code> 您的 <code>valueformat</code>，尤其是使用 <code>valueexpression</code>，以确保最准确地显示您的信息。 </p> <p>有关此行的其他值的信息，请参见 <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">在文本模式下使用条件格式</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>您可以添加此行来替换 <code>valuefield</code>，以便在列中显示计算字段。</p> <p>您必须将 <code>valuefield</code> 中每次使用大括号内的对象时 <code>valueexpression</code>.</p> <p>存在以下情况： </p> 
       <ol> 
        <li value="1"> <p>如果要以大写形式在列中显示字段，您可以使用：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>此 <code>valuefield</code> 对象的URL将拼写为API Explorer中显示的内容。 </p> </li> 
        <li value="2">如果要添加多个 <code>valuefields</code> 将它们捆绑在一起，必须用句号将它们分开。</li> 
        <li value="3"> <p>例如，如果要显示任务的主要被分配人的姓名，请使用 <code>valueexpression</code>，您将使用：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>如果要在中使用自定义字段 <code>valueexpression</code> 字段名称前面必须加一行 <code>DE:</code> 以指示它是一个自定义字段。 字段的名称在界面中显示时拼写。 </p> <p>重要提示：如果自定义字段放置在权限受限的自定义表单分区中，并且某些用户在报表中查看此计算时，值表达式的计算为空。 有关调整自定义表单分区的权限的信息，请参阅 <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a></span>.</p> <p>例如，如果您有一个标记为“开发人员姓名”的自定义字段，并且您想在列中大写显示此字段，您可以使用以下内容 <code>valueexpression</code> 以指示此情况：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>在引用“预输入”类型自定义字段时，使用以下表达式来引用在标记为“开发人员名称”的字段中选择的对象的名称：</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>descriptionkey= /描述=</strong> </p> </td> 
      <td> <p>当您将鼠标悬停在列的名称上时，此行定义工具提示的文本。 在这种情况下，它使用键来翻译描述文本中的名称值。 如果要修改说明，请将此行更改为： </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>该行定义列标签。 在此例中，它使用基于键的缩写值。</p> <p>如果要修改列名，可将此值更改为： </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> 允许您为列名输入任何文本，而<code>namekey</code> 需要输入用于翻译列名的键。</p> <p>要更改列名，您还可以添加 <code>displayname </code>行（如果不存在）。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>您可以添加以下行来更改列的名称，这将暂停 <code>namekey/name</code> 值：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
     <tr> 
      <td><strong>查询排序=</strong> </td> 
      <td>该行定义在单击列标题时如何对结果进行排序。 如果列不存在，则在运行报告后无法对该列进行排序。</td> 
     </tr> 
     <tr> 
      <td><strong>宽度=</strong> </td> 
      <td> <p>此线条表示用于列的像素数。 如果省略该行或将其设置为0（零），则该列不会出现在视图中。</p> <p>在文本模式下手动修改此字段时，还必须添加 <code>usewidths=true</code> 值到列。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>usewidths=true</strong> </td> 
      <td> <p>除了使用本行外， <code>width=</code> 自定义列宽时的行。 </p> </td> 
     </tr> 
     <tr> 
      <td><strong>makeFieldEditable=</strong> </td> 
      <td> <p>此行定义列中显示的值是否可内联编辑。 如果此行等于 <strong>true</strong>，列中的值可内联编辑。 如果此行等于 <code>false</code>，列中的值不可内联编辑。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valuefield=</strong> </td> 
      <td> <p>仅当希望列中显示的值链接到与其关联的对象时，才插入此行。 该链接将打开对象的详细信息页面。 此值应与 <code>valuefield=</code> 行。 插入时，您还必须添加 <code>link.valueformat=</code> 行。 </p> <p> 例如，您可以插入 <code>link.valuefield=priority</code> 在问题视图中，问题的“优先级”显示为链接。 单击此链接将打开问题页面。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valueformat=</strong> </td> 
      <td> <p>只有在已插入 <code>link.valuefield</code> 行，添加指向列中值的链接。 该链接将打开对象的详细信息页面。 此值应与 <code>valueformat=</code> 行，并指示用于显示 <code>valuefield</code>. </p> <p>重要提示：在也包含链接的内置列中查看文本模式时，您会注意到许多行引用了该链接。 当您在文本模式下创建自己的自定义列并向其中添加链接语句时，其中某些行可能不再受支持或不必要。 添加链接值时必需使用的行包括<code> link.valuefield</code> 和 <code>link.valueformat</code>. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>aggregator.function=</strong> </td> 
      <td> <p>这是指如何汇总每个列的值。 有多行以开头 <code>aggregator.</code> 他们都引用汇总列结果的汇总。 </p> <p>一般来说， <code>aggregator.</code> 行与列对象的行匹配。 </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>">
        <span class="autonumber"><span><b>示例： </b></span></span> 
        <p>任务报告中按“总和”汇总的“计划小时数”列可能如下所示： </p> 
        <div>
         <pre>textmode=true</pre>
         <pre>valuefield=workRequired</pre>
         <pre>valueformat=compound</pre>
         <pre>aggregator.function=SUM</pre>
         <pre>aggregator.valuefield=workRequired</pre>
         <pre>aggregator.displayformat=minutesAsHoursString</pre>
         <pre>aggregator.valueformat=compound</pre>
         <pre>namekey=workRequired</pre>
         <pre>shortview=false</pre> 
        </div> 
       </div> 
       <div>
        此 <code>aggregator. </code>行可以包含 <code>valuefield </code>或 <code>valueexpression</code>
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **应用** 如果要保存更改并继续编辑视图。
1. 单击 **保存+关闭** 以保存报告。

   或

   单击 **保存视图** 在列表中保存视图。
