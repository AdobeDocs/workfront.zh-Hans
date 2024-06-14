---
title: 报告更新区域
description: 日志条目报表会从项目、任务、问题和其他对象的更新区域显示系统更新，以前只能通过Adobe Workfront API使用这些更新区域。 虽然这是一个针对特定用例的高级报告，但采用更易于理解的格式后，您可以在Workfront中报告项目活动和系统更新。
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: ecf947ce-54d8-4103-8903-f455b1d86c39
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '2776'
ht-degree: 3%

---

# 报告更新区域

日志条目报表会从项目、任务、问题和其他对象的更新区域显示系统更新，以前只能通过Adobe Workfront API使用这些更新区域。 虽然这是一个针对特定用例的高级报告，但采用更易于理解的格式后，您可以在Workfront中报告项目活动和系统更新。

>[!TIP]
>
>日志条目报表仅包含来自对象更新区域的系统更新。 要报告“更新”区域中留下的注释，您必须使用“注释”报告。\
>有关“注释”报表的更多信息，请参阅 [在备注报告中查看所有更新](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md). ‍

日记帐分录报表可以显示：

* 发生了多少次状态更改
* 删除任务或问题时
* 重要自定义字段中的值在项目生命周期中的变化情况
* 在项目生命周期中哪些重要日期发生了变化
* 如果项目所有者已更改

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>新增：标准 </p><p>或 </p><p>当前：计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看对包含您在报表中显示的日志条目的对象的权限</p> <p>在创建报告后，您将获得对报告的管理权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 先决条件

在执行本文中所述的操作之前，必须确保以下各项：

* 您要报告的任何字段均在Workfront中进行跟踪。 您只能报告更新区域中被跟踪的数据。

  要了解如何添加希望Workfront跟踪的字段，请参阅 [配置系统更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* 要报告的任何自定义字段均具有设置 **在更新源中显示字段更改** 已启用。

  要了解如何为自定义字段启用此设置，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#).

## 日记帐分录报表概览

由于“日志条目”报表会查询系统更新，因此它可以返回大量结果。 因此，我们建议您在创建报告时过滤到特定对象，如项目、项目群、项目组合、组等。

要了解有关Workfront中各种对象类型的更多信息，请参阅 [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>由于日志条目报表返回的数据很多，因此不支持导出和计划报表提交。

此报表的默认视图包含以下列：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>字段</th> 
   <th>说明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>字段名称</strong> </td> 
   <td> <p><span style="font-weight: normal;">受影响字段的名称。 根据您设置报表的方式，此列可能包含“状态”、“所有者ID”、“任务名称”、“计划完成日期”或其他字段。</span> </p> <p><span style="font-weight: normal;">时间</span> <strong>DE</strong>：<span style="font-weight: normal;"> 显示在此列中，它指示列出的字段是自定义字段。</span></p> </td> 
  </tr> 
  <tr> 
   <td><strong>更改类型</strong> </td> 
   <td> <p>对受影响字段所做的更改类型。 根据您设置的过滤器规则以及用户执行的操作，此字段可能会显示以下内容：</p> 
    <ul> 
     <li> <p>添加</p> </li> 
     <li> <p>审计</p> </li> 
     <li> <p>删除</p> </li> 
     <li> <p>摘要</p> </li> 
     <li> <p>编辑</p> </li> 
     <li> <p>恢复</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>主要对象代码</strong> </td> 
   <td> <p>层次结构中最高的父对象。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>范围</strong> </td> 
   <td> <p>已更改的对象的类型。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>输入日期</strong> </td> 
   <td> <p>字段的更改日期。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>按名称编辑</strong> </td> 
   <td> <p>更改字段的用户。</p> </td> 
  </tr> 
 </tbody> 
</table>

要组织此报表中的信息，您可以使用称为“项目”的内置分组。 项目分组为您提供项目名称的主要分组和输入日期的辅助分组。 您可以在报告创建期间应用此现有分组，也可以在查看报告时应用此现有分组。

要了解如何为报告设置所需的视图、筛选器和分组，请参阅相关部分：

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: from&nbsp;Luke: Take this for what it's worth, but part of me wonders if all of these subsections should be separate articles.</p>
<p>The biggest reason for breaking these up would be searchability, in my mind. For example, as a user, I might want to know how to see if the owner of a project changed. If I search the help site for that, I would be a lot more likely to find a separate article called "See if the owner of a project changed" vs an article titled "Create a Journal Entry report" because "Journal Entry" might mean nothing to me.) </p>
</div>
-->

* [查看发生了哪些状态更改](#see-what-status-changes-occurred)
* [查看任务或问题何时被删除](#see-when-a-task-or-issue-was-deleted)
* [查看自定义字段在项目生命周期中的变化](#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle)
* [查看规划完成日期在项目生命周期中的变化](#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle)
* [查看项目所有者是否已更改](#see-if-the-owner-of-a-project-changed)

## 查看发生了哪些状态更改 {#see-what-status-changes-occurred}

您可以设置“日记帐分录”报表以显示：

* 一个项目、任务或问题更改了多少状态

* 更改前的状态
* 谁更改了状态
* 发生状态更改的时间

如果要查看项目的运行状况，还可以使用项目设置报表以显示相同的信息 **条件** 字段。

此信息可用于帮助进行审核以及说明您和您的组织的计划情况。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;for tip below: When analytics adds the status option, update this note to say "these entries (status or condition changes)")</p>
-->

>[!TIP]
>
>如果要比较条件更改之间的天数差异，您可以使用增强型分析。\
>要了解有关增强型分析的更多信息，请参阅 [增强的分析概述](../../../enhanced-analytics/enhanced-analytics-overview.md).

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **报表**.
1. 单击 **新建报告**，然后选择 **日志条目**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   加载Report Builder。

1. 在 **列（视图）** 选项卡，添加以下列：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>列</th> 
      <th>说明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">字段名称</p> </td> 
      <td> <p>受影响字段的名称。 在本例中， <strong>状态</strong> 应会显示在此列中。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改类型</p> </td> 
      <td> <p>对受影响字段所做的更改类型，如 <strong>添加</strong>， <strong>删除</strong>，或 <strong>编辑</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">按名称编辑</p> </td> 
      <td> <p>更新状态的用户的名称。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">输入日期</p> </td> 
      <td> <p>状态更改的日期。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">旧文本值</p> </td> 
      <td> <p>上一个状态的键。 以下是默认项目状态的状态键：</p> 
       <ul> 
        <li> <p> <strong>当前</strong>：当前</p> </li> 
        <li> <p><strong>DED</strong>：已终止</p> </li> 
        <li> <p><strong>ONE</strong>：保持</p> </li> 
        <li> <p><strong>计划</strong>：规划</p> </li> 
        <li> <p><strong>CPL</strong>：完成</p> </li> 
        <li> <p><strong>需要</strong>：已请求</p> </li> 
        <li> <p><strong>四月</strong>：已批准</p> </li> 
        <li> <p><strong>REJ</strong>：已拒绝</p> </li> 
        <li> <p><strong>IDA</strong>：构思</p> </li> 
       </ul> <p>如果您的组织设置了自定义状态，则此列中可能会显示其他状态键。 要了解哪些自定义状态与状态键相关，请与Workfront管理员或组管理员联系。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新文本值</p> </td> 
      <td> <p>更新状态的密钥。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">主要的对象代码</p> </td> 
      <td> <p>状态更改的字段的最高父对象。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">范围</p> </td> 
      <td> <p>具有状态更改的对象的类型。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">问题名称<br>（可选）</p> </td> 
      <td> <p>状态发生更改的问题名称。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">任务名称<br>（可选）</p> </td> 
      <td> <p>状态已更改的任务的名称。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   有关添加列的详细信息，请参见 [Adobe Workfront中的视图概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **过滤器** 选项卡，单击 **添加筛选器规则**，然后添加筛选规则 **字段名称** > **等于** > **状态**.

   ![](assets/nwe-journal-entry-status-filter-rules-350x90.png)

   >[!TIP]
   >
   >要报告条件更改，您可以改为添加筛选规则 **字段名称** > **等于** > **条件**.

   有关添加过滤器的更多信息，请参阅 [过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （可选）要缩小报告的焦点并减少加载时间，请添加提示。

   或

   创建其他筛选器规则以包含特定项目、任务或问题。

   >[!IMPORTANT]
   >
   >创建使用该修饰符的过滤器规则 **包含** 实际上会增加加载时间。 因此，我们建议使用其他修饰符，例如 **等于** 筛选特定项目或更高级别的对象ID。

   要了解如何添加提示，请参阅 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 在 **分组** 选项卡，单击 **应用现有分组**，然后选择 **项目**.

   有关添加分组的详细信息，请参阅 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 单击 **保存+关闭**.

   新报表将被加载。

## 查看任务或问题何时被删除 {#see-when-a-task-or-issue-was-deleted}

您可以设置“日记帐分录”报表以显示：

* 已删除哪些任务或问题
* 谁删除了任务或问题

要查看任务或问题何时被删除，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **报表**.
1. 单击 **新建报告**，然后选择 **日志条目**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   加载Report Builder。

1. 在 **列（视图）** 选项卡，添加以下列：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>列</th> 
      <th>说明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">范围</p> </td> 
      <td> <p>已删除的对象类型。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改类型</p> </td> 
      <td> <p>发生的更改类型。 此 <strong>删除</strong> 更改将显示在此列中。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">输入日期</p> </td> 
      <td> <p>删除任务或问题的日期。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">按名称编辑</p> </td> 
      <td> <p>删除任务或问题的用户的名称。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">项目名称</p> </td> 
      <td> <p>已删除任务或问题的项目的名称。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   有关添加列的详细信息，请参见 [Adobe Workfront中的视图概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **过滤器** 选项卡，单击 **添加筛选器规则**，然后添加以下过滤器：

   * **更改类型** > **等于** > **删除**
   * **项目编号** > **等于** > **`<project>`**

     <!--WRITER check link; this png file has spaces
     [![](assets/classic-task-or-issue-deleted-350x90.png)](../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png)-->

   有关添加过滤器的更多信息，请参阅 [过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （可选）要缩小报告的焦点并减少加载时间，请添加提示。

   或

   创建其他筛选器规则以包含特定项目、任务或问题。

   >[!IMPORTANT]
   >
   >创建使用该修饰符的过滤器规则 **包含** 实际上会增加加载时间。 因此，我们建议使用其他修饰符，例如 **等于** 筛选特定项目或更高级别的对象ID。

   要了解如何添加提示，请参阅 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. （可选）在 **分组** 选项卡，单击 **应用现有分组**，然后选择 **项目**.

   有关添加分组的详细信息，请参阅 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 单击 **保存+关闭**.

   新报表将被加载。

## 查看自定义字段在项目生命周期中的变化 {#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle}

您可以跟踪项目过程中重要的字段更改。 为此，您可以设置要跟踪的日志条目：

* 添加、更新或编辑某些自定义字段时
* 发生这些更改的时间
* 谁进行了更改

要查看自定义字段在项目生命周期中的变化情况，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **报表**.
1. 单击 **新建报告**，然后选择 **日志条目**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   加载Report Builder。

1. 在 **列（视图）** 选项卡，添加以下列：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>列</th> 
      <th>说明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">字段名称</p> </td> 
      <td> <p>受影响的自定义字段的名称。</p> <p><span style="font-weight: normal;">时间</span> <strong>DE</strong>：<span style="font-weight: normal;"> 显示在此列中，它指示列出的字段是自定义字段。</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改类型</p> </td> 
      <td> <p>对受影响字段所做的更改类型，如 <strong>添加</strong>， <strong>删除</strong>，或 <strong>编辑</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">按名称编辑</p> </td> 
      <td> <p>更新自定义字段的用户的名称。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">输入日期</p> </td> 
      <td> <p>自定义字段中值的更改日期。</p> <p>您应该按此字段降序排序。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">旧数值</p> </td> 
      <td> <p>自定义字段中的上一个数值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新数值</p> </td> 
      <td> <p>自定义字段中的当前数值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">旧日期值</p> </td> 
      <td> <p>自定义字段中的上一个日期值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新日期值</p> </td> 
      <td> <p>自定义字段中的当前日期值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">旧文本值</p> </td> 
      <td> <p>自定义字段中的上一个文本值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新文本值</p> </td> 
      <td> <p>自定义字段中的当前文本值。</p> <p>如果自定义字段是预输入字段，则 <strong>新建文本值</strong> 列显示对象ID。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   有关添加列的详细信息，请参见 [Adobe Workfront中的视图概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **过滤器** 选项卡，单击 **添加筛选器规则**，然后添加以下过滤器：

   * **日志条目字段名称** > **包含** > **DE**

     >[!TIP]
     >
     >要将此报告限制到特定的自定义字段，请添加筛选规则 **日志条目字段名称** > **等于** > **`<custom field>`**.

   * **项目编号** > **等于** > **`<project>`**

     ![](assets/qs-custom-form-changes-filter-350x92.png)

   有关添加过滤器的更多信息，请参阅 [过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （可选）要缩小报告的焦点并减少加载时间，请添加提示。

   或

   创建其他筛选器规则以包含特定项目、任务或问题。

   >[!IMPORTANT]
   >
   >创建使用该修饰符的过滤器规则 **包含** 实际上会增加加载时间。 因此，我们建议使用其他修饰符，例如 **等于** 筛选特定项目或更高级别的对象ID。

   要了解如何添加提示，请参阅 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 在 **分组** 选项卡，单击 **应用现有分组**，然后选择 **项目**.

   有关添加分组的详细信息，请参阅 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 单击 **保存+关闭**.

   新报表将被加载。

## 查看规划完成日期在项目生命周期中的变化 {#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle}

您可以设置“日记帐分录”报表，以显示计划完成日期在项目生命周期中的更改频率。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **报表**.
1. 单击 **新建报告**，然后选择 **日志条目**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   加载Report Builder。

1. 在 **列（视图）** 选项卡，添加以下列：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>列</th> 
      <th>说明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">字段名称</p> </td> 
      <td> <p>受影响字段的名称。</p> <p><span style="font-weight: normal;">时间</span> <strong>DE</strong>：<span style="font-weight: normal;"> 显示在此列中，它指示列出的字段是自定义字段。</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改类型</p> </td> 
      <td>发生的更改类型，如 <strong>添加</strong>， <strong>删除</strong>，或 <strong>编辑</strong>.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">按名称编辑</p> </td> 
      <td> <p>更新了项目的计划完成日期的用户的名称。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">输入日期</p> </td> 
      <td> <p>更改项目计划完成日期的日期。</p> <p>您应该按此字段降序排序。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">主要的对象代码</p> </td> 
      <td> <p>计划完成日期更改的字段的最高父对象。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">范围</p> </td> 
      <td> <p>计划完成日期更改的对象。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">旧日期值</p> </td> 
      <td> <p>计划完成日期的上一个值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新日期值</p> </td> 
      <td> <p>计划完成日期的当前值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">项目名称</p> <p>（可选）</p> </td> 
      <td> <p>计划完成日期更改的项目名称。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">任务名称</p> <p>（可选）</p> </td> 
      <td> <p>项目中计划完成日期更改的任务的名称。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">问题名称</p> <p>（可选）</p> </td> 
      <td>项目中计划完成日期发生更改的问题名称。</td> 
     </tr> 
    </tbody> 
   </table>

   有关添加列的详细信息，请参见 [Adobe Workfront中的视图概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **过滤器** 选项卡，单击 **添加筛选器规则**，然后添加以下内容：

   * **字段名称** > **等于** > **日期**
   * **项目编号** > **等于** > **`<project>`**

   ![](assets/qs-planned-completion-date-change-filter-350x91.png)

   有关添加过滤器的更多信息，请参阅 [过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （可选）要缩小报告的焦点并减少加载时间，请添加提示。

   或

   创建其他筛选器规则以包含特定项目、任务或问题。

   >[!IMPORTANT]
   >
   >创建使用该修饰符的过滤器规则 **包含** 实际上会增加加载时间。 因此，我们建议使用其他修饰符，例如 **等于** 筛选特定项目或更高级别的对象ID。

   要了解如何添加提示，请参阅 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 在 **分组** 选项卡，单击 **应用现有分组**，然后选择 **项目**.

   有关添加分组的详细信息，请参阅 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 单击 **保存+关闭**.

   新报表将被加载。

## 查看项目所有者是否已更改 {#see-if-the-owner-of-a-project-changed}

您可以设置“日记条目”报表，以显示项目所有者（或项目经理）在项目生命周期中的更改次数。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **报表**.
1. 单击 **新建报告**，然后选择 **日志条目**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   加载Report Builder。

1. 在 **列（视图）** 选项卡，添加以下列：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>列</th> 
      <th>说明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">字段名称</p> </td> 
      <td>受影响字段的名称。 此 <strong>ownerID</strong> 将显示在此列中。</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改类型</p> </td> 
      <td> <p>发生的更改类型，如 <strong>添加</strong>， <strong>删除</strong>，或 <strong>编辑</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">主要的对象代码</p> </td> 
      <td> <p>已更新项目所有者的项目的最高父对象。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">输入日期</p> </td> 
      <td>更改项目所有者的日期。<br>您应该按此字段降序排序。</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">按名称编辑</p> </td> 
      <td> <p>更新项目所有者的用户的名称。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">附加信息 1</p> </td> 
      <td> <p>项目的当前项目所有者。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">附加信息 2</p> </td> 
      <td> <p>项目的前一个项目所有者。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">项目名称</p> </td> 
      <td> <p>更新了项目所有者字段的项目。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   有关添加列的详细信息，请参见 [Adobe Workfront中的视图概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **过滤器** 选项卡，单击 **添加筛选器规则**，然后添加以下内容：

   * **字段名称** > **等于** > **ownerID**
   * **项目编号** > **等于** > **`<project name>`**

     ![](assets/qs-owner-changes-filter-350x94.png)

   有关添加过滤器的更多信息，请参阅 [过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （可选）要缩小报告的焦点并减少加载时间，请添加提示。

   或

   创建其他筛选器规则以包含特定项目、任务或问题。

   >[!IMPORTANT]
   >
   >创建使用该修饰符的过滤器规则 **包含** 实际上会增加加载时间。 因此，我们建议使用其他修饰符，例如 **等于** 筛选特定项目或更高级别的对象ID。

   要了解如何添加提示，请参阅 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. （可选）在 **分组** 选项卡，单击 **应用现有分组**，然后选择 **项目**.

   有关添加分组的详细信息，请参阅 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 单击 **保存+关闭**.

   新报表将被加载。
