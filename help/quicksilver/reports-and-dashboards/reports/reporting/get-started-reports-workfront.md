---
content-type: overview;reference
product-area: reporting
navigation-topic: reporting-navigation-topic
title: 开始使用Adobe Workfront中的报表
description: 报表可以显示用户和工作的进展情况。 使用报表，可显示有关Adobe Workfront中对象的信息。
author: Nolan
feature: Reports and Dashboards
exl-id: 478512af-a47c-4488-878a-581e238e0064
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '3449'
ht-degree: 0%

---

# 开始使用Adobe Workfront中的报表

报表可以显示用户和工作的进展情况。 使用报表，可显示有关Adobe Workfront中对象的信息。

有关了解对象以及如何在Workfront应用程序中报告对象的信息，请参阅 [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 报表元素

报表是Workfront中以下三个元素的组合：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">查看</td> 
   <td> <li>定义报表中的列以及可包含在每个列中的信息。</li> <li>有关视图的信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">视图Adobe Workfront概述</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">分组</td> 
   <td> <li>根据常用信息对信息进行分类，并在蓝色标题下列出报告结果。</li> <li>有关分组的信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Adobe Workfront中的分组概述</a>.</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">筛选</td> 
   <td> <li>控制报表中显示的信息量。</li> <li>有关过滤器的信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">过滤器Adobe Workfront概述</a>.</li> <li>有关过滤器修饰符的信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">过滤器和条件修饰符</a>.</li> <li>您可以使用通配符进行筛选，以使筛选器更加常规，并更加灵活地使用。</li> <li>有关在过滤器中使用通配符的信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">通配符过滤器变量</a>.</li> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>当您从列表中选择新过滤器、查看或分组时，即使您注销Workfront或关闭浏览器，该选择也会保留。

有关报表元素的信息，请参阅文章 [报表元素：过滤器、视图和分组](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

要增强报表，可添加以下元素：

* 图表：结果在报表中的可视表示形式。\
   有关图表报表的信息，请参阅文章 [将图表添加到报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* 矩阵分组：以汇总表格式汇总报表信息。\
   有关矩阵报表的信息，请参阅文章 [创建矩阵报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* 提示：一个打开过滤器，每次运行报表时，您都可以通过不同的方式自定义和应用该过滤器。\
   有关提示的信息，请参阅 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

在构建报表时，您可以在报表生成器中单独修改其中的任何元素。

提高报告中所包含信息相关性的另一种方法是对视图应用条件格式。\
有关使用条件格式的信息，请参阅 [在视图中使用条件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## 系统报告

Workfront会提供默认加载到系统中的多个系统报表。\
在系统中输入信息后，您可以使用这些报表以可视方式显示信息。

有关如何访问系统报告的信息，请参阅 [使用Adobe Workfront内置报表](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md) 在文章中 [使用Adobe Workfront内置报表](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

有关哪些系统报告可用的更多信息，请参阅文章 [使用Adobe Workfront内置报表](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

## 创建报表

除了Workfront提供的系统报表之外，您还可以创建自己的自定义报表以满足您组织的需求。

要创建报表，您可以执行以下操作之一：

* 从头开始构建报表。
* 复制现有报表。\
   您必须至少具有“查看”权限才能复制其他人创建的报表。 有关复制报表的更多信息，请参阅文章 [创建报表副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

有关创建报告的信息，请参阅文章 [日历报表概述](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

* [创建报告的先决条件](#prerequisites-for-creating-reports)
* [报表所有权](#report-ownership)
* [在生成器界面中创建报表](#create-reports-in-the-builder-interface)
* [在文本模式下创建报表](#create-reports-in-text-mode)

### 创建报告的先决条件 {#prerequisites-for-creating-reports}

* 您必须拥有计划许可证才能创建自己的报告。\
   有关Workfront许可证类型的信息，请参阅文章 [Adobe Workfront许可证概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

* 您的Workfront管理员必须授予您在访问级别中编辑报表的访问权限。\
   有关授予对“编辑”报表的访问权限的信息，请参阅文章 [授予对报表、功能板和日历的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Workfront管理员必须授予您在访问级别中“编辑过滤器”、“视图”和“分组”的访问权限。

   有关授予对“编辑过滤器”、“视图”和“分组”的访问权限的信息，请参阅 [授予对过滤器、视图和分组的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* 您必须定义一个要报告的对象。 报表是Workfront中特定的对象，您必须先选择对象类型，然后才能开始构建报表。 您只能报告Workfront界面中可用的对象。

### 报表所有权 {#report-ownership}

在Workfront中创建报表时，您将成为报表的默认所有者，并会显示在我的报表部分。 您无法更改报表的所有者。

在复制报表时，您会自动成为复制报表的所有者。

有关复制报表的信息，请参阅文章 [创建报表副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

您可以通过查看 **输入者** 字段。

![](assets/nwe-entered-by-350x218.png)

### 在生成器界面中创建报表 {#create-reports-in-the-builder-interface}

我们建议您首先使用报表生成界面来生成新报表。 界面提供了一组简化的工具，可指导您将元素组合在一起以创建所需的报表。 您有一些对象和字段，可以从列表中选择这些对象和字段，并将其添加到所有报表元素。\
有关在报告构建界面中创建报告的更多信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

有关可报告的对象列表，请参阅 [对象报告](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) 章节 [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

有关可在报表中显示的字段的详细信息，请参阅文章 [Adobe Workfront术语表](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

### 在文本模式下创建报表 {#create-reports-in-text-mode}

有时，您可能无法在生成器界面中找到某些字段，但它们可能在API中可用。\
有关API中可用字段的信息，请参阅文章 [API Explorer](../../../wf-api/general/api-explorer.md).

有关如何使用API资源管理器的信息，请参阅文章 [使用API资源管理器](../../../wf-api/general/using-api-explorer.md).

>[!NOTE]
>
>无法在Workfront界面中报告报表生成器中不可用的对象。 但是，如果这些字段通过API可用，则可以报告与报表生成器中的对象关联的字段。 要实现此目的，必须使用文本模式界面。

文本模式允许您使用标准模式界面中不可用的字段，从而创建更复杂的视图、过滤器、分组和提示。

* [文本模式术语](#text-mode-terminology)
* [文本模式的计算列、条件格式和其他用法](#calculated-columns-conditional-formatting-and-other-uses-of-text-mode)
* [文本模式示例](#text-mode-samples)

#### 文本模式术语 {#text-mode-terminology}

必须使用特定语法才能使用Workfront文本模式界面。

有关文本模式的Workfront语法的更多详细信息，请参阅 [文本模式语法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

#### 文本模式的计算列、条件格式和其他用法 {#calculated-columns-conditional-formatting-and-other-uses-of-text-mode}

在报告生成器界面中不可用的字段之外，您可以使用文本模式显示某些字段之间的计算或比较。

有关报表中文本模式最常用用法的列表，请参阅文章 [文本模式常见用法概述](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

有关在报表中包含计算的自定义数据的信息，请参阅部分 [报表中的计算自定义数据](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

有关比较条件格式中字段的信息，请参阅文章 [比较条件格式中的字段](../../../reports-and-dashboards/reports/text-mode/compare-fields-conditional-formatting.md).

您还可以在报表中使用文本模式引用收藏集字段。\
有关使用文本模式在报表中显示收藏集信息的信息，请参阅文章 [在报表中引用集合](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

#### 文本模式示例 {#text-mode-samples}

我们拥有一个库，其中包含您可以使用文本模式创建的最常用视图、过滤器和分组的示例。

要浏览此库并使用我们提供的一些示例，请参阅文章 [自定义视图、过滤器和分组示例](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md).

## 报表的选项卡

在界面中运行报表时，报表可以包含多个选项卡。

有关运行报表的信息，请参阅文章 [运行报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

在每个选项卡上，报表中包含的信息以略微不同的格式显示。 选择最适合贵组织需求的格式。

您可以将任何选项卡设为报表的默认选项卡。 默认选项卡是在单击报表名称以将其打开时显示的第一个选项卡，它是在将报表置于功能板上时显示的选项卡。

根据您在报表中选择的元素，报表可以包含以下选项卡：

* [“详细信息”选项卡](#details-tab)
* [“摘要”选项卡](#summary-tab)
* [“矩阵”选项卡](#matrix-tab)
* [“图表”选项卡](#chart-tab)
* [“提示”选项卡](#prompts-tab)

### “详细信息”选项卡 {#details-tab}

报表的“详细信息”(Details)选项卡在列表形式中显示报表的对象以及为该对象选择的属性。 每个报表都有一个“详细信息”选项卡。

>[!IMPORTANT]
>
>“详细信息”选项卡中的信息显示方式可能与“图表”选项卡不同，具体视您所在时区而定。\
>例如，加利福尼亚的某位用户在2月12日晚上9:30（太平洋标准时间）完成了一项任务。 当纽约的用户查看包含此任务完成情况的报表时，“详细信息”选项卡中的“实际完成日期”显示为2月13日，因为该报表是在2月13日东部标准时间凌晨12:30完成的。 但是，在图表中，它包含在2月12日的分组中，直到您展开图表元素为止。

### “摘要”选项卡 {#summary-tab}

包含分组的报表具有“摘要”选项卡。

“详细信息”选项卡上以列表格式显示的相同信息会根据“摘要”选项卡上报表中的分组进行汇总和汇总。

有关分组的信息，请参阅文章 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

### “矩阵”选项卡 {#matrix-tab}

包含矩阵分组的报表具有“矩阵”选项卡。

“详细信息”(Details)选项卡上以列表格式显示的相同信息以表格格式显示，按“矩阵”(Matrix)选项卡的报表中的分组进行分组。

在将矩阵分组添加到报表时，“摘要”选项卡会被“矩阵”选项卡替换。

有关构建矩阵分组的信息，请参阅文章 [创建矩阵报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

### “图表”选项卡 {#chart-tab}

包含图表的报表具有“图表”选项卡。

考虑在报表中包含一个图表，以便为执行人员提供具有影响力的功能板。 图表是在报表中显示信息的简洁方式。 您可以通过单击图表元素来展开该元素，以显示该元素中包含的项目。

>[!IMPORTANT]
>
>单击图表元素时，展开的信息可能会根据您的时区与图表显示不同。\
>例如，加利福尼亚的某位用户在2月12日晚上9:30（太平洋标准时间）完成了一项任务。 当纽约的用户查看包含此任务完成情况的报表时，“详细信息”选项卡和“图表”详细信息中的“实际完成日期”都显示为2月13日，因为该报表是在2月13日东部标准时间凌晨12:30完成的。 但是，在图表中，它包含在2月12日的分组中，直到您展开图表元素为止。

有关使用图表构建报表的信息，请参阅文章 [将图表添加到报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

### “提示”选项卡 {#prompts-tab}

包含提示的报表具有“提示”选项卡。

每次运行报表时，系统都会显示一条提示，提示您向报表中添加过滤器。 在向报表添加提示时，“提示”选项卡会自动成为报表的默认选项卡。 不能将其更改为其他选项卡。

有关生成报告提示的信息，请参阅文章 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## 共享报表

创建报表后，您可以与其他用户共享该报表。

您可以通过以下方式与其他用户共享报表：

* [为报表授予共享权限](#give-sharing-permissions-to-a-report)
* [计划报表提交](#schedule-a-report-delivery)
* [导出报表结果](#export-the-results-of-a-report)
* [将报表添加到功能板](#add-a-report-to-a-dashboard)

### 为报表授予共享权限 {#give-sharing-permissions-to-a-report}

您可以为其他用户授予查看或管理您创建的报表的共享权限。 您可以为其他用户授予的权限级别等于或小于您的权限级别。 您还可以使用共享权限将报表设为公用报表。 有关共享报表的信息，请参阅 [在Adobe Workfront中共享报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### 计划报表提交 {#schedule-a-report-delivery}

您可以计划报表提交。 与您共享报表的用户会收到一封电子邮件，其中包含报表结果的附件。 附件可采用以下格式：

* HTML
* PDF
* Excel
* .TSV

有关计划报表提交的信息，请参阅文章 [报表交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

### 导出报表结果 {#export-the-results-of-a-report}

可以将报表结果导出为以下文件格式

* PDF
* Excel（.xls和.xlsx格式）
* 制表符分隔

有关导出报表结果的信息，请参阅文章 [导出数据](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

将报表导出为其中一种格式后，您可以通过以附件形式发送电子邮件或打印来与其他用户共享该报表。

### 将报表添加到功能板 {#add-a-report-to-a-dashboard}

您可以将报表添加到功能板，并与其他用户共享该功能板。 有关将报表添加到功能板的信息，请参阅文章 [将报表添加到功能板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

## 创建日历

如果要以日历格式显示数据，可以创建日历而不是报表。

有关构建日历的信息，请参阅文章。

有关使用日历的信息，请参阅文章 [日历报表概述](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## 报表使用情况

创建报表并与其他用户共享这些报表后，您可以跟踪他们使用这些报表的频率。\
有关报表使用情况（包括查看频率、用户查看次数、显示功能板）的信息，请参阅文章 [报表使用情况概述](../../../reports-and-dashboards/reports/report-usage/report-usage-overview.md).

## 在报告中使用的常见术语

以下术语在参考Workfront报表时使用：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>术语或短语</strong> </th> 
   <th><strong>定义</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>高级选项</td> 
   <td> <p>指Report Builder的列（视图）选项卡上的链接，通过该链接，可以执行以下操作：</p> 
    <ul> 
     <li>根据您选择的条件设置文本和图像的列条件样式格式。</li> 
     <li>重新标记您的列。</li> 
     <li>设置列值的格式。</li> 
    </ul> <p>例如，您可能希望以粗体显示所有父任务，或者如果任务延迟，则可能希望以红色显示计划完成日期。</p> </td> 
  </tr> 
  <tr> 
   <td>属性</td> 
   <td> 数据库中定义的对象的字段。 它用在文本模式表达式中。 <br>例如，“状态”字段显示为 <em>状态</em> 在文本模式表达式中使用时。 </td> 
  </tr> 
  <tr> 
   <td>Bean或JavaBean</td> 
   <td>Bean表示可重用的编程元素。 术语Bean标识Workfront应用程序中不同对象之间的关系。 当您尝试显示有关基本报表工具中不可用对象的其他属性时，请务必熟悉这些关系。</td> 
  </tr> 
  <tr> 
   <td>生成器界面或Report Builder</td> 
   <td>“生成器界面”是一系列下拉菜单，其中包含列（视图）、过滤器和分组选项卡中显示的字段。 它提供Bean关系的直观映射，以帮助识别视图中的列、过滤器的标准以及分组的通用属性。</td> 
  </tr> 
  <tr> 
   <td>驼峰</td> 
   <td> <p>驼峰式大小写是指将编程元素写入字符串多字属性的一种特定方式。 在驼峰式拼写属性时，第一个单词的第一个字母小写，单词之间没有空格，任何后续单词的第一个字母都是大写的。</p> <p>例如，Home Group将写为 <em>homeGroup</em>，资源池将为 <em>resourcePool</em>，实际开始日期为 <em>actualStartDate</em>.</p> </td> 
  </tr> 
  <tr> 
   <td>图表</td> 
   <td> <p>在保存报表后，报表生成器中会显示一个选项卡、一个报表选项卡，以及一个可选的报表元素，通过该元素可向任何报表添加图表。 在创建图表之前，必须在报表中定义分组。</p> <p>以下是可添加到任何报表的图表类型：<br></p> 
    <ul> 
     <li>列</li> 
     <li>条形图</li> 
     <li>饼图</li> 
     <li>行</li> 
     <li>计量</li> 
     <li>气泡</li> 
    </ul> <p>有关将图表添加到报表的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">将图表添加到报表</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>详细信息</td> 
   <td>这是保存报表后报表的其中一个选项卡。 它显示报告的结果，显示在您选择的视图和分组中。</td> 
  </tr> 
  <tr> 
   <td>表达式</td> 
   <td>表达式是文本模式下的书写公式，用于在使用文本模式界面时传递要搜索或显示的信息。 它通常是较大的文本模式语句中的一行。</td> 
  </tr> 
  <tr> 
   <td>字段</td> 
   <td> <p>指对象的属性。 例如，“状态”是“项目”、“任务”或“问题”的字段。 “Portfolio管理器”是Portfolio对象的字段。</p> <p>您还可以拥有自行创建并添加到自定义Forms的自定义字段。<br>有关创建自定义Forms的信息，请参阅文章 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>字段名称 </td> 
   <td>在视图中显示、在过滤器条件中使用，或作为分组的公共元素的属性值。 字段名称的选项取决于字段源的选择。</td> 
  </tr> 
  <tr> 
   <td>字段源 </td> 
   <td>在视图中显示、在过滤器条件中使用，或作为分组公共元素的对象值。 字段源中的选项取决于所创建UI元素的对象类型。 字段源允许您从UI元素的对象类型以外的对象引用属性。</td> 
  </tr> 
  <tr> 
   <td>筛选</td> 
   <td>一个主报表元素，可确定报表中显示的结果。</td> 
  </tr> 
  <tr> 
   <td>表单 </td> 
   <td>可与“自定义表单”互换使用。 字段和部分会添加到表单中，然后附加到对象，以扩展可与对象关联的字段数。</td> 
  </tr> 
  <tr> 
   <td>分组 </td> 
   <td>一个主报表元素，用于标识结果列表的组织方式。 “分组”会在整个报表中创建水平条，以按创建结果时定义的通用属性对结果进行分组。 矩阵报表中使用分组来聚合数据，图表中也使用分组来确定图表的轴。</td> 
  </tr> 
  <tr> 
   <td>对象或对象类型</td> 
   <td> 对象是Workfront应用程序元素（即，项目、任务、组、公司、过滤器）。 创建新报表、查看、过滤器或分组时，会使用“对象类型”来标识报表的焦点对象。 报表只能具有一个对象类型，该对象类型是报表的主要对象。<br>可在同一报表中引用父对象。<br>有关对象层次结构的更多信息，请参阅文章中的“了解对象的相互依赖关系和层次结构”一节 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">了解Adobe Workfront中的对象</a>.</td> 
  </tr> 
  <tr> 
   <td>提示</td> 
   <td> <p>可选的报表元素，当您需要在每次运行报表之前运行其他过滤器时，可以将其添加到报表中。</p> <p>有关提示的信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">过滤器和条件修饰符</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>限定符或条件修改量</td> 
   <td> <p>此字段显示在报表的以下区域：</p> 
    <ul> 
     <li>在过滤器选项卡上</li> 
     <li>列（视图）选项卡中列的高级选项屏幕。 通过定义限定符，可以将字段名称与其他字段或值进行比较。</li> 
     <li> 在自定义提示中<br>有关自定义提示的信息，请参阅文章中的“创建提示”部分 <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">过滤器和条件修饰符</a>.</li> 
    </ul> <p>例如，在为计划完成日期为今天的任务构建过滤器时，您可以选择 <strong>等于</strong> 在限定词字段中，在日期字段中显示今天的日期：</p> <p><em>任务&gt;计划完成日期&gt;等于&gt;（当天日期）</em> </p> <p>在此方案中，限定符为 <strong>等于</strong>.<br>有关限定符的详细信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">过滤器和条件修饰符</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>报告 </td> 
   <td>视图、过滤器和（有时）分组的组合。 报表的用途是在整个界面中始终如一地显示数据，分发信息，并且无需定期运行相同的搜索或查询。</td> 
  </tr> 
  <tr> 
   <td>语句</td> 
   <td>由多个表达式组成，用于定义使用文本模式时报表中显示的信息。 可以为报表中的查看、过滤、分组或自定义提示创建语句。</td> 
  </tr> 
  <tr> 
   <td>摘要</td> 
   <td>这是保存报表后报表的其中一个选项卡。 仅当您为报表定义分组时，才会创建此选项卡。 它根据在报表创建过程中定义的分组来总结信息，并快速概述报表的聚合对象。 它不会显示报表中的每个对象，而只显示聚合的对象。</td> 
  </tr> 
  <tr> 
   <td>文本模式界面</td> 
   <td>提供创建或修改最初通过生成器界面创建的自定义视图、过滤器、分组和提示代码的功能。 建议报表元素最初通过生成器界面创建，并在保存后转换为文本模式，以简化高级视图、过滤器、分组或提示的编码。</td> 
  </tr> 
  <tr> 
   <td>用户界面(UI)</td> 
   <td>是指用户在任何给定时间的屏幕上显示的内容的组件或构建基块。</td> 
  </tr> 
  <tr> 
   <td>视图（或列）</td> 
   <td>报表的主要元素之一。 它标识将在报表列表中显示的列标题。</td> 
  </tr> 
 </tbody> 
</table>
