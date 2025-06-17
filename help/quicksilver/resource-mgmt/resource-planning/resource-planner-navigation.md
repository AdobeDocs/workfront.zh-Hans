---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: 资源规划者导航概述
description: 通过使用Adobe Workfront资源规划者，您可以轻松了解资源的可用性以及完成项目工作所需的计划时间。 然后，您可以管理用户及其工作角色在分配给他们的项目中的分配。
author: Lisa
feature: Resource Management
exl-id: 5a1be723-e3ac-443a-9c09-85e8839fcbef
source-git-commit: af7789f3a4c7443854639fd60bcf0661217b37ae
workflow-type: tm+mt
source-wordcount: '2424'
ht-degree: 2%

---

# 资源规划程序导航概述

<!-- Audited: 5/2025 -->

Adobe Workfront资源规划者帮助您轻松了解资源的可用性以及完成项目工作所需的计划时间。 然后，您可以管理用户及其工作角色在分配到的项目中的分配。

>[!TIP]
>
>您无法在资源规划者中管理团队在分配给他们的任务上的分配。

您必须满足充分使用资源规划者所需的先决条件。 有关资源规划者的详细信息，请参阅[资源规划者概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

![资源规划程序](assets/resource-planner-overview.png)

以下部分概述了资源规划者的所有区域。

## 项目时间线

![时间线日历](assets/calendar-months.png)


使用资源规划者顶部的日历来导航您正在查看的项目的时间表。 默认情况下，时间轴从当月开始。

有关更改在资源规划者中显示的时间线时间范围的更多信息，请参阅本文中的[时间范围选择](#timeframe-selection)部分。

## 时间范围选择  {#timeframe-selection}

![时间范围选择](assets/timeframe-selection.png)

默认情况下，资源规划者从当月开始，一次显示3或4个月的资源信息。 显示的时段数取决于屏幕的宽度。

>[!TIP]
>
>您不能在资源规划程序中一次显示超过4个时间段。

要导航时间轴，请单击后退和前进箭头，以在时间轴上前后移动。 然后，您可以通过单击相应的按钮，从资源计划程序中的以下日期范围选项中进行选择：

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">周</td> 
      <td>按周显示信息。<br>星期数显示在列标题中的日期旁边。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">月</td> 
      <td> 按月显示信息。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">季度</td> 
      <td>按季度显示信息。<br>季度编号显示在列标题中的日期旁边。<br>自定义季度未显示在资源规划者中。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">今天</td> 
      <td>返回到今天的月、周或季度。</td> 
     </tr> 
    </tbody> 
   </table>

## 项目/角色/用户视图选择

![按项目、角色或用户查看](assets/view-by-drop-down.png)

您可以根据您希望信息的显示方式更改资源规划者中的视图。

默认情况下，资源规划者显示在用户视图中。 您可以将视图更改为项目视图或角色视图。 将其更改为其他视图时，您的选择将变成默认视图。

在更改视图时，以下信息也会更改：

* 对象层次结构（资源规划程序行中的信息）。
* 小时分配信息（资源规划者列中的信息）。

  有关根据您选择的视图在资源规划者中显示哪些列的详细信息，请参阅[使用Adobe Workfront资源规划者查看资源可用性和分配](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md)。

要在资源计划程序中显示准确的信息，您必须满足一组先决条件。 有关先决条件的更多信息，请参阅[资源规划者概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md)文章中的在资源规划者中工作的先决条件部分。

要更改资源规划者中的视图，请在查看方式下拉菜单中选择以下视图之一：

* [按项目查看](#view-by-project)
* [按角色查看](#view-by-role)
* [按用户查看](#view-by-user)

### 按项目查看 {#view-by-project}

在资源规划者中选择项目视图时，请考虑以下事项：

* 您可以查看自己有权查看的项目。
* 在首次访问资源规划者时，您可以看到按默认筛选条件筛选的项目。\
  有关详细信息，请参阅资源规划者[&#128279;](../../resource-mgmt/resource-planning/filter-resource-planner.md)中的筛选信息。

* 为了提高性能，您显示或可从“项目视图”中导出的项数会受到限制。\
  有关详细信息，请参阅[资源规划者显示限制](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)文章中“项目视图”部分的限制。

* 项目按其在项目视图中的优先级顺序列出。\
  有关详细信息，请参阅本文中的[项目计划优先级](#project-planning-priority)部分。

* 展开每个项目时，您可以显示与其关联的工作角色。

* 展开每个角色时，可以显示与其关联的用户。 滚动以在每个项目下加载更多角色和用户。

* 应用此视图后，角色小时数、FTE或成本将合计到项目小时数、FTE或成本。

* 您可以在“项目”视图中查看以下小时、FTE或成本信息：

   * 可用
   * 计划
   * 已预算
   * 变量
   * 净值

     有关详细信息，请参阅使用项目和角色视图的资源规划者中的[预算资源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)。

### 按角色查看 {#view-by-role}

在资源规划者中选择角色视图时，请考虑以下事项：

* 您必须至少具有资源管理的查看访问权限和项目的查看权限，才能查看与这些项目关联的角色。
* 您可以展开每个角色以显示项目列表，展开每个项目以显示可在项目中履行这些角色的用户列表。
* 为了提高性能，您显示或可以从“角色视图”中导出的项目数量是有限的。\
  有关详细信息，请参阅[资源规划者显示限制](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)中角色视图部分的限制。

* 项目在工作角色下列出，其优先顺序与项目视图中所列的顺序相同。
* 应用此视图后，项目小时数、FTE或成本将合计到角色小时数、FTE或成本。
* 您可以在“角色”视图中查看以下小时、FTE或成本信息：

   * 可用
   * 计划
   * 已预算
   * 变量
   * 净值

     有关详细信息，请参阅使用项目和角色视图的资源规划者中的[预算资源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)。

### 按用户查看 {#view-by-user}

您可以在用户视图中显示资源规划者，以了解计划的小时数与用户的可用小时数或FTE之间的差异，或查看他们记录的实际小时数。

将用户视图应用于资源规划者时，您无法预算资源。 您必须使用“项目”或“角色”视图来预算资源，并使用“用户”视图来查看与计划工作相关的用户分配和可用性。

用户视图是资源规划者的默认视图。

在资源规划者中选择“用户视图”时，请考虑以下事项：

* 您可以看到您有权查看的所有用户，最多有2,000个处于活动状态且至少已登录Adobe Workfront一次的用户。 按团队、工作角色或池筛选用户列表，以查看仅与这些实体关联的用户。
* 如果已按项目筛选用户列表，则只有与已筛选项目关联的用户才能展开并显示小时信息。\
  有关详细信息，请参阅资源规划者[&#128279;](../../resource-mgmt/resource-planning/filter-resource-planner.md)中的筛选信息。

* 为了提高性能，您显示或可从“用户视图”中导出的项目数会受到限制。\
  有关详细信息，请参阅[资源规划者显示限制](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)中“用户视图”部分的限制。

* 项目按照与项目视图中所列顺序相同的优先级列在用户名称下。\
  有关详细信息，请参阅本文中的[项目计划优先级](#project-planning-priority)部分。

* 如果用户没有关联的工作角色，则小时数或FTE值会列在无角色部分下。
* 应用此视图后，项目小时或FTE总计为用户小时或FTE。

  >[!TIP]
  >
  >您不能在“用户视图”中按“成本”显示用户的分配和可用性。

* 您的项目和任务权限决定了在“用户视图”中看到的用户名称下显示的内容。

  存在以下情况：

   * 如果您无权查看项目以及分配给资源规划者中显示的用户的任务或问题，则这些项目列在无法访问的项目部分下。 在这种情况下，这些部分将替换“项目”或“任务”部分。

   * 如果您无权查看项目，但有权查看项目的任务或问题，则项目、任务和问题将列在分配给它们的用户的名称下。
   * 如果您有权查看项目，但没有查看项目中的任何任务或问题，则会显示项目名称，并且任务和问题列在“无法访问的项目”部分下。

     有关详细信息，请参阅[对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。


* 您可以在“用户”视图中查看以下小时和FTE信息：

   * 可用
   * 计划
   * 实际
   * 计划与实际之间的差异
   * 计划分配的百分比

     有关详细信息，在使用用户视图时，请参阅资源规划者中的[查看可用、计划和实际小时数或FTE](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)

## 项目名称

您可以在资源规划者中看到以下项目：

* 您有权查看的项目。 您还必须具有在访问级别查看资源管理的访问权限。

  有关信息，请参阅[在Adobe Workfront中预算资源所需的访问权限](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)。

* 受应用于资源规划者的过滤器限制的项目。

  有关详细信息，请参阅资源规划者[&#128279;](../../resource-mgmt/resource-planning/filter-resource-planner.md)中的筛选信息。

  >[!NOTE]
  >
  >我们建议使用过滤器减少您在资源规划者中显示的项目数。

## 项目计划优先级 {#project-planning-priority}

项目按优先级在资源规划程序中列出，最重要的项目在顶部。 优先级由项目名称前面的数字表示。

![项目计划优先级](assets/project-ranking.png)

您还可以启用设置，以便在项目与项目组合关联时，根据项目组合显示项目优先级。 有关信息，请参阅[在资源规划者](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md)中排定项目的优先级。

## 职位角色名称

资源规划者中列出了以下工作角色类别：

* 分配给任务的工作角色。
* 未分配给任务但是与项目的资源池关联的用户的首要工作角色的工作角色。
* 分配给这些工作角色中任务的用户的辅助工作角色。
* 在其配置文件中具有有效FTE可用性百分比的用户的辅助工作角色。\
  有关工作角色的FTE可用性百分比的详细信息，请参阅[编辑用户的配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

>[!NOTE]
>
>启用包括来自问题的小时数设置后，也会列出分配给问题的工作角色。 有关在资源规划者中启用问题时数的详细信息，请参阅[设置](#settings)部分。

## 用户名

资源规划者的“项目”和“角色”视图中列出的用户属于与项目关联的资源池。\
有关详细信息，请参阅[将资源池与用户关联](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md)。

您有权查看且已登录Workfront至少一次的所有用户都将显示在“用户视图”中。

在“项目”和“角色”视图中，用户可显示在以下工作角色类型下：

* 他们的主要工作角色
* 他们的辅助工作角色，在以下场景中：

   * 辅助工作角色在其用户配置文件中具有FTE可用性百分比的有效数字。
   * 如果用户被分配到这些角色中的任务。
有关工作角色FTE可用性百分比的更多信息，请参阅[编辑用户配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) 。

## 无角色和用户部分

### 无角色部分  {#no-role-section}

当用户属于与项目关联的资源池，但没有与其关联的工作角色时，他们显示在“无角色”部分而不是特定工作角色下。

您不能为无角色分区中的用户预算小时数。 用户必须具有至少一个与其关联的工作角色才能为工作编列预算。


### 无用户部分  {#no-user-section}

将任务分配给团队或保持未分配状态时，计划小时数显示在无用户部分下，该部分显示在资源规划者的无角色部分下。 使用“按用户查看”视图时，这些任务不会显示在资源规划者中。

您可以在资源规划者的“无用户”部分中看到项目上任务归因的计划小时数，但无法为这些分配编列预算。

![无用户部分](assets/no-user.png)

## 过滤器

通过使用过滤器，您可以限制在资源规划者中显示的信息。

![筛选器按钮](assets/filter-button.png)

有关在资源规划者中进行筛选的更多信息，请参阅[资源规划者中的筛选信息](../../resource-mgmt/resource-planning/filter-resource-planner.md) 。

## 设置 {#settings}

在“设置”区域中，可以启用或禁用在“资源规划者”中显示或隐藏信息的选项。 要打开“资源规划者设置”对话框，请单击页面右上角的设置图标。

![资源规划者设置图标](assets/settings-icon.png)

在此处，您可以启用以下一项或两项设置：

* **包括来自问题的小时数**：这显示来自问题的已计划小时数。

  启用此设置时，请考虑以下事项：

   * 分配给问题的用户名称显示在问题中与其关联的工作角色下。 您可以在“项目”和“角色”视图中指定用户的预算小时数以及工作角色。
   * 在“用户”视图中，用户所分配到的问题列在工作角色的名称下。

     >[!IMPORTANT]
     >
     >当问题的计划开始日期和完成日期在项目的时间表之外时，问题的计划小时数根据问题的日期显示。 例如，如果项目时间线在一月到三月之间，但问题的时间线是在八月，则问题的计划小时数将显示在八月时间段。


* **显示Portfolio优先级**：根据项目所分配的Portfolio显示项目优先级。

  有关在资源规划程序中排列项目优先顺序的信息，请参阅[在资源规划程序中排列项目优先顺序](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md)。


  ![资源规划者设置](assets/resource-planner-settings.png)

## 全屏选项

您可以全屏显示资源规划者，以放大可在屏幕上查看的信息量。 此选项适用于所有视图。

要全屏显示资源规划者，请单击页面右上角的全屏图标。

![RP_sull_sccreen_area_User_View__1_.png](assets/rp-full-screen-icon-highlighted-user-view--350x260.png)

展开屏幕后，您可以单击关闭全屏图标以恢复为以前的显示。

## 导出选项

![导出按钮](assets/export-button-highlighted-resource-planner-350x92.png)

您可以从资源规划者的任何视图将信息导出到Excel (.xlsx)文件。

有关从资源规划者导出信息的信息，请参阅[从资源规划者导出信息](../../resource-mgmt/resource-planning/export-resource-planner.md)。

您可以管理信息量和导出文件的显示。

有关可从资源规划者导出哪些信息以及如何管理导出文件外观的信息，请参阅[资源规划者显示限制](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)。
