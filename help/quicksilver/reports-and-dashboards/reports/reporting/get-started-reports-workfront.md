---
content-type: overview;reference
product-area: reporting
navigation-topic: reporting-navigation-topic
title: 报告入门
description: 通过报告，可查看用户和工作的最新动态。 使用报表，您可以显示有关Adobe Workfront中对象的信息。
author: Nolan
feature: Reports and Dashboards
exl-id: 478512af-a47c-4488-878a-581e238e0064
source-git-commit: e9d1e35a9c94143a84eb2007985a42f0960a09f7
workflow-type: tm+mt
source-wordcount: '3293'
ht-degree: 0%

---

# 报告入门

<!-- Audited: 12/2023 -->

通过报告，可查看用户和工作的最新动态。 使用报表，您可以显示有关Adobe Workfront中对象的信息。

有关了解对象以及如何在Workfront应用程序中报告对象的信息，请参阅[Adobe Workfront对象概述](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)。

## 报表元素

报表是Workfront中以下三个元素的组合：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">查看</td> 
   <td> <li>定义报表中的列以及每列可包含的信息。</li> <li>有关视图的信息，请参阅Adobe Workfront中的<a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">视图概述</a>。</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">分组</td> 
   <td> <li>根据常见的信息对信息进行分类，并在标题下列出报告结果。</li> <li>有关分组的信息，请参阅Adobe Workfront中的<a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">分组概述</a>。</li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">筛选条件</td> 
   <td> <li>控制报表中显示的信息量。</li> <li>有关筛选器的信息，请参阅<a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">筛选器概述</a>。</li> <li>有关筛选器修饰符的信息，请参阅<a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">筛选器和条件修饰符</a>。</li> <li>您可以使用通配符进行过滤，以使过滤器更通用，并为其提供更大的使用灵活性。</li> <li>有关在筛选器中使用通配符的信息，请参阅<a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">通配符筛选器变量</a>。</li> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>当您从列表中选择新的筛选器、视图或分组时，即使您注销Workfront或关闭浏览器，该选择仍会保留。

有关报表元素的信息，请参阅[报表元素：筛选器、视图和分组](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)。

要增强报表，可添加以下元素：

* 图表：报表中结果的可视表示形式。\
  有关图表报表的信息，请参阅[将图表添加到报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

* 矩阵分组：汇总汇总汇总表格式的报表信息。\
  有关矩阵报表的信息，请参阅[创建矩阵报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)。

* 提示：打开过滤器，每次运行报表时，您都可以对其进行不同的自定义和应用。\
  有关提示的信息，请参阅[向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)。

在构建报表时，您可以在Report Builder中单独修改其中的任何元素。

增强报表中包含的信息相关性的另一种方法是将条件格式应用于视图。 有关使用条件格式的信息，请参阅[在视图中使用条件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)。

## 系统报表

Workfront提供了多个默认加载到系统中的系统报告。\
在系统中输入信息后，您可以使用这些报表直观地显示信息。

有关如何访问系统报告以及哪些系统报告可用的详细信息，请参阅[使用Adobe Workfront内置报告](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)。

## 创建报告

除了Workfront提供的系统报告之外，您还可以创建自己的自定义报告，以满足贵组织的需求。

要创建报告，您可以执行以下操作之一：

* 从头开始构建报表。
* 复制现有报表。

  您必须至少具有“查看”权限才能复制其他人创建的报告。 有关复制报告的详细信息，请参阅[创建报告的副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)。

有关创建报告的信息，请参阅[创建自定义报告](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

### 创建报告的先决条件 {#prerequisites-for-creating-reports}

* 您必须拥有Plan许可证（当前许可证）或Standard许可证（新许可证）才能创建自己的报告。

  有关Workfront许可证类型的信息，请参阅当前许可证的[许可证概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md)和新许可证的[新许可证概述](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md)。

* 您的Workfront管理员必须为您授予在访问级别编辑报表的权限。

  有关授予对“编辑”报告的访问权限的信息，请参阅[授予对报告、功能板和日历的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)。

* 您的Workfront管理员必须为您授予在访问级别编辑筛选器、视图和组的权限。

  有关授予对编辑筛选器、视图和分组的访问权限的信息，请参阅[授予对筛选器、视图和分组的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)。

* 您必须定义一个要报告的对象。 报告是Workfront中的特定对象，您必须先选择对象类型，然后才能开始构建报告。 您只能报告Workfront界面中可用的对象。

### 报告所有权 {#report-ownership}

在Workfront中创建报告时，您成为该报告的默认所有者，并显示在您的“我的报告”部分中。 您无法更改报告的所有者。

当您复制报告时，您会自动成为所复制报告的所有者。
有关复制报告的信息，请参阅[创建报告副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)。

您可以通过查看&#x200B;**输入者**&#x200B;字段来查看报表的所有者。

![输入者字段](assets/unshimmed-entered-by.png)

### 在生成器界面中创建报表 {#create-reports-in-the-builder-interface}

我们建议您首先使用报表生成界面来生成新报表。 该界面提供了一组简化的工具，可指导您逐步将元素集中在一起，以创建所需的报表。 您有可从列表中选择并添加到所有报表元素的对象和字段。\
有关在报告生成界面中创建报告的详细信息，请参阅[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

有关可以报告的对象列表，请参阅文章[Adobe Workfront对象概述](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)中的[对象报告](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#report-on-objects)部分。

有关可在报表中显示的字段的更多信息，请参阅[Adobe Workfront术语词汇表](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

### 在文本模式下创建报表 {#create-reports-in-text-mode}

有时，您可能无法在生成器界面中找到某些字段，但这些字段可能在API中可用。\
有关API中哪些字段可用的信息，请参阅文章[API资源管理器](../../../wf-api/general/api-explorer.md)。

有关如何使用API Explorer的信息，请参阅文章[使用API Explorer](../../../wf-api/general/using-api-explorer.md)。

>[!NOTE]
>
>您无法在Workfront界面中报告在Report Builder中不可用的对象。 但是，如果通过API可以获得与Report Builder中的对象关联的字段，则可以报告这些字段。 要实现此目的，必须使用文本模式界面。

文本模式允许您使用标准模式界面中不可用的字段，从而创建更复杂的视图、筛选器、分组和提示。

#### 文本模式术语 {#text-mode-terminology}

您必须使用特定语法才能使用Workfront文本模式界面。

有关文本模式的Workfront语法的更多详细信息，请参阅[文本模式语法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)。

#### 计算列、条件格式和文本模式的其他用法 {#calculated-columns-conditional-formatting-and-other-uses-of-text-mode}

在生成器界面中不可用的字段的报表之外，您可以使用文本模式显示特定字段之间的计算或比较。

有关报告中文本模式最常见用法的列表，请参阅[文本模式常见用法概述](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)。

有关在报表中包括计算的自定义数据的信息，请参阅[报表中的计算的自定义数据](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md)。

有关比较条件格式中的字段的信息，请参阅[比较条件格式中的字段](../../../reports-and-dashboards/reports/text-mode/compare-fields-conditional-formatting.md)。

您还可以在报表中使用文本模式引用收藏集字段。\
有关使用文本模式在报表中显示集合信息的信息，请参阅[引用报表中的集合](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)。

#### 文本模式示例 {#text-mode-samples}

我们有一个示例库，其中包含您可以使用文本模式创建的最常用的视图、筛选器和分组。

要浏览此库并使用我们提供的某些示例，请参阅文章[自定义视图、筛选器和分组示例：文章索引](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)。

## 报告的选项卡

在界面中运行报告时，报告可以包含多个选项卡。

有关运行报表的信息，请参阅文章[运行报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md)。

在每个选项卡上，您在报表中包含的信息以略微不同的格式显示。 选择最适合您组织需求的格式。

您可以将任何选项卡设置为报表的默认选项卡。 默认选项卡是单击报表名称以将其打开时显示的第一个选项卡，也是将报表放在仪表板上时显示的选项卡。

### “详细信息”选项卡 {#details-tab}

报告的“详细信息”选项卡在列表表单中显示报告的对象以及您为该对象选择的属性。 每个报表都有一个详细信息选项卡。

>[!IMPORTANT]
>
>根据您的时区，“详细信息”选项卡中的信息可能与“图表”选项卡中的信息显示方式不同。\
>例如，加利福尼亚的一位用户在2月12日晚上9:30 PST完成了一项任务。 当纽约用户查看包含此任务完成的报表时，实际完成日期在“详细信息”选项卡和“图表”详细信息中显示为2月13日，因为实际完成日期在2月13日东部标准时间凌晨12:30完成。 但是，在图表中，它包含在2月12日分组中，直到您展开图表元素为止。

### “摘要”选项卡 {#summary-tab}

包含分组的报表具有“摘要”选项卡。

“详细信息”选项卡上以列表格式显示的相同信息将根据“摘要”选项卡上的报告中的分组进行汇总和汇总。

有关分组的信息，请参阅Adobe Workfront中的[分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。

### “矩阵”选项卡 {#matrix-tab}

包含Matrix Grouping的报告具有Matrix选项卡。

“详细信息”选项卡上以列表格式显示的相同信息以表格格式显示，在“矩阵”选项卡上的报告中按分组分组。

将Matrix分组添加到报表时， Summary选项卡将替换为Matrix选项卡。

有关构建矩阵分组的信息，请参阅文章[创建矩阵报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)。

### “图表”选项卡 {#chart-tab}

包含图表的报表具有图表选项卡。

考虑在您的报告中包含一个图表，以便对您的执行人员形成有影响力的功能板。 图表是一种在报告中显示信息的简洁方式。 您可以通过单击图表元素来展开该元素，以显示该元素中包含的项目。

>[!IMPORTANT]
>
>单击某个图表元素时，展开的信息可能会根据您的时区显示与图表不同的内容。\
>例如，加利福尼亚的一位用户在2月12日晚上9:30 PST完成了一项任务。 当纽约用户查看包含此任务完成的报表时，实际完成日期在“详细信息”选项卡和“图表”详细信息中显示为2月13日，因为实际完成日期在2月13日东部标准时间凌晨12:30完成。 但是，在图表中，它包含在2月12日分组中，直到您展开图表元素为止。

有关使用图表构建报告的信息，请参阅文章[将图表添加到报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

### “提示”选项卡 {#prompts-tab}

包含提示的报告具有提示选项卡。

每次运行报表时，系统都会提示您向报表中添加过滤器。 向报告添加提示时，“提示”选项卡将自动成为报告的默认选项卡。 无法更改到其他选项卡。

有关为报表生成提示的信息，请参阅文章[向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)。

## 共享报表

创建报表后，您可以与其他用户共享该报表。

### 向报告授予共享权限 {#give-sharing-permissions-to-a-report}

您可以将共享权限授予其他用户查看或管理您创建的报表。 您可以为其他用户授予与您的权限相同或更低的权限级别。 您还可以使用共享权限公开报表。 有关共享报告的信息，请参阅[在Adobe Workfront中共享报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)。

### 计划报表提交 {#schedule-a-report-delivery}

您可以计划报表提交。 您共享报告的用户将收到一封包含报告结果附件的电子邮件。 附件可采用以下格式：

* HTML
* PDF
* Excel
* .TSV

有关计划报表传送的信息，请参阅[报表传送概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

### 导出报告结果 {#export-the-results-of-a-report}

可将报告结果导出为以下文件格式：

* PDF
* Excel （.xls和.xlsx格式）
* 制表符分隔

有关导出报告结果的信息，请参阅[导出数据](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)。

在将报告导出为上述一种格式后，您可以通过通过电子邮件将报告作为附件发送或打印来与其他用户共享。

### 将报表添加到功能板 {#add-a-report-to-a-dashboard}

您可以将报表添加到功能板并与其他用户共享该功能板。 有关将报告添加到仪表板的信息，请参阅[将报告添加到仪表板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md)。

## 创建日历

如果要以日历格式显示数据，可以创建日历而不是报告。

有关生成和使用日历的信息，请参阅[日历报告概述](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md)。

## 报告使用情况

创建报告并与其他用户共享后，您可以跟踪他们使用这些报告的频率。
有关报告使用情况的信息，包括查看频率、查看者以及所显示功能板，请参阅文章[报告使用情况概述](../../../reports-and-dashboards/reports/report-usage/report-usage-overview.md)。

## 用于引用报告的常用术语

以下术语用于引用Workfront报表：

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
   <td> <p>引用Report Builder的列（视图）选项卡上的链接，该链接提供了执行以下操作的功能：</p> 
    <ul> 
     <li>根据您选择的条件设置文本和图像的列条件样式格式。</li> 
     <li>为列重新添加标签。</li> 
     <li>设置列中值的格式。</li> 
    </ul> <p>例如，您可能希望以粗体显示所有父级任务，或者，如果任务延迟，您可能希望以红色显示“规划完成日期”。</p> </td> 
  </tr> 
  <tr> 
   <td>属性</td> 
   <td> 数据库中定义的对象字段。 在文本模式表达式中使用它。 <br>例如，在文本模式表达式中使用时，状态字段显示为<em>状态</em>。 </td> 
  </tr> 
  <tr> 
   <td>Bean或JavaBean</td> 
   <td>Bean表示可重用的编程元素。 术语Bean标识Workfront应用程序中不同对象之间的关系。 在尝试显示有关基本报告工具中不可用的对象的其他属性时，务必熟悉这些关系。</td> 
  </tr> 
  <tr> 
   <td>生成器界面或Report Builder</td> 
   <td>生成器界面是一系列下拉菜单，其中包含显示在列（视图）、筛选器和分组选项卡中的字段。 它提供了Bean关系的直观映射，以帮助确定视图中的列、过滤器的标准和分组的公共属性。</td> 
  </tr> 
  <tr> 
   <td>驼峰式大小写</td> 
   <td> <p>Camel Case是指将编程元素写入到一起字符串多个单词属性的特定方法。 在驼峰式拼写属性时，第一个单词的第一个字母是小写，单词之间没有空格，任何后续单词的第一个字母是大写。</p> <p>例如，主组将写为<em>homeGroup</em>，资源池将为<em>resourcePool</em>，实际开始日期将为<em>actualStartDate</em>。</p> </td> 
  </tr> 
  <tr> 
   <td>图表</td> 
   <td> <p>Report Builder中的选项卡，保存报告后的报告选项卡，以及可用于向任何报告添加图表的可选报告元素。 在创建图表之前，必须在报告中定义分组。</p> <p>以下是可添加到任何报表中的图表类型：<br></p> 
    <ul> 
     <li>列</li> 
     <li>条形图</li> 
     <li>饼图</li> 
     <li>行</li> 
     <li>计量</li> 
     <li>气泡</li> 
    </ul> <p>有关将图表添加到报表的更多信息，请参阅文章<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">将图表添加到报表</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>详细信息</td> 
   <td>这是保存报告后报告的选项卡之一。 它显示报告的调查结果，显示在您选择的视图和分组中。</td> 
  </tr> 
  <tr> 
   <td>表达式</td> 
   <td>表达式是文本模式中的一种书面公式，用于传达使用文本模式界面时要搜索或显示的信息。 它通常是较大的Text Mode语句中的一行。</td> 
  </tr> 
  <tr> 
   <td>字段</td> 
   <td> <p>指对象的属性。 例如，“状态”是项目、任务或问题的字段。 “Portfolio管理器”是Portfolio对象的字段。</p> <p>您还可以具有您自己创建并添加到自定义表单中的自定义字段。<br>有关创建自定义表单的信息，请参阅文章<a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">创建自定义表单</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>字段名称 </td> 
   <td>在视图中显示、在筛选条件中使用或作为分组公用元素的属性的值。 字段名称的选项取决于字段Source选择。</td> 
  </tr> 
  <tr> 
   <td>字段源 </td> 
   <td>在视图中显示的对象、在筛选条件中使用的对象值或作为分组的公共元素使用的对象值。 字段Source中的选项取决于所创建UI元素的对象类型。 字段Source允许您引用UI元素的对象类型以外的对象属性。</td> 
  </tr> 
  <tr> 
   <td>筛选条件</td> 
   <td>确定在报表中显示哪些结果的主要报表元素。</td> 
  </tr> 
  <tr> 
   <td>表单 </td> 
   <td>可与“自定义表单”互换使用。 字段和部分会添加到表单中，然后这些字段和部分会附加到对象中，以增加可与对象关联的字段数。</td> 
  </tr> 
  <tr> 
   <td>分组 </td> 
   <td>标识结果列表的组织方式的主要报表元素。 分组会在整个报表中创建水平条，以按创建结果时定义的公共属性对结果进行分组。 在矩阵报表中使用分组来聚合数据，在图表中使用分组来确定图表的轴。</td> 
  </tr> 
  <tr> 
   <td>对象或对象类型</td> 
   <td> 对象是一个Workfront应用程序元素（例如，项目、任务、组、公司、筛选器）。 创建新报告、视图、过滤器或分组时，会使用对象类型来标识哪个对象是报告的焦点。 报告只能有一个对象类型，它是报告的主对象。<br>可以在同一报表中引用父对象。<br>有关对象层次结构的详细信息，请参阅<a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Adobe Workfront对象概述</a>一文中的“了解对象的相互依赖性和层次结构”一节。</td> 
  </tr> 
  <tr> 
   <td>提示</td> 
   <td> <p>可在每次运行报表需要使用其他过滤器时添加到报表的可选报表元素。</p> <p>有关提示的信息，请参阅<a href="/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">向报表添加提示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>限定词或条件修饰符</td> 
   <td> <p>此字段显示在报告的以下区域中：</p> 
    <ul> 
     <li>在“筛选器”选项卡上</li> 
     <li>列（视图）选项卡中列的“高级选项”屏幕。 通过定义限定词，您可以将“字段名”与另一个字段或值进行比较。</li> 
     <li> 在自定义提示中<br><p>有关提示的信息，请参阅<a href="/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md" class="MCXref xref">向报表添加提示</a>。</p>。</li> 
    </ul> <p>例如，在为计划完成日期为今天的任务构建过滤器时，您可以在“限定符”字段中选择<strong>等于</strong>，在“日期”字段中选择今天的日期：</p> <p><em>任务&gt;计划完成日期&gt;等于&gt;（今天的日期）</em> </p> <p>在此方案中，限定符为<strong>等于</strong>。<br>有关限定符的详细信息，请参阅文章<a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">筛选器和条件修饰符</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>报告 </td> 
   <td>视图、筛选器和（有时）分组的组合。 报告的目的是跨界面显示一致的数据，分发信息，并消除定期运行相同搜索或查询的需要。</td> 
  </tr> 
  <tr> 
   <td>语句</td> 
   <td>由多个表达式组成，这些表达式组合在一起，用于定义在使用文本模式时报表中显示的信息。 可以为报表中的视图、筛选器、分组或自定义提示创建语句。</td> 
  </tr> 
  <tr> 
   <td>摘要</td> 
   <td>这是保存报告后报告的选项卡之一。 仅当您为报告定义分组时，才会创建此选项卡。 它根据报告创建期间定义的分组汇总信息，并提供报告聚合对象的快速概览。 它不会显示报表中的每个对象，只会显示汇总的对象。</td> 
  </tr> 
  <tr> 
   <td>文本模式界面</td> 
   <td>提供创建或修改最初通过生成器界面创建的自定义视图、筛选器、分组和提示的代码的功能。 建议最初通过生成器界面创建报告元素，然后在保存后将其转换为文本模式，以简化高级视图、筛选器、分组或提示的编码。</td> 
  </tr> 
  <tr> 
   <td>用户界面(UI)</td> 
   <td>是指在任何给定时间显示在用户屏幕上的内容的组件或构建块。</td> 
  </tr> 
  <tr> 
   <td>视图（或列）</td> 
   <td>报告的主要内容之一。 它标识将在报告列表中显示的列标题。</td> 
  </tr> 
 </tbody> 
</table>
