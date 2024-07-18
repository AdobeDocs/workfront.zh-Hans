---
product-area: reporting
navigation-topic: text-mode-reporting
title: 在报表中引用收藏集
description: 在报表中引用收藏集
author: Nolan
feature: Reports and Dashboards
exl-id: 18ba3f4b-ae03-4694-a2fe-fdbeeb576ea9
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '2598'
ht-degree: 0%

---

# 在报表中引用收藏集

在Adobe Workfront中构建报表允许您以列表、网格或图表格式显示一组对象、其各自的字段或链接对象。

有关在Workfront中生成报告的详细信息，请参阅[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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
   <td> <p>编辑对筛选器、视图、分组的访问权限</p> <p>编辑对报告、功能板和日历的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>管理对视图、筛选器或分组的权限 </p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

+++

## 了解收藏集

集合是链接到其他对象的对象列表。

Workfront中的对象之间存在以下两个关系：

* **一对一关系**：一个对象一次只能链接到另一个对象。\
  例如，一个项目一次只能链接到一个项目组合。

* **一对多关系**：一个对象一次可以链接到多个其他对象。\
  例如，一个项目可以有多个任务。 在这种情况下，任务列表将构成项目的集合。

>[!IMPORTANT]
>
>您可以使用标准Report Builder构建显示对象之间一对一关系的报表。 但是，您只能通过使用Report Builder中的文本模式界面来构建显示对象之间一对多关系的报表。

有关在标准Report Builder中生成报表的更多信息，请参阅[创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

有关使用文本模式界面构建报表的更多信息，请参阅：

* [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [文本模式的常见使用概述](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)。
* [文本模式语法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)

## 在API Explorer中查找收藏集对象及其字段 {#find-collection-objects-and-their-fields-in-the-api-explorer}

并非所有收藏集都可以报告。

要了解哪些对象可以与其他对象的集合相关联，您必须使用API Explorer。\
有关API Explorer表的详细信息，请参阅[API Explorer](../../../wf-api/general/api-explorer.md)。

要了解可报告哪些收藏集，请执行以下操作：

1. 转到[API资源管理器](../../../wf-api/general/api-explorer.md)。
1. 查找报告的对象。
1. 选择&#x200B;**收藏集**&#x200B;选项卡。

   >[!NOTE]
   >
   >只有此选项卡上列出的对象才能在选定对象的报表中表示为集合。

1. 单击收藏集的对象以将其展开。
1. 单击显示的链接可转至收藏集的对象。\
   这将打开集合对象的&#x200B;**字段**&#x200B;选项卡。

   >[!NOTE]
   >
   >只有此选项卡上列出的字段才能在集合报表中引用，或者只能引用与此选项卡上列出的对象关联的字段。

## 报表中的引用收藏集

您可以在以下报表元素中引用收藏集中的对象：

* 视图
* 过滤器
* 提示

在以下报表元素中，不能引用收藏集中的对象：

* 分组
* 图表

例如，您可以从项目报告中引用任务或问题集合，以在项目级别显示任务或问题信息。

* [引用报表视图中的收藏集](#reference-a-collection-in-the-view-of-a-report)
* [引用报告筛选器中的集合](#reference-a-collection-in-the-filter-of-a-report)
* [在报表的自定义提示中引用集合](#reference-a-collection-in-the-custom-prompt-of-a-report)

### 在报表视图中引用收藏集 {#reference-a-collection-in-the-view-of-a-report}

您可以在报表视图中引用对象集合，以显示与报表对象关联的对象的属性。

例如，通过在报告视图中构建任务或问题的收集列，您可以在项目报告中显示任务或问题信息。

您可以在收藏集视图中显示有关任务或问题的信息，如名称、日期、主要分派人、完成百分比等。

该视图以列表格式显示任务或问题信息，列表的每一行表示有关任务或问题的信息。 任务或问题及其字段的列表显示在任务或问题所属项目的同一行上。\
![issue_and_tasks_collections_in_reports.png](assets/issue-and-tasks-collections-in-reports-350x171.png)

* [在报表视图中添加收藏集列](#add-a-collection-column-in-a-report-view)
* [在文本模式下了解收藏集视图的行](#understand-the-lines-of-a-collection-view-in-text-mode)
* [收藏集视图的限制](#limitations-of-a-collection-view)

### 在报表视图中添加收藏集列 {#add-a-collection-column-in-a-report-view}

要在报表视图中添加收藏集列，请执行以下操作：

1. 单击&#x200B;**主**&#x200B;菜单![](assets/main-menu-icon.png)，然后单击&#x200B;**报表**。
1. 单击&#x200B;**新建报告**。
1. 选择报表的对象。
1. 从报表中导航出来，使用[API Explorer](../../../wf-api/general/api-explorer.md)确定您为报表选择的对象有哪些收藏集可用。

   有关选择集合对象的更多信息，请参阅本文中的[在API资源管理器](#find-collection-objects-and-their-fields-in-the-api-explorer)中查找集合对象及其字段部分。\
   记下集合对象的名称。

1. 使用[API Explorer](../../../wf-api/general/api-explorer.md)，转到要显示在集合中的对象的字段列表。

   有关查找集合对象的字段的更多信息，请参阅本文中的[在API资源管理器中查找集合对象及其字段](#find-collection-objects-and-their-fields-in-the-api-explorer)部分。

   记下要在集合中显示的字段名称。

1. 导航回您的报告，在&#x200B;**列（视图）**&#x200B;选项卡中，单击&#x200B;**添加列**。
1. 单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在该对话框上，然后单击&#x200B;**单击以编辑文本**。
1. 在&#x200B;**文本模式**&#x200B;对话框中选择所有文本并将其删除，然后粘贴以下代码（如果您正在引用集合对象的字段）：

   ```
   valueformat=HTML
   textmode=true
   type=iterate
   listdelimiter=<p>
   displayname=Column Name
   listmethod=nested(collection object name).lists
   valuefield=collection object field
   ```

1. 将&#x200B;**Column Name**&#x200B;替换为`displayname`行中的列名。
1. 将&#x200B;**集合对象名称**&#x200B;替换为[API资源管理器](../../../wf-api/general/api-explorer.md)中显示的集合对象名称（位于`listmethod`行）。

1. 将&#x200B;**集合对象字段**&#x200B;替换为[API资源管理器](../../../wf-api/general/api-explorer.md)中显示的集合对象在`valuefield`行中的字段名称。

   如果要在视图中创建自定义表达式，可以使用&#x200B;**valueexpression**&#x200B;替换&#x200B;**valuefield**。

   有关计算自定义表达式的详细信息，请参阅[计算数据表达式的概述](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

   例如，如果要在项目报告中显示任务列表。 此集合使用`valuefield`行引用任务的名称。

   执行下列操作之一：

   * 使用以下代码构建您的列：

     ```
     valueformat=HTML
     textmode=true
     type=iterate
     listdelimiter=<p>
     displayname=Project Tasks Names
     listmethod=nested(tasks).lists
     valuefield=name
     ```

   * 使用以下代码可显示报告中的问题列表：

     ```
     displayname=Project Issues Names
     listdelimiter=<p>
     listmethod=nested(issues).lists
     textmode=true
     type=iterate
     valuefield=name
     valueformat=HTML
     ```

     请注意，在集合中，您必须对&#x200B;**listmethod**&#x200B;行使用&#x200B;**问题**，而不是使用&#x200B;**opTasks**（问题的数据库名称）。 有关何时使用&#x200B;**问题**&#x200B;以及何时在引用问题时使用&#x200B;**opTask**&#x200B;的信息，请参阅在引用问题时[使用“opTask”和“issue”](../../../manage-work/issues/issue-information/use-optask-instead-of-issue.md)。

   * 如果要显示项目报告中任务的列表以及任务的主要被分配人，可使用&#x200B;**valueexpression**&#x200B;行引用与其主要被分配人名称相邻的任务名称，而不是&#x200B;**valuefield**。

     使用以下代码构建您的列：

     ```
     valueformat=HTML
     textmode=true
     type=iterate
     listdelimiter=<p>
     displayname=Tasks Names - Primary Assignee
     listmethod=nested(tasks).lists
     valueexpression=CONCAT({name},' - ',{assignedTo}.{name})
     ```

1. 项目报表中显示以下列，列出每个项目中的所有任务及其主要受分配人：

   ![](assets/project-report-with-task-and-assignee-collection-view-nwe-350x222.png)

1. 单击&#x200B;**保存**。
1. （可选）继续编辑报表。

   或

   单击&#x200B;**保存+关闭**&#x200B;以保存报告。

#### 在文本模式下了解收藏集视图的行

下表概述了集合的文本模式视图中的行：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>示例行</strong> </th> 
   <th><strong>描述</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>valueformat=HTML</code> </td> 
   <td> <p>您可以对此行使用各种值，但我们建议集合列表的<code style="font-weight: normal;">valueformat</code>HTML应为<strong>。</strong></p>
   </td> 
  </tr> 
  <tr> 
   <td><code>textmode=true</code> </td> 
   <td> <p>此行表示该列已使用文本模式进行配置。 如果删除此行，Workfront会默认将其添加回来。</p> </td> 
  </tr> 
  <tr> 
   <td><code>type=iterate</code> </td> 
   <td> <p>生成视图时，列表的<code>type</code>始终为<code>iterate</code>。</p> </td> 
  </tr> 
  <tr> 
   <td><code>listdelimiter=&lt;p&gt;</code> </td> 
   <td> <p>这是用于分隔列表中各个值的分隔符。<br>我们建议使用<code>&lt;p&gt;</code>，它在值之间添加换行符。</p> <p>您还可以使用以下命令：</p> <p><code>&amp;zwj;</code> （零宽度连接符）。 集合的值之间没有分隔符。<br><strong>，</strong> =逗号分隔符。 收藏集的值由逗号分隔，后跟空格。<br><strong>/</strong> =斜杠分隔符。 集合的值用斜杠分隔。<br><strong>-</strong> =短划线分隔符。 集合的值用短划线分隔。<br>默认情况下，将此行留空将在集合的值之间添加一个逗号，后跟一个空格。</p> </td> 
  </tr> 
  <tr> 
   <td><code>displayname=</code><em>列名称</em> </td> 
   <td> <p>将<strong>列名称</strong>替换为您的新列的实际名称。</p> </td> 
  </tr> 
  <tr> 
   <td><code>listmethod=nested(collection object name).list</code> </td> 
   <td> <p> 该行定义您正在引用的收藏集。</p> <p>将<strong>收藏集对象名称</strong>替换为您在收藏集中引用的对象的名称，该名称显示在<a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>中。 此值通常是集合对象名称的多种形式。</p> </td> 
  </tr> 
  <tr> 
   <td><code>valuefield=collection object field</code> </td> 
   <td> <p>该行定义您从集合对象中引用哪个字段。</p> <p>将<strong>收藏集对象字段</strong>替换为您在收藏集中引用的对象的字段名称，因为该字段显示在<a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>中。</p> <p>您可以将此行替换为：</p> <p><strong>valueexpression</strong>=计算的集合对象字段/字段</p> <p>使用<strong>valueexpression</strong>，您可以  在列中显示计算的自定义表达式。</p> <p>有关如何设置<strong>valueexpression</strong>行的格式的详细信息，请参阅<a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">文本模式语法概述</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 收藏集视图的限制 {#limitations-of-a-collection-view}

构建收藏集视图时，请考虑以下限制：

* 您无法控制集合数据的显示顺序。
* 不能对收藏集视图应用条件格式。
* 不能将收藏集中的对象设为可单击的链接。
* 您无法生成其他收藏集的收藏集视图。\
  例如，您不能在项目报告中显示每项任务的所有被分配人。 您只能在项目视图中的每个任务上显示主要被分配人。

### 在报表的过滤器中引用集合 {#reference-a-collection-in-the-filter-of-a-report}

您可以引用报表过滤器中的对象集合，以过滤与报表对象关联的对象的属性。

例如，可通过在过滤器语句中使用对项目上任务或问题属性的引用，来过滤项目报告中的任务或问题信息。

要在报表过滤器中添加对收藏集的引用，请执行以下操作：

1. 单击&#x200B;**主**&#x200B;菜单![](assets/main-menu-icon.png)，然后单击&#x200B;**报表**。
1. 单击&#x200B;**新建报告**。
1. 选择报表的对象。
1. 从报表中导航出来，使用[API Explorer](../../../wf-api/general/api-explorer.md)确定您为报表选择的对象有哪些收藏集可用。

   有关选择集合对象的更多信息，请参阅本文中的[在API资源管理器](#find-collection-objects-and-their-fields-in-the-api-explorer)中查找集合对象及其字段部分。

   记下集合对象的名称。

1. 使用[API Explorer](../../../wf-api/general/api-explorer.md)，转到要显示在集合中的对象的字段列表。

   有关查找集合对象的字段的更多信息，请参阅本文中的[在API资源管理器中查找集合对象及其字段](#find-collection-objects-and-their-fields-in-the-api-explorer)部分。

   记下要在收藏集中显示的字段。

1. 导航回您的报告，在&#x200B;**筛选器**&#x200B;选项卡中，单击&#x200B;**切换到文本模式**。

1. 在&#x200B;**为报表**&#x200B;设置筛选规则区域中，粘贴以下代码：

   ```
   collection object name:collection object field=collection object value
   collection object name:collection object field_Mod=value of the modifier
   ```

1. 将&#x200B;**收藏集对象名称**&#x200B;替换为您在[API资源管理器](../../../wf-api/general/api-explorer.md)中显示的收藏集对象名称。 此值通常是集合对象名称的多种形式。

1. 将&#x200B;**收藏集对象字段**&#x200B;替换为您的收藏集对象在[API Explorer](../../../wf-api/general/api-explorer.md)中显示的字段名称。

1. 将&#x200B;**集合对象值**&#x200B;替换为该集合对象在Workfront中显示的值。
1. 用有效的修饰符替换修饰符&#x200B;**的**&#x200B;值。

   有关修饰符列表，请参阅[筛选器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。\
   例如，要生成一个项目报告，其中仅显示名称中包含“营销”任务的项目，请使用以下代码：

   ```
   tasks:name=Marketing
   tasks:name_Mod=cicontains
   ```

   此报表仅显示至少有一个任务名称包含“营销”字样的项目。

   ![](assets/marketing-only-tasks-in-project-report-nwe-350x309.png)

1. 要筛选问题的名称，请使用以下代码：

   ```
   issues:name=Marketing
   issues:name_Mod=cicontains
   ```

   >[!TIP]
   >
   >请注意，您必须使用`issues`作为集合对象名称，而不是使用`optask`，后者是问题在API资源管理器中的显示方式。

1. 单击&#x200B;**完成**。
1. （可选）继续编辑报表。

   或

   单击&#x200B;**保存+关闭**&#x200B;以保存报告。

### 在报表的自定义提示中引用集合 {#reference-a-collection-in-the-custom-prompt-of-a-report}

您可以在报表的自定义提示中引用对象集合，以过滤报表结果，找出与报表对象关联的对象属性。

例如，可通过在项目的自定义提示中使用对项目上任务属性的引用，来提示项目报告中的任务信息。

>[!NOTE]
>
>不能在标准提示中引用收藏集。

自定义提示是一种自定义过滤器，其中语句由&amp;符号连接。 我们建议您在筛选器中构建语句，首先使用&amp;符号连接语句行。

有关使用集合引用构建过滤器语句的更多信息，请参阅本文中的[引用报表过滤器中的集合](#reference-a-collection-in-the-filter-of-a-report)部分。

要在报表的自定义提示中添加对收藏集的引用，请执行以下操作：

1. 单击&#x200B;**主**&#x200B;菜单![](assets/main-menu-icon.png)，然后单击&#x200B;**报表**。
1. 单击&#x200B;**新建报告**。
1. 选择报表的对象。
1. 使用集合引用生成筛选器，如本文中报表](#reference-a-collection-in-the-filter-of-a-report)的筛选器中的[引用集合部分所述。
1. 单击&#x200B;**报表设置**。
1. 单击&#x200B;**报告提示**。
1. 单击&#x200B;**添加提示**。
1. 单击&#x200B;**自定义提示**。
1. 在&#x200B;**字段{name****1}字段中指定提示的名称。**

1. 指定&#x200B;**下拉项目标签**。
1. 在&#x200B;**条件**&#x200B;字段中指定以下内容：

   ```
   collection object name:collection object field_Mod=value of the modifier
   ```

1. （可选）指定是否默认在提示中显示此选项。
1. 将&#x200B;**收藏集对象名称**&#x200B;替换为您在[API资源管理器](../../../wf-api/general/api-explorer.md)中显示的收藏集对象名称。 此值通常是集合对象名称的多种形式。
1. 将&#x200B;**收藏集对象字段**&#x200B;替换为收藏集对象字段的名称，该字段显示在[API Explorer](../../../wf-api/general/api-explorer.md)中。
1. 将&#x200B;**集合对象值**&#x200B;替换为该集合对象在Workfront中显示的值。

   例如，如果您正在筛选任务名称包含“营销”的项目，请将&#x200B;**集合对象值**&#x200B;替换为&#x200B;**营销**。

1. 用有效的修饰符替换修饰符&#x200B;**的**&#x200B;值。

   有关修饰符的列表，请参见  [筛选器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

   **示例：**&#x200B;例如，要生成一个带有自定义提示的项目报告，其中您只想显示至少有一个任务分配给特定用户的项目，请使用以下代码：

   ```
   tasks:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&tasks:assignedToID_Mod=in
   ```

   这将生成一个报告，其中列出的所有项目都至少分配了一个任务给GUID为57cf1b7a000077c9f02f66cb09c8f86c的用户。

   >[!NOTE]
   >
   >根据[API Explorer](../../../wf-api/general/api-explorer.md)，您无法引用任务的主要被分配人（“分配给”字段）的名称。 您只能引用主要被分配人的ID。

   例如，要筛选将任何项目问题分配给特定用户的任何项目，请使用以下代码进行自定义提示：

   ```
   issues:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&issues:assignedToID_Mod=in
   ```

   这将生成一个报告，其中列出的所有项目都至少分配了一个问题给GUID为57cf1b7a000077c9f02f66cb09c8f86c的用户。

   >[!NOTE]
   >
   >请注意，您必须使用&#x200B;**问题**&#x200B;作为集合对象名称。 API资源管理器  目前不提供问题的收藏集对象名称。

1. 单击&#x200B;**完成**。
1. （可选）继续编辑报表。

   或

   单击&#x200B;**保存+关闭**&#x200B;以保存报告。
