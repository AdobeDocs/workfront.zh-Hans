---
title: 报告更新区域
description: 报告更新区域
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: ecf947ce-54d8-4103-8903-f455b1d86c39
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2698'
ht-degree: 4%

---

# 报告更新区域

“日记帐分录”报表显示系统从项目、任务、问题和其他对象的“更新”区域进行的更新，这些对象以前只能通过Adobe Workfront API使用。 虽然这是一份面向特定用例的高级报表，但是更易于理解的格式可让您更轻松地报告Workfront中的项目活动和系统更新。

>[!TIP]
>
>“日记帐分录”报表仅包含对象“更新”区域的系统更新。 要报告“更新”区域中剩余的注释，必须使用“注释”报表。\
>有关注释报表的详细信息，请参阅 [在备注报表中查看所有更新](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md). ‍

“日记帐分录”报表可显示：

* 发生了多少次状态更改
* 删除任务或问题时
* 重要自定义字段中的值在项目生命周期中的变化情况
* 在项目的生命周期中更改了哪些重要日期
* 如果项目的所有者发生更改

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
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看包含报表中显示的日记帐分录的对象的权限</p> <p>在创建报表后，您将获得该报表的管理权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在执行本文所述的操作之前，必须确保：

* 您要报告的任何字段都将在Workfront中进行跟踪。 您只能报告所跟踪更新区域的数据。

   要了解如何添加要Workfront跟踪的字段，请参阅 [配置系统更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* 要报告的任何自定义字段均具有设置 **在更新馈送中显示字段更改** 已启用。

   要了解如何为自定义字段启用此设置，请参阅部分 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) 在文章中 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 日记帐分录报表概述

由于日记帐分录报表查询系统更新，因此它可返回大量结果。 因此，我们建议您在创建报表时过滤特定对象（如项目、项目、项目组合、组等）。

要详细了解Workfront中的不同对象类型，请参阅 [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>由于“日记帐分录”报表返回了大量数据，因此不支持导出和计划报表提交。

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
   <td> <p><span style="font-weight: normal;">受影响字段的名称。 根据报表的设置方式，此列可能包含“状态”、“所有者ID”、“任务名称”、“计划完成日期”或其他字段。</span> </p> <p><span style="font-weight: normal;">When</span> <strong>DE</strong>:<span style="font-weight: normal;"> 显示在此列中，表示列出的字段是自定义字段。</span></p> </td> 
  </tr> 
  <tr> 
   <td><strong>更改类型</strong> </td> 
   <td> <p>对受影响的字段所做的更改类型。 根据您设置的过滤器规则和用户执行的操作，此字段中可能会显示以下内容：</p> 
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
   <td><strong>主要的对象代码</strong> </td> 
   <td> <p>层次结构中最高的父对象。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>范围</strong> </td> 
   <td> <p>已更改的对象类型。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>输入日期</strong> </td> 
   <td> <p>字段更改的日期。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>按名称编辑</strong> </td> 
   <td> <p>更改字段的用户。</p> </td> 
  </tr> 
 </tbody> 
</table>

要组织此报表中的信息，您可以使用内置的分组项目。 “项目”分组为您提供“项目名称”的主要分组和“登入日期”的辅助分组。 您可以在报表创建期间应用此现有分组，也可以在查看报表时应用此现有分组。

要了解如何为报表设置所需的视图、过滤器和分组，请参阅相关部分：

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: from&nbsp;Luke: Take this for what it's worth, but part of me wonders if all of these subsections should be separate articles.</p>
<p>The biggest reason for breaking these up would be searchability, in my mind. For example, as a user, I might want to know how to see if the owner of a project changed. If I search the help site for that, I would be a lot more likely to find a separate article called "See if the owner of a project changed" vs an article titled "Create a Journal Entry report" because "Journal Entry" might mean nothing to me.) </p>
</div>
-->

* [查看发生了哪些状态更改](#see-what-status-changes-occurred)
* [查看任务或问题何时被删除](#see-when-a-task-or-issue-was-deleted)
* [查看自定义字段在项目生命周期中的更改情况](#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle)
* [查看计划完成日期在项目生命周期中是如何更改的](#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle)
* [查看项目所有者是否发生更改](#see-if-the-owner-of-a-project-changed)

## 查看发生了哪些状态更改 {#see-what-status-changes-occurred}

您可以设置“日记帐分录”报表以显示：

* 对项目、任务或问题进行了多少次状态更改

* 更改前的状态
* 更改了状态的人
* 状态更改发生时

如果要查看项目的运行状况，还可以设置报表以使用项目显示相同的信息 **条件** 字段。

此信息可用于帮助进行审核，并说明您和贵组织的计划情况。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;for tip below: When analytics adds the status option, update this note to say "these entries (status or condition changes)")</p>
-->

>[!TIP]
>
>如果要比较条件更改之间的天数差异，可以使用增强的分析。\
>要了解有关Enhanced Analytics的更多信息，请参阅 [增强的分析概述](../../../enhanced-analytics/enhanced-analytics-overview.md).

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **报表**.
1. 单击 **新建报表**，然后选择 **日记帐分录**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   加载报表生成器。

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
      <td> <p>受影响字段的名称。 在这种情况下， <strong>状态</strong> 应显示在此列中。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改类型</p> </td> 
      <td> <p>对受影响的字段所做的更改类型，如 <strong>添加</strong>, <strong>删除</strong>或 <strong>编辑</strong>.</p> </td> 
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
      <td> <p>上一状态的键。 以下是默认项目状态的状态键：</p> 
       <ul> 
        <li> <p> <strong>CUR</strong>:当前</p> </li> 
        <li> <p><strong>DED</strong>:死亡</p> </li> 
        <li> <p><strong>ONH</strong>:保持</p> </li> 
        <li> <p><strong>PLN</strong>:规划</p> </li> 
        <li> <p><strong>CPL</strong>:完成</p> </li> 
        <li> <p><strong>请求</strong>:请求</p> </li> 
        <li> <p><strong>4月</strong>:已批准</p> </li> 
        <li> <p><strong>REJ</strong>:被拒绝</p> </li> 
        <li> <p><strong>IDA</strong>:构思</p> </li> 
       </ul> <p>如果贵组织已设置自定义状态，则其他状态键可能会显示在此列中。 要了解与状态键相关的自定义状态，请联系Workfront管理员或组管理员。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新文本值</p> </td> 
      <td> <p>更新状态的键。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">主要的对象代码</p> </td> 
      <td> <p>状态发生更改的字段的最高父对象。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">范围</p> </td> 
      <td> <p>状态发生更改的对象类型。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">问题名称<br>（可选）</p> </td> 
      <td> <p>状态发生更改的问题的名称。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">任务名称<br>（可选）</p> </td> 
      <td> <p>状态发生更改的任务的名称。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   有关添加列的更多信息，请参阅 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **过滤器** ，单击 **添加过滤器规则**，然后添加过滤器规则 **字段名称** > **等于** > **状态**.

   ![](assets/nwe-journal-entry-status-filter-rules-350x90.png)

   >[!TIP]
   >
   >要报告条件更改，您可以添加过滤器规则 **字段名称** > **等于** > **条件**.

   有关添加过滤器的更多信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （可选）要缩小报表焦点并缩短加载时间，请添加提示。

   或

   创建其他过滤器规则以包含特定项目、任务或问题。

   >[!IMPORTANT]
   >
   >创建使用修饰符的过滤器规则 **包含** 实际上会增加加载时间。 因此，我们建议使用其他修饰符，例如 **等于** （如果可能）筛选特定项目或更高级别的对象ID。

   要了解如何添加提示，请参阅 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 在 **分组** ，单击 **应用现有分组**，然后选择 **项目**.

   有关添加分组的更多信息，请参阅 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 单击 **保存并关闭**.

   加载新报表。

## 查看任务或问题何时被删除 {#see-when-a-task-or-issue-was-deleted}

您可以设置“日记帐分录”报表以显示：

* 删除了哪些任务或问题
* 删除任务或问题的人员

要查看任务或问题何时被删除，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **报表**.
1. 单击 **新建报表**，然后选择 **日记帐分录**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   加载报表生成器。

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
      <td> <p>发生的更改类型。 的 <strong>删除</strong> 此列中将显示更改。</p> </td> 
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
      <td> <p>已删除任务或问题的项目名称。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   有关添加列的更多信息，请参阅 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **过滤器** ，单击 **添加过滤器规则**，然后添加以下内容：

   * **更改类型** > **等于** > **删除**
   * **项目ID** > **等于** > **`<project>`**

      <!--WRITER check link; this png file has spaces
     [![](assets/classic-task-or-issue-deleted-350x90.png)](../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png)-->
   有关添加过滤器的更多信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （可选）要缩小报表焦点并缩短加载时间，请添加提示。

   或

   创建其他过滤器规则以包含特定项目、任务或问题。

   >[!IMPORTANT]
   >
   >创建使用修饰符的过滤器规则 **包含** 实际上会增加加载时间。 因此，我们建议使用其他修饰符，例如 **等于** （如果可能）筛选特定项目或更高级别的对象ID。

   要了解如何添加提示，请参阅 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. （可选）在 **分组** ，单击 **应用现有分组**，然后选择 **项目**.

   有关添加分组的更多信息，请参阅 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 单击 **保存并关闭**.

   加载新报表。

## 查看自定义字段在项目生命周期中的更改情况 {#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle}

您可以在项目过程中跟踪重要字段的更改。 为此，您可以设置“日记帐分录”以跟踪：

* 如果添加、更新或编辑了某些自定义字段
* 发生这些更改时
* 谁做了更改

要查看自定义字段在项目生命周期中的更改情况，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **报表**.
1. 单击 **新建报表**，然后选择 **日记帐分录**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   加载报表生成器。

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
      <td> <p>受影响的自定义字段的名称。</p> <p><span style="font-weight: normal;">When</span> <strong>DE</strong>:<span style="font-weight: normal;"> 显示在此列中，表示列出的字段是自定义字段。</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改类型</p> </td> 
      <td> <p>对受影响的字段所做的更改类型，如 <strong>添加</strong>, <strong>删除</strong>或 <strong>编辑</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">按名称编辑</p> </td> 
      <td> <p>更新自定义字段的用户名称。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">输入日期</p> </td> 
      <td> <p>自定义字段中的值发生更改的日期。</p> <p>您应该按此字段的降序排序。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">旧数值</p> </td> 
      <td> <p>自定义字段中的上一个数字值。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新数值</p> </td> 
      <td> <p>自定义字段中的当前数字值。</p> </td> 
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
      <td> <p>自定义字段中的当前文本值。</p> <p>如果自定义字段是类型提前字段，则 <strong>新文本值</strong> 列显示对象ID。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   有关添加列的更多信息，请参阅 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **过滤器** ，单击 **添加过滤器规则**，然后添加以下内容：

   * **日记帐分录字段名称** > **包含** > **DE**

      >[!TIP]
      >
      >要将此报表限制为特定的自定义字段，请添加过滤器规则 **日记帐分录字段名称** > **等于** > **`<custom field>`**.

   * **项目ID** > **等于** > **`<project>`**

      ![](assets/qs-custom-form-changes-filter-350x92.png)
   有关添加过滤器的更多信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （可选）要缩小报表焦点并缩短加载时间，请添加提示。

   或

   创建其他过滤器规则以包含特定项目、任务或问题。

   >[!IMPORTANT]
   >
   >创建使用修饰符的过滤器规则 **包含** 实际上会增加加载时间。 因此，我们建议使用其他修饰符，例如 **等于** （如果可能）筛选特定项目或更高级别的对象ID。

   要了解如何添加提示，请参阅 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 在 **分组** ，单击 **应用现有分组**，然后选择 **项目**.

   有关添加分组的更多信息，请参阅 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 单击 **保存并关闭**.

   加载新报表。

## 查看计划完成日期在项目生命周期中是如何更改的 {#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle}

您可以设置“日记帐分录”报表以显示计划完成日期在项目生命周期中更改的频率。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **报表**.
1. 单击 **新建报表**，然后选择 **日记帐分录**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   加载报表生成器。

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
      <td> <p>受影响字段的名称。</p> <p><span style="font-weight: normal;">When</span> <strong>DE</strong>:<span style="font-weight: normal;"> 显示在此列中，表示列出的字段是自定义字段。</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改类型</p> </td> 
      <td>发生的更改类型，例如 <strong>添加</strong>, <strong>删除</strong>或 <strong>编辑</strong>.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">按名称编辑</p> </td> 
      <td> <p>更新项目计划完成日期的用户名称。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">输入日期</p> </td> 
      <td> <p>更改项目计划完成日期的日期。</p> <p>您应该按此字段的降序排序。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">主要的对象代码</p> </td> 
      <td> <p>具有计划完成日期更改的字段的最高父对象。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">范围</p> </td> 
      <td> <p>具有计划完成日期更改的对象。</p> </td> 
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
      <td> <p style="font-weight: bold;">项目名称</p> <p>(可选的)</p> </td> 
      <td> <p>具有计划完成日期更改的项目名称。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">任务名称</p> <p>(可选的)</p> </td> 
      <td> <p>项目中具有计划完成日期更改的任务的名称。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">问题名称</p> <p>(可选的)</p> </td> 
      <td>项目中计划完成日期发生更改的问题的名称。</td> 
     </tr> 
    </tbody> 
   </table>

   有关添加列的更多信息，请参阅 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **过滤器** ，单击 **添加过滤器规则**，然后添加以下内容：

   * **字段名称** > **等于** > **日期**
   * **项目ID** > **等于** > **`<project>`**

   ![](assets/qs-planned-completion-date-change-filter-350x91.png)

   有关添加过滤器的更多信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （可选）要缩小报表焦点并缩短加载时间，请添加提示。

   或

   创建其他过滤器规则以包含特定项目、任务或问题。

   >[!IMPORTANT]
   >
   >创建使用修饰符的过滤器规则 **包含** 实际上会增加加载时间。 因此，我们建议使用其他修饰符，例如 **等于** （如果可能）筛选特定项目或更高级别的对象ID。

   要了解如何添加提示，请参阅 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 在 **分组** ，单击 **应用现有分组**，然后选择 **项目**.

   有关添加分组的更多信息，请参阅 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 单击 **保存并关闭**.

   加载新报表。

## 查看项目所有者是否发生更改 {#see-if-the-owner-of-a-project-changed}

您可以设置“日记帐分录”报表以显示项目所有者或项目经理在项目生命周期中更改的次数。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **报表**.
1. 单击 **新建报表**，然后选择 **日记帐分录**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   加载报表生成器。

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
      <td>受影响字段的名称。 的 <strong>ownerID</strong> 显示在此列中。</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">更改类型</p> </td> 
      <td> <p>发生的更改类型，例如 <strong>添加</strong>, <strong>删除</strong>或 <strong>编辑</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">主要的对象代码</p> </td> 
      <td> <p>更新了项目所有者的项目的最高父对象。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">输入日期</p> </td> 
      <td>更改项目所有者的日期。<br>您应该按此字段的降序排序。</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">按名称编辑</p> </td> 
      <td> <p>更新项目所有者的用户名称。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">附加信息 1</p> </td> 
      <td> <p>项目的当前项目所有者。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">附加信息 2</p> </td> 
      <td> <p>项目上的上一个项目所有者。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">项目名称</p> </td> 
      <td> <p>更新了“项目所有者”字段的项目。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   有关添加列的更多信息，请参阅 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **过滤器** ，单击 **添加过滤器规则**，然后添加以下内容：

   * **字段名称** > **等于** > **ownerID**
   * **项目ID** > **等于** > **`<project name>`**

      ![](assets/qs-owner-changes-filter-350x94.png)
   有关添加过滤器的更多信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （可选）要缩小报表焦点并缩短加载时间，请添加提示。

   或

   创建其他过滤器规则以包含特定项目、任务或问题。

   >[!IMPORTANT]
   >
   >创建使用修饰符的过滤器规则 **包含** 实际上会增加加载时间。 因此，我们建议使用其他修饰符，例如 **等于** （如果可能）筛选特定项目或更高级别的对象ID。

   要了解如何添加提示，请参阅 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. （可选）在 **分组** ，单击 **应用现有分组**，然后选择 **项目**.

   有关添加分组的更多信息，请参阅 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 单击 **保存并关闭**.

   加载新报表。
