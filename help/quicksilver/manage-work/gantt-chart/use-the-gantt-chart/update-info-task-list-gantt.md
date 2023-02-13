---
product-area: projects
navigation-topic: use-the-gantt-chart
title: 更新任务列表甘特图中的信息
description: 任务列表甘特图显示有关项目或模板上任务的详细信息。
author: Alina
feature: Work Management
exl-id: 0a8e6fd5-985c-49e5-842d-67ade29ee1c9
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 1%

---

# 更新任务列表中的信息 [!UICONTROL 甘特图]

任务列表 [!UICONTROL 甘特图] 显示有关项目或模板中任务的详细信息。

在模板中，任务列表 [!UICONTROL 甘特图] 反映在模板任务级别的任务列表中所做的更新。 您无法编辑 [!UICONTROL 甘特图] 与模板关联。

在项目中，您可以直接在任务列表中更新任务信息 [!UICONTROL 甘特图].

本文介绍了可直接在任务列表中执行的以下操作 [!UICONTROL 甘特图]:

* 修改任务持续时间
* 创建或删除前置关系
* 更改任务开始和结束日期
* 更新完成百分比
* 级别项目资源

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL计划] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>对项目和任务的[!UICONTROL编辑]访问权限</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>[!UICONTROL管理]对项目和任务的访问权限 </p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 修改任务持续时间

1. 转到要修改的项目。
1. 单击 **[!UICONTROL 任务]** 中。

   ![](assets/qs-tasks-area-highlighted-in-the-secondary-nav-350x206.png)

1. 单击 **[!UICONTROL 甘特图]** 图标。

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

   所有更改在 **[!UICONTROL 自动保存]** 选项。 默认情况下处于启用状态。

1. （可选）单击 **[!UICONTROL 计划模式]** 图标，选择 **[!UICONTROL 手动保存Standard]** 或 **[!UICONTROL 时间轴规划]** 以手动保存更改。

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 将鼠标悬停在任务的时间轴上，然后将时间线指示器拖动到其他日期。
1. 当任务达到正确的新完成日期时，请删除指示器。
1. （可选和视情况而定）如果您选择手动保存更改，请单击 **[!UICONTROL 撤消]** 或&#x200B;**[!UICONTROL 重做]** 图标。

   >[!TIP]
   >
   >您可以使用以下键盘快捷键撤消或重做甘特图上的更改：
   >
   >   
   >   
   >   * [!DNL Mac]:使用 [!UICONTROL Command + Z] 撤消和 [!UICONTROL Command + Shift + Z] 重做。
   >   * [!DNL Windows]:使用 [!UICONTROL Ctrl + Z] 撤消和 [!UICONTROL Ctrl + Y] 重做。


1. 单击 **[!UICONTROL 保存]** 的右上角 [!UICONTROL 甘特图].

## 创建或删除前置关系

1. 转到要修改的项目。
1. 在 **[!UICONTROL 任务]** 区域，单击 **[!UICONTROL 甘特图]** 图标。

   的 **[!UICONTROL 自动保存]** 选项，在这种情况下，所有更改都会自动保存。

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. （可选）单击 **[!UICONTROL 计划模式]** 图标，选择 **[!UICONTROL 手动保存Standard]** 或 **[!UICONTROL 时间轴规划]** 以手动保存更改。

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 要创建前置关系，请单击任务的起始点并将其拖动到任务的终点。
1. 要删除前置关系，请单击连接两个任务的前置行以将其选中，然后按 **[!UICONTROL 删除]** 键盘上。\
   ![Delete_prepisent.png](assets/delete-predecessor-350x152.png)

1. （可选和视情况而定）如果您选择手动保存更改，请单击 **[!UICONTROL 撤消]** 或&#x200B;**[!UICONTROL 重做]** 图标。

   >[!TIP]
   >
   >您可以使用以下键盘快捷键撤消或重做甘特图上的更改：
   >
   >   
   >   
   >   * [!DNL Mac]:使用 [!UICONTROL Command + Z] 撤消和 [!UICONTROL Command + Shift + Z] 重做。
   >   * [!DNL Windows]: [!UICONTROL 使用Ctrl + Z] 撤消和 [!UICONTROL Ctrl + Y] 重做。


1. 单击&#x200B;**[!UICONTROL 保存]**。

## 更改任务开始和结束日期

1. 转到要修改的项目。
1. 在 **[!UICONTROL 任务]** 区域，单击 **[!UICONTROL 甘特图]** 图标。

   所有更改在 **[!UICONTROL 自动保存]** 选项。 默认情况下处于启用状态。

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. （可选）单击 **[!UICONTROL 计划模式]** 图标，选择 **[!UICONTROL 手动保存Standard]** 或 **[!UICONTROL 时间轴规划]** 以手动保存更改。

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 将鼠标悬停在任务的中心上，并找到多向箭头。
1. 单击并将任务拖到所需的日期。

   ![Change_start_end_date.png](assets/change-start-end-date.png)

1. 如果更改任务日期的方式影响任务约束，请单击 **[!UICONTROL 接受]** 确认任务约束更改。

   >[!NOTE]
   >
   >如果任务具有以下约束之一，则系统会更新 [!UICONTROL 任务约束] to [!UICONTROL 开始前否] 如果从 [!UICONTROL 开始日期] 或 [!UICONTROL 不迟于完成] 是否从 [!UICONTROL 完成日期]:
   >
   >   
   >   
   >   * [!UICONTROL 尽可能早]
   >   * [!UICONTROL 尽可能迟]
   >   * [!UICONTROL 最早可用时间]
   >   * [!UICONTROL 最晚可用时间]

   >   
   >   
   >在某些情况下，前置关系可能会阻止任务提前开始，并且不允许任务移动。

1. （可选和视情况而定）如果您选择手动保存更改，请单击 **[!UICONTROL 撤消]** 或&#x200B;**[!UICONTROL 重做]** 图标。

   >[!TIP]
   >
   >您可以使用以下键盘快捷键撤消或重做 [!UICONTROL 甘特图]:
   >
   >   
   >   
   >   * [!DNL Mac]:使用 [!UICONTROL Command + Z] 撤消和 [!UICONTROL Command + Shift + Z] 重做。
   >   * [!DNL Windows]:使用 [!UICONTROL Ctrl + Z] 撤消和 [!UICONTROL Ctrl + Y] 重做。


1. 单击&#x200B;**[!UICONTROL 保存]**。

## 更新完成百分比

1. 转到要修改的项目。
1. 在 **[!UICONTROL 任务]** 区域，单击 **[!UICONTROL 甘特图]** 图标。

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

   所有更改在 **[!UICONTROL 自动保存]** 选项。 默认情况下处于启用状态。

1. （可选）单击 **[!UICONTROL 计划模式]** 图标，选择 **[!UICONTROL 手动保存Standard]** 或 **[!UICONTROL 时间轴规划]** 以手动保存更改。
1. 双击任务内部的百分比数字并输入该数字。

   >[!IMPORTANT]
   >
   >您必须 [!UICONTROL 完成%] 在 [!UICONTROL 选项] 对话框，以更新完成百分比。 为此，请单击 **[!UICONTROL 选项]** 图标，选择 **[!UICONTROL 完成%]**.
   >
   >
   >![update_percent_complete.png](assets/update-percent-complete-350x175.png)   >

1. （可选和视情况而定）如果您选择手动保存更改，请单击 **[!UICONTROL 撤消]** 或&#x200B;**[!UICONTROL 重做]** 图标。

   >[!TIP]
   >
   >您可以使用以下键盘快捷键撤消或重做 [!UICONTROL 甘特图]:
   >
   >   
   >   
   >   * [!DNL Mac]:使用 [!UICONTROL Command + Z] 撤消和 [!UICONTROL Command + Shift + Z] 重做。
   >   * [!DNL Windows]:使用 [!UICONTROL Ctrl + Z] 撤消和 [!UICONTROL Ctrl + Y] 重做。


1. 单击 **[!UICONTROL 保存]** 的右上角 [!UICONTROL 甘特图].

## 级别项目资源

您可以使用任务列表 [!UICONTROL 甘特图] 来提升您的资源级别。

有关在 [!UICONTROL 甘特图]，请参阅 [中的级别资源 [!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;this is drafted because I moved the whole content to the article linked above)</p>
<ol>
<li value="1">Go to the project you want to level.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> In the <strong>Tasks</strong> area, click the <strong>Gantt chart</strong> icon.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">All changes are saved automatically when the <strong>Autosave</strong> option is enabled. It is enabled by default. </p> </li>
<li value="3">
<div>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) Click the <strong>Plan mode</strong> icon and select <strong>Manual save Standard</strong> or <strong>Timeline Planning</strong> to save your changes manually.</p> <note type="tip">
You cannot level resources in the Gantt chart when the Autosave option is enabled.
</note>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png" style="width: 350;height: 493;"> </p>
</div> </li>
<li value="4"> <p>Click the <strong>Level Resources</strong> drop-down menu.</p> <p> <img src="assets/level-resouces.png" alt="Level_resouces.png"> </p> </li>
<li value="5">Select one of following options:
<ul>
<li><strong>Level Now</strong>: Applies resource leveling to the selected task.</li>
<li><p><strong>Clear Leveling</strong>: Removes all resource leveling from the selected task.</p></li>
</ul><note type="note">
Your resources might be overallocated if they are assigned to multiple tasks which occur during the same time frame.
</note></li>
<li value="6"> <p>(Optional and conditional) If you have disabled the Autosave option, click the <strong>Undo</strong> or<strong>Redo</strong> icons if you want to cancel or duplicate any of the changes. </p> <note type="tip">
<p>You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:</p>
<ul>
<li>Mac: Use Command + Z to undo and Command + Shift + Z to redo.</li>
<li>Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.</li>
</ul>
</note> </li>
<li value="7">Click <strong>Save</strong> in the upper-right corner of the Gantt chart.</li>
</ol>
</div>
-->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"> </h2>
-->
