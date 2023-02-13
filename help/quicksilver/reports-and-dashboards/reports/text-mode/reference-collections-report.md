---
product-area: reporting
navigation-topic: text-mode-reporting
title: 在报表中引用集合
description: 在报表中引用集合
author: Nolan
feature: Reports and Dashboards
exl-id: 18ba3f4b-ae03-4694-a2fe-fdbeeb576ea9
source-git-commit: 8b6324302a70319f387d1e09d1eb92fbdabf7e32
workflow-type: tm+mt
source-wordcount: '2609'
ht-degree: 0%

---

# 在报表中引用集合

在Adobe Workfront中构建报表允许您在列表、网格或图表格式中显示一组对象、其各自的字段或链接对象。

有关在Workfront中构建报表的更多信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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
   <td> <p>编辑对过滤器、视图、分组的访问权限</p> <p>编辑对报表、功能板、日历的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>管理视图、过滤器或分组的权限 </p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 了解集合

集合是链接到另一个对象的对象列表。

在Workfront中的对象之间具有以下两个关系：

* **一对一关系**:一个对象一次只能链接到另一个对象。\
   例如，一个项目一次只能链接到一个项目组合。

* **一对多关系**:一个对象一次可以链接到多个其他对象。\
   例如，一个项目可以有多个任务。 在这种情况下，任务列表将构成项目的集合。

>[!IMPORTANT]
>
>您可以使用标准报表生成器构建一个报表，其中显示对象之间的一对一关系。 但是，您只能使用报表生成器中的文本模式界面来构建显示对象之间一对多关系的报表。

有关在标准报表生成器中构建报表的更多信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

有关使用文本模式界面构建报表的更多信息，请参阅：

* [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [文本模式常见用法概述](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
* [文本模式语法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)

## 在API资源管理器中查找集合对象及其字段 {#find-collection-objects-and-their-fields-in-the-api-explorer}

并非所有收藏集都可报告。

要了解哪些对象可以与其他对象集合关联，您必须使用API资源管理器。\
有关API资源管理器表的更多信息，请参阅 [API Explorer](../../../wf-api/general/api-explorer.md).

要了解可报告哪些收藏集，请执行以下操作：

1. 转到 [API Explorer](../../../wf-api/general/api-explorer.md).
1. 查找报表的对象。
1. 选择 **收藏集** 选项卡。

   >[!NOTE]
   >
   >只有此选项卡上列出的对象才能在所选对象的报表中显示为集合。

1. 通过单击展开集合的对象。
1. 单击显示的链接可转到集合的对象。\
   这将打开 **字段** 选项卡。

   >[!NOTE]
   >
   >只能在收藏集报表中引用此选项卡上列出的字段，或者只能在与此选项卡中列出的对象关联的字段中引用。

## 在报表中引用集合

您可以在以下报表元素中引用集合中的对象：

* 视图
* 过滤器
* 提示

不能引用以下报表元素中集合中的对象：

* 分组
* 图表

例如，您可以从项目报表中引用任务或发出集合，以在项目级别显示任务或发出信息。

* [在报表视图中引用收藏集](#reference-a-collection-in-the-view-of-a-report)
* [在报表过滤器中引用集合](#reference-a-collection-in-the-filter-of-a-report)
* [在报表的自定义提示中引用集合](#reference-a-collection-in-the-custom-prompt-of-a-report)

### 在报表视图中引用收藏集 {#reference-a-collection-in-the-view-of-a-report}

可以在报表视图中引用对象集合，以显示与报表对象关联的对象的属性。

例如，您可以在项目报表中显示任务或问题信息，方法是在报表视图中为任务或问题构建收集列。

您可以在收集视图中显示有关任务或问题的信息，如名称、日期、主要受分配者、完成百分比等。

视图以列表格式显示任务或问题信息，列表的每一行都表示有关任务或问题的信息。 任务或问题列表及其字段显示在与任务或问题所属的项目相同的一行上。\
![issue_and_tasks_collections_in_reports.png](assets/issue-and-tasks-collections-in-reports-350x171.png)

* [在报表视图中添加收藏集列](#add-a-collection-column-in-a-report-view)
* [了解文本模式下收藏集视图的行](#understand-the-lines-of-a-collection-view-in-text-mode)
* [收藏集视图的限制](#limitations-of-a-collection-view)

### 在报表视图中添加收藏集列 {#add-a-collection-column-in-a-report-view}

要在报表视图中添加收藏集列，请执行以下操作：

1. 单击 **主要** 菜单 ![](assets/main-menu-icon.png)，然后单击 **报表**.
1. 单击 **新建报表**.
1. 选择报表的对象。
1. 从报表中导航离开，并使用 [API Explorer](../../../wf-api/general/api-explorer.md)，确定为报表选择的对象可用的集合。

   有关选择集合对象的更多信息，请参阅部分 [在API资源管理器中查找集合对象及其字段](#find-collection-objects-and-their-fields-in-the-api-explorer) 在本文中。\
   记下集合对象的名称。

1. 使用 [API Explorer](../../../wf-api/general/api-explorer.md)，转到要在集合中显示的对象的字段列表。

   有关查找集合对象字段的更多信息，请参阅部分 [在API资源管理器中查找集合对象及其字段](#find-collection-objects-and-their-fields-in-the-api-explorer) 在本文中。

   记下要在集合中显示的字段名称。

1. 导航回报表，然后在 **列（视图）** ，单击 **添加列**.
1. 单击 **切换到文本模式**.
1. 将鼠标悬停在对话框上，然后单击 **单击以编辑文本**.
1. 选择 **文本模式** 对话框，并将其删除，如果您引用集合对象的字段，请粘贴以下代码：

   ```
   valueformat=HTML
   textmode=true
   type=iterate
   listdelimiter=<p>
   displayname=Column Name
   listmethod=nested(collection object name).lists
   valuefield=collection object field
   ```

1. 替换 **列名称** ，并在 `displayname` 行。
1. 替换 **集合对象名称**，并在 `listmethod` 行，如 [API Explorer](../../../wf-api/general/api-explorer.md).

1. 替换 **集合对象字段** ，其名称为 `valuefield` 行，如 [API Explorer](../../../wf-api/general/api-explorer.md).

   您可以将 **valuefield** with **valueexpression**，以便在视图中创建自定义表达式。

   有关计算自定义表达式的更多信息，请参阅 [计算数据表达式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   例如，要在项目报表中显示任务列表。 此集合使用 `valuefield` 行，以引用任务的名称。

   执行下列操作之一：

   * 使用以下代码构建列：

      ```
      valueformat=HTML
      textmode=true
      type=iterate
      listdelimiter=<p>
      displayname=Project Tasks Names
      listmethod=nested(tasks).lists
      valuefield=name
      ```

   * 使用以下代码显示报表中的问题列表：

      ```
      displayname=Project Issues Names
      listdelimiter=<p>
      listmethod=nested(issues).lists
      textmode=true
      type=iterate
      valuefield=name
      valueformat=HTML
      ```

      请注意，在集合中，您必须使用 **问题** 对于 **listmethod** 行，而不是 **opTasks** 这是“问题”的数据库名称。 有关何时使用的信息 **问题** 以及何时使用 **opTask** 在提及问题时，请参阅 [引用问题时，请使用“opTask”和“issue”](../../../manage-work/issues/issue-information/use-optask-instead-of-issue.md).

   * 如果要在项目报表中显示任务列表及其主要代理人，则应使用 **valueexpression** 用于引用任务名称的行，位于其主要任务的名称旁边，而不是 **valuefield**.

      使用以下代码构建列：

      ```
      valueformat=HTML
      textmode=true
      type=iterate
      listdelimiter=<p>
      displayname=Tasks Names - Primary Assignee
      listmethod=nested(tasks).lists
      valueexpression=CONCAT({name},' - ',{assignedTo}.{name})
      ```

1. 以下列显示在项目报表中，列出了每个项目中的所有任务及其主要任务分配者：

   ![](assets/project-report-with-task-and-assignee-collection-view-nwe-350x222.png)

1. 单击&#x200B;**保存**。
1. （可选）继续编辑报表。

   或

   单击 **保存并关闭** 以保存报表。

#### 了解文本模式下收藏集视图的行

下表列出了集合的文本模式视图中的各行：

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
   <td> <p>您可以对此行使用各种值，但我们建议 <code style="font-weight: normal;">valueformat</code> ，则 <strong>HTML。</strong></p>
   </td> 
  </tr> 
  <tr> 
   <td><code>textmode=true</code> </td> 
   <td> <p>此行表示该列已使用文本模式进行配置。 如果删除此行，Workfront会默认将其添加回来。</p> </td> 
  </tr> 
  <tr> 
   <td><code>type=iterate</code> </td> 
   <td> <p>的 <code>type</code> 总是 <code>iterate</code>，构建视图时。</p> </td> 
  </tr> 
  <tr> 
   <td><code>listdelimiter=&lt;p&gt;</code> </td> 
   <td> <p>这是用于分隔列表中值的分隔符。<br>我们建议使用 <code>&lt;p&gt;</code> 在值之间添加换行符。</p> <p>您还可以使用以下代码：</p> <p><code>&amp;zwj;</code> （零宽度连接符）。 集合的值之间没有分隔。<br><strong>,</strong> =逗号分隔符。 集合的值以逗号分隔，后跟无空格。<br><strong>/</strong> =斜杠分隔符。 集合的值以斜杠分隔。<br><strong>-</strong> =短划线分隔符。 集合的值用短划线分隔。<br>默认情况下，将此行留空会在集合值之间添加一个逗号，后跟一个空格。</p> </td> 
  </tr> 
  <tr> 
   <td><code>displayname=</code><em>列名称</em> </td> 
   <td> <p>替换 <strong>列名称</strong> 以及新列的实际名称。</p> </td> 
  </tr> 
  <tr> 
   <td><code>listmethod=nested(collection object name).list</code> </td> 
   <td> <p> 此行定义您引用的集合。</p> <p>替换 <strong>集合对象名称</strong> ，且其名称中包含您在集合中引用的对象，如 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. 此值通常为集合对象名称的复数形式。</p> </td> 
  </tr> 
  <tr> 
   <td><code>valuefield=collection object field</code> </td> 
   <td> <p>此行定义您要从集合对象中引用的字段。</p> <p>替换 <strong>集合对象字段</strong> ，且其名称为您在集合中引用的对象的字段，如 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>您可以将此行替换为：</p> <p><strong>valueexpression</strong>=计算的集合对象字段/字段</p> <p>使用 <strong>valueexpression</strong>，则可以在列中显示计算的自定义表达式。</p> <p>有关如何设置格式的更多信息 <strong>valueexpression</strong> 行，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">文本模式语法概述</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 收藏集视图的限制 {#limitations-of-a-collection-view}

在构建收藏集视图时，请考虑以下限制：

* 您无法控制收集数据的显示顺序。
* 不能对收藏集视图应用条件格式。
* 不能将集合中的对象设为可单击链接。
* 您无法构建其他收藏集的收藏集视图。\
   例如，您无法在项目报表中显示每个任务的所有受分配者。 您只能在项目视图中显示每项任务的主要代理人。

### 在报表过滤器中引用集合 {#reference-a-collection-in-the-filter-of-a-report}

您可以在报表的过滤器中引用对象集合，以过滤与报表对象关联的对象的属性。

例如，您可以在项目报表中过滤任务或问题信息，方法是引用筛选器语句中项目任务或问题的属性。

要在报表过滤器中添加对收藏集的引用，请执行以下操作：

1. 单击 **主要** 菜单 ![](assets/main-menu-icon.png)，然后单击 **报表**.
1. 单击 **新建报表**.
1. 选择报表的对象。
1. 从报表中导航离开，并使用 [API Explorer](../../../wf-api/general/api-explorer.md)，确定为报表选择的对象可用的集合。

   有关选择集合对象的更多信息，请参阅部分 [在API资源管理器中查找集合对象及其字段](#find-collection-objects-and-their-fields-in-the-api-explorer) 在本文中。

   记下集合对象的名称。

1. 使用 [API Explorer](../../../wf-api/general/api-explorer.md)，转到要在集合中显示的对象的字段列表。

   有关查找集合对象字段的更多信息，请参阅部分 [在API资源管理器中查找集合对象及其字段](#find-collection-objects-and-their-fields-in-the-api-explorer) 在本文中。

   记下要在收藏集中显示的字段。

1. 导航回报表，然后在 **过滤器** ，单击 **切换到文本模式**.

1. 在 **为报表设置过滤器规则** ，请粘贴以下代码：

   ```
   collection object name:collection object field=collection object value
   collection object name:collection object field_Mod=value of the modifier
   ```

1. 替换 **集合对象名称** ，其名称为 [API Explorer](../../../wf-api/general/api-explorer.md). 此值通常为集合对象名称的复数形式。

1. 替换 **集合对象字段** ，其中包含集合对象的字段名称，如 [API Explorer](../../../wf-api/general/api-explorer.md).

1. 替换 **集合对象值** ，其值为集合对象在Workfront中显示的值。
1. 替换 **修饰符的值** 的值。

   有关修饰符列表，请参阅 [过滤器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).\
   例如，要构建仅显示其名称中包含“营销”任务的项目报表，请使用以下代码：

   ```
   tasks:name=Marketing
   tasks:name_Mod=cicontains
   ```

   此报表仅显示至少包含一个名称中带有“营销”字样的任务的项目。

   ![](assets/marketing-only-tasks-in-project-report-nwe-350x309.png)

1. 要筛选问题的名称，请使用以下代码：

   ```
   issues:name=Marketing
   issues:name_Mod=cicontains
   ```

   >[!TIP]
   >
   >请注意，您必须使用 `issues` ，而不是 `optask` 这就是API资源管理器中出现问题的方式。

1. 单击 **完成**.
1. （可选）继续编辑报表。

   或

   单击 **保存并关闭** 以保存报表。

### 在报表的自定义提示中引用集合 {#reference-a-collection-in-the-custom-prompt-of-a-report}

可以在报表的自定义提示中引用对象集合，以过滤报表结果中与报表对象关联的对象的属性。

例如，您可以在项目报表中使用对项目任务属性的引用来提示输入任务信息，该引用位于报表的自定义提示符中。

>[!NOTE]
>
>不能在标准提示中引用集合。

自定义提示是自定义筛选器，其中语句使用与号联接。 我们建议您先在过滤器中构建语句，然后使用与号连接语句的行。

有关使用集合引用构建filter语句的更多信息，请参阅部分 [在报表过滤器中引用集合](#reference-a-collection-in-the-filter-of-a-report) 在本文中。

要在报表的自定义提示中添加对集合的引用，请执行以下操作：

1. 单击 **主要** 菜单 ![](assets/main-menu-icon.png)，然后单击 **报表**.
1. 单击 **新建报表**.
1. 选择报表的对象。
1. 使用集合引用构建过滤器，如部分中所述 [在报表过滤器中引用集合](#reference-a-collection-in-the-filter-of-a-report) 在本文中。
1. 单击 **报表设置**.
1. 单击 **报表提示**.
1. 单击 **添加提示**.
1. 单击 **自定义提示**.
1. 在 **字段****名称** 字段。

1. 指定 **下拉项目标签**.
1. 在 **条件** 字段：

   ```
   collection object name:collection object field_Mod=value of the modifier
   ```

1. （可选）指定提示中默认显示此选项。
1. 替换 **集合对象名称** ，其名称为 [API Explorer](../../../wf-api/general/api-explorer.md). 此值通常为集合对象名称的复数形式。
1. 替换 **集合对象字段** ，其名称为集合对象的字段名称，如 [API Explorer](../../../wf-api/general/api-explorer.md).
1. 替换 **集合对象值** ，其值为集合对象在Workfront中显示的值。

   例如，如果要筛选任务名称包含“营销”的项目，请将 **集合对象值** with **营销**.

1. 替换 **修饰符的值** 的值。

   有关修饰符列表，请参阅  [过滤器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   **示例：** 例如，要在自定义提示下构建项目报表，以便您仅显示至少为特定用户分配了一项任务的项目，请使用以下代码：

   ```
   tasks:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&tasks:assignedToID_Mod=in
   ```

   这会生成一个报告，其中列出的所有项目都至少为GUID为57cf1b7a000077c9f02f66cb09c8f86c的用户分配了一个任务。

   >[!NOTE]
   >
   >根据 [API Explorer](../../../wf-api/general/api-explorer.md). 您只能引用主代理人的ID。

   例如，要筛选将任何项目问题分配给特定用户的任何项目，请为自定义提示使用以下代码：

   ```
   issues:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&issues:assignedToID_Mod=in
   ```

   这会生成一个报告，其中列出的所有项目都至少为GUID为57cf1b7a000077c9f02f66cb09c8f86c的用户分配了一个问题。

   >[!NOTE]
   请注意，您必须使用 **问题** ，用于集合对象名称。 目前，API资源管理器没有为问题提供集合对象名称。

1. 单击 **完成**.
1. （可选）继续编辑报表。

   或

   单击 **保存并关闭** 以保存报表。
