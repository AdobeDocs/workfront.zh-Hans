---
product-area: reporting
navigation-topic: text-mode-reporting
title: 使用文本模式编辑视图
description: ‘注意：在本文中添加一节：/Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html ***此外，在文本模式概述文章中草拟此区域)`
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '1636'
ht-degree: 1%

---

# 使用文本模式编辑视图

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Also, draft this area in the Text Mode overview article) </p>
-->

您可以使用文本模式在列表或报表中编辑视图，以访问标准界面中不可用的字段，并创建更复杂的视图。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对过滤器、视图、分组的访问权限</p> <p>编辑对报表、功能板、日历的访问权限，以编辑报表中的报表元素</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限以编辑报表中的视图</p> <p>管理要编辑的视图的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

开始在报表或列表中使用文本模式之前，请始终确保您熟悉Workfront文本模式语法。

有关更多信息，请参阅：

* [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [文本模式语法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [自定义视图、过滤器和分组示例](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## 在视图中编辑文本模式

对于报表和列表，使用文本模式编辑视图的方式相同。 从报表或列表访问视图的方式有所不同。

>[!TIP]
>
>我们建议您在标准模式下尽可能多地构建视图，然后将其转换为文本模式以对其进行编辑。

有关构建视图的信息，请参阅 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

有关创建报表的信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 执行下列操作之一：

   1. 要从报表访问视图，请转到报表，然后单击 **报表操作** > **编辑** > **列（视图）** 选项卡。
   1. 要从列表访问视图，请转到列表，然后从 **查看** 下拉菜单中，将鼠标悬停在要修改的视图上，然后单击 **编辑** 图标 ![](assets/edit-icon.png).

      此时会打开视图生成器。

1. 在视图中选择列。

   或

   选择 **列（视图）** 选项卡，然后选择列。

   >[!TIP]
   >
   >要使用文本模式编辑视图，必须一次编辑一列。

1. 单击 **切换到文本模式** 中。

   >[!NOTE]
   >
   >在文本模式下编辑列时，Workfront会将 `textmode=true` 代码行到列。 这表示该列在文本模式下已修改。

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
      <td> <p>这是对象或字段在数据库中显示的名称。 有关对象和字段在数据库中的显示方式的详细信息，请参阅 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>存在以下情形：</p> 
       <ol> 
        <li value="1"> <p> 如果显示的字段名称是短语而不是单个名词，则必须对 <code>valuefield</code>. 例如，对于任务的计划起始日期，代码为： </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>如果要显示自定义字段，请 <code>valuefield</code> value是字段的实际名称，如您在界面中看到的。 例如，对于名为“More information”的自定义字段，代码为：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>如果要使用 <code>valuefield</code> 代码行对象名称和属性以冒号分隔。 </p> <p>例如，任务视图中显示Portfolio所有者名称的列对于值字段行具有以下值：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>这表示从报表（任务）的对象中，您可以访问下一个相关对象（项目），从此处，您可以从项目（项目组合）访问以下相关对象，然后访问项目组合所有者（所有者）及其名称（名称）。 </p> </li> 
       </ol> <p>有关对象如何彼此连接的信息，请参阅部分 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">对象的相互依赖和层次结构</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">了解Adobe Workfront中的对象</a>.</p> <p>注意：如果在文本模式下选择的字段在标准界面中无效，则无法切换回列中的标准界面。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>此行表示用于显示 <code>valuefield</code>. 的 <code>valueformat</code> 标识对象或字段是显示为文本、数字、百分比还是日期。</p> <p>我们建议使用 <code>HTML</code> , <code>valueformat</code>，尤其是在使用 <code>valueexpression</code>，以确保最准确地显示您的信息。 </p> <p>有关此行的其他值的信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">在文本模式中使用条件格式</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>您可以添加此行以替换 <code>valuefield</code>，以在列中显示计算字段。</p> <p>您必须将 <code>valuefield</code> 在 <code>valueexpression</code>.</p> <p>存在以下情形： </p> 
       <ol> 
        <li value="1"> <p>如果要在列中以大写方式显示字段，应使用：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>的 <code>valuefield</code> 对象的拼写形式与在API资源管理器中显示的对象一样。 </p> </li> 
        <li value="2">如果要添加多个 <code>valuefields</code> 把它们串在一起，就必须用一段时间将它们分开。</li> 
        <li value="3"> <p>例如，如果要使用 <code>valueexpression</code>，则会使用：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>如果要在 <code>valueexpression</code> 行，您必须在字段名称之前 <code>DE:</code> 来指示它是自定义字段。 字段名称在界面中显示时拼写。 </p> <p>重要信息：如果您使用的自定义字段位于自定义表单部分中，且该字段对某些用户的权限有限，则当这些用户在报表中查看此计算时，值表达式的计算为空。 有关调整自定义表单部分权限的信息，请参阅 <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a></span>.</p> <p>例如，如果您有一个标有“开发人员名称”的自定义字段，并且希望在列中以大写显示此字段，则可以使用以下内容 <code>valueexpression</code> 以指示：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>引用Typeahead类型自定义字段时，请使用以下表达式引用在标记为“开发人员名称”的字段中选择的对象的名称：</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>descriptionkey= / description=</strong> </p> </td> 
      <td> <p>当您将鼠标悬停在列名称上时，此行将定义工具提示的文本。 在这种情况下，它使用键来翻译描述文本中的名称值。 如果要修改说明，请将此行更改为： </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>此行定义列标签。 在这种情况下，它使用基于键的缩写值。</p> <p>如果要修改列名称，可将此值更改为： </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> 允许您输入列名称的任何文本，而<code>namekey</code> 需要输入用于转换列名称的键。</p> <p>要更改列名称，您还可以在 <code>displayname </code>行，如果没有。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>您可以添加以下行来更改列的名称，该名称将挂起 <code>namekey/name</code> 值：</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例: </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
     <tr> 
      <td><strong>querysort=</strong> </td> 
      <td>此行定义单击列标题时对结果的排序方式。 如果列不存在，则在运行报表后无法对列进行排序。</td> 
     </tr> 
     <tr> 
      <td><strong>width=</strong> </td> 
      <td> <p>此行表示用于列的像素数。 如果忽略该行或将其设置为0（零），则该列不会显示在视图中。</p> <p>在文本模式下手动修改此字段时，还必须添加 <code>usewidths=true</code> 值。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>usewidths=true</strong> </td> 
      <td> <p>除了 <code>width=</code> 行。 </p> </td> 
     </tr> 
     <tr> 
      <td><strong>makeFieldEditable=</strong> </td> 
      <td> <p>此行定义列中显示的值是否可在内联编辑。 如果此行等于 <strong>true</strong>，则列中的值可在内联编辑。 如果此行等于 <code>false</code>，则列中的值不可内联编辑。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valuefield=</strong> </td> 
      <td> <p>仅当您希望列中显示的值链接到与其关联的对象时，才插入此行。 该链接会打开对象的详细信息页面。 此值应与 <code>valuefield=</code> 行。 插入此插件时，还必须将 <code>link.valueformat=</code> 行。 </p> <p> 例如，您可以插入 <code>link.valuefield=priority</code> 在“问题”视图中，“问题的优先级”显示为链接。 单击此链接可打开问题页面。</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valueformat=</strong> </td> 
      <td> <p>仅在插入 <code>link.valuefield</code> 行，以添加指向列中值的链接。 该链接会打开对象的详细信息页面。 此值应与 <code>valueformat=</code> 行和指示用于显示 <code>valuefield</code>. </p> <p>重要信息：在内置列（其中也包含链接）中查看文本模式时，您会注意到引用该链接的行数。 当您在文本模式下创建自己的自定义列并将link语句添加到该列时，这些行中的某些行可能不再受支持或不必要。 添加链接值时必须填写的行为<code> link.valuefield</code> 和 <code>link.valueformat</code>. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>congregator.function=</strong> </td> 
      <td> <p>这是指如何汇总每列的值。 有多行以开头 <code>aggregator.</code> 它们都引用汇总列结果的聚合器。 </p> <p>通常， <code>aggregator.</code> 行与列对象的行匹配。 </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>">
        <span class="autonumber"><span><b>示例: </b></span></span> 
        <p>按“总和”汇总的任务报表中的“计划时数”列可能如下所示： </p> 
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
        的 <code>aggregator. </code>行可以包含 <code>valuefield </code>或 <code>valueexpression</code>
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **应用** 如果要保存更改并继续编辑视图，请执行以下操作：
1. 单击 **保存并关闭** 保存报表。

   或

   单击 **保存视图** 以在列表中保存视图。
