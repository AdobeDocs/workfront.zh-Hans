---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 在日历报表中使用计划日期
description: 日历报告是一种动态报告，提供工作的可视化表示形式。 您可以在任务、问题和项目的日历报告中使用“规划日期”字段。
author: Lisa
feature: Reports and Dashboards
exl-id: 27bf6f03-2f6b-4556-a715-75c4a21bfbbb
source-git-commit: 78cfafe4c9a0fb846533c04da392a09dc1dbc9f1
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 2%

---

# 在日历报告中使用[!UICONTROL 计划日期]

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</span> 
-->

日历报告是一种动态报告，提供工作的可视化表示形式。 您可以在日历报告中为以下对象使用[!UICONTROL 计划日期]字段：

* 任务
* 问题
* 项目

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>[！UICONTROL编辑]对[！UICONTROL报表]、[！UICONTROL功能板]和[！UICONTROL日历的访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>[！UICONTROL Manage]对日历报表的访问权限</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 设置生产中的项目组

您可以选择您希望项目组在日历上显示的方式。

{{step1-to-calendars}}

1. 选择要向其添加新项目组的日历。
或
单击**[!UICONTROL +新建日历]**&#x200B;并输入日历名称。

   >[!NOTE]
   >
   >您必须拥有访问级别的报告、功能板和日历的编辑访问权限，才能创建日历报告。

1. 在左侧，单击&#x200B;**[!UICONTROL 添加到日历]**，然后单击&#x200B;**[!UICONTROL 添加高级项目]**。

1. 指定以下内容：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL命名这组项目]</strong></td>
      <td>键入项目组的名称。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL颜色]</strong></td>
      <td>选择项目组的颜色。 所有项目均以选定的颜色显示在日历报表中。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL日期字段]</strong></td>
      <td><p>选择<strong>[！UICONTROL计划日期]</strong>。 有关计划日期的详细信息，请参阅 </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-start-date.md" class="MCXref xref">项目计划开始日期概述</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">任务计划开始日期概述</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">任务计划完成日期概览</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">设置项目计划完成日期</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>在日历上，显示</strong></td>
      <td><p>选择日期的显示方式：</p>
       <ul>
        <li><strong>[！UICONTROL仅开始日期]</strong>：日历在单个日期显示对象。</li>
        <li><strong>[！UICONTROL仅结束日期]</strong>：日历在单个日期显示对象。</li>
        <li><strong>[！UICONTROL Duration] （开始到结束）</strong>：日历显示跨天对象。</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[！UICONTROL在可用时切换到实际日期]</strong></td>
      <td><p>当日期可用时，日历会自动切换到实际日期。 <br>选择<strong>[！UICONTROL是]</strong>或<strong>[！UICONTROL否]</strong>以切换到实际日期（可用时）。 有关实际日期的详细信息，请参阅</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">项目实际开始日期概览 </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">项目实际完成日期概览 </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. 继续下一节。

## 将对象添加到生产中的项目组

设置项目显示方式后，您需要将要在日历上看到的对象添加到分组中。

1. 在&#x200B;**[!UICONTROL 中，您希望向日历添加什么？]**&#x200B;分区，选择

   * **[!UICONTROL 任务]**
   * **[!UICONTROL 项目]**
   * **[!UICONTROL 问题]**

1. 根据要添加到日历的对象类型，单击&#x200B;**[!UICONTROL 添加任务]**、**[!UICONTROL 添加项目]**&#x200B;或&#x200B;**[!UICONTROL 添加问题]**。
   ![为日历](assets/field-name.png)选择对象

1. 在下拉菜单中，开始键入字段名称，然后选择要显示在日历上的对象的字段源（例如，**[!UICONTROL 延迟任务]**）。
1. 为日历分组设置条件语句。

   ![条件语句](assets/condition-statement-calendar.png)

   要了解如何设置条件，请参阅[筛选器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

1. （可选）通过重复步骤1-4为日历分组指定其他对象。
1. 在&#x200B;**[!UICONTROL 将任务/项目/问题标签设置为……]**&#x200B;字段中，选择此日历分组中的对象在日历中的标签方式。

   >[!NOTE]
   >
   >如果某个对象无法使用默认标签选项，则会改为显示对象名称。 例如，当选择[!UICONTROL 父任务]标签并且没有与对象关联的父任务时，[!DNL Adobe Workfront]将显示您在日历中查看的对象名称。

1. 单击&#x200B;**[!UICONTROL 保存]**。

<!--

## Set up the group of items in Preview

You can choose how you want the group of items to display on your calendar.

{{step1-to-calendars}}

1. Select the calendar you want to add a new group of items to.
   Or
   Click **[!UICONTROL + New Calendar]** and enter the calendar name.

   >[!NOTE]
   >
   >You must have Edit access to Reports, Dashboards, and Calendars in your access level to create a calendar report.

1. On the left, click **[!UICONTROL Add to Calendar]**, then click **[!UICONTROL Add advanced items]**.

1. Specify the following:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Name this group of items]</strong></td>
      <td>Type a name for the group of items.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Select a color for the group of items. All items display in the selected color on the calendar report.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Date Field]</strong></td>
      <td><p>Choose <strong>[!UICONTROL Planned dates]</strong>. For more information on planned dates, see </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-start-date.md" class="MCXref xref">Overview of the project Planned Start Date</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Overview of the task Planned Start Date</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Overview of the task Planned Completion Date</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Set the project Planned Completion Date</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>On the calendar, show</strong></td>
      <td><p>Choose how you want the dates to show:</p>
       <ul>
        <li><strong>[!UICONTROL Start Date Only]</strong>: The calendar displays the object on a single date.</li>
        <li><strong>[!UICONTROL End Date Only]</strong>: The calendar displays the object on a single date.</li>
        <li><strong>[!UICONTROL Duration] (Start to End)</strong>: The calendar displays the object over a span of days.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Switch to actual dates when available]</strong></td>
      <td><p>The calendar automatically switches to actual dates when they are available. <br>Choose <strong>[!UICONTROL Yes]</strong> or <strong>[!UICONTROL No]</strong> to switch to actual dates when available. For more information on Actual Dates, see</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Overview of the project Actual Start Date </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Overview of the project Actual Completion Date </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Continue to the following section.

## Add objects to the group of items in Preview

After you set up how you want items to display, you need to add the objects you want to see on the calendar to the grouping.

1. In the **[!UICONTROL What would you like to add to the calendar?]** section, select

   * **[!UICONTROL Tasks]**
   * **[!UICONTROL Projects]**
   * **[!UICONTROL Issues]**

1. Click **[!UICONTROL Add Tasks]**, **[!UICONTROL Add Projects]**, or **[!UICONTROL Add Issues]**, depending on the object type you are adding to the calendar.
   ![Select object for calendar](assets/field-name.png)

1. In the drop-down menu, begin typing the field name, then select the field source of the object you want to display on the calendar (for example, **[!UICONTROL Late Tasks]**).
1. Set a condition statement for the calendar grouping.

   ![Condition statement](assets/condition-statement-calendar.png)

   To learn about setting conditions, see [Filter and condition modifiers](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Optional) Specify additional objects for the calendar grouping by repeating Steps 1-4.
1. In the **[!UICONTROL Set the Tasks/Projects/Issues labels to be the...]** field, select how the objects in this calendar grouping are labeled in the calendar.

   >[!NOTE]
   >
   >If the default label options are not available for a certain object, the object name is shown instead. For example, when the [!UICONTROL Parent Task] label is selected and there is no parent task associated with the object, [!DNL Adobe Workfront] displays the object name you are viewing in the calendar.

1. Click **[!UICONTROL Save]**. 

-->