---
product-area: projects
navigation-topic: use-the-gantt-chart
title: 更新任务列表甘特图中的信息
description: Adobe Workfront任务列表的甘特图显示有关项目或模板中任务的详细信息。
author: Alina
feature: Work Management
exl-id: 0a8e6fd5-985c-49e5-842d-67ade29ee1c9
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 1%

---

# 更新任务列表[!UICONTROL 甘特图]中的信息

<!--Audited: 08/2025-->

Adobe Workfront任务列表的[!UICONTROL 甘特图]显示有关项目或模板中任务的详细信息。

在模板中，任务列表[!UICONTROL 甘特图]反映了模板任务级别在模板任务列表中进行的更新。 您无法编辑与模板关联的[!UICONTROL 甘特图]。

在项目中，可以直接在任务列表[!UICONTROL 甘特图]中更新任务信息。

本文介绍了可直接在任务列表[!UICONTROL 甘特图]中执行的以下操作：

* 修改任务持续时间
* 创建或删除前置任务关系
* 更改任务的开始和结束日期
* 更新完成百分比
* 均衡项目资源

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>[！UICONTROL标准版]</p>
   <p>[！UICONTROL计划]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>[！UICONTROL Edit]对项目和任务的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>[！UICONTROL Manage]对项目和任务的访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++ 

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] access to the project and tasks </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 修改任务持续时间

1. 转到要修改的项目。
1. 单击左侧面板中的&#x200B;**[!UICONTROL 任务]**。

   ![任务区域](assets/qs-tasks-area-highlighted-in-the-secondary-nav-350x206.png)

1. 单击&#x200B;**[!UICONTROL 甘特图]**&#x200B;图标。

   ![单击甘特图图标](assets/click-gantt-chart-icon.png)

   启用&#x200B;**[!UICONTROL 自动保存]**&#x200B;选项后，将自动保存所有更改。 默认情况下，它处于启用状态。

1. （可选）单击&#x200B;**[!UICONTROL 计划模式]**&#x200B;图标并选择&#x200B;**[!UICONTROL 手动保存标准]**&#x200B;或&#x200B;**[!UICONTROL 时间线计划]**&#x200B;以手动保存更改。

   ![手动设置已启用](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 将鼠标悬停在任务的时间线上，并将时间线指示器拖至其他日期。
1. 在到达任务的新正确完成日期时放置指示器。
1. （可选且有条件）如果您已选择手动保存更改，如果要取消或复制任何更改，请单击&#x200B;**[!UICONTROL 撤消]**&#x200B;或&#x200B;**[!UICONTROL 重做]**&#x200B;图标。

   >[!TIP]
   >
   >可以使用以下键盘快捷键撤消或重做甘特图上的更改：
   >
   >   
   >   
   >   * [!DNL Mac]：使用[!UICONTROL Command + Z]撤消和[!UICONTROL Command + Shift + Z]重做。
   >   * [!DNL Windows]：使用[!UICONTROL Ctrl + Z]撤消和[!UICONTROL Ctrl + Y]重做。
   >   
   >

1. 单击&#x200B;**[!UICONTROL 甘特图]**&#x200B;右上角的[!UICONTROL 保存]。

## 创建或删除前置任务关系

1. 转到要修改的项目。
1. 在&#x200B;**[!UICONTROL 任务]**&#x200B;区域中，单击&#x200B;**[!UICONTROL 甘特图]**&#x200B;图标。

   默认情况下已选中&#x200B;**[!UICONTROL 自动保存]**&#x200B;选项，在这种情况下，所有更改都将自动保存。

   ![单击甘特图图标](assets/click-gantt-chart-icon.png)

1. （可选）单击&#x200B;**[!UICONTROL 计划模式]**&#x200B;图标并选择&#x200B;**[!UICONTROL 手动保存标准]**&#x200B;或&#x200B;**[!UICONTROL 时间线计划]**&#x200B;以手动保存更改。

   ![手动设置已启用](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 要创建前置任务关系，请单击任务的起点，然后将其拖到任务的终点。
1. 要删除前置任务关系，请单击连接两个任务的前置任务行以将其选定，然后按键盘上的&#x200B;**[!UICONTROL 删除]**。\
   ![Delete_precession.png](assets/delete-predecessor-350x152.png)

1. （可选且有条件）如果您选择手动保存更改，如果要取消或复制任何更改，请单击&#x200B;**[!UICONTROL 撤消]**&#x200B;或&#x200B;**[!UICONTROL 重做]**&#x200B;图标。

   >[!TIP]
   >
   >可以使用以下键盘快捷键撤消或重做甘特图上的更改：
   >
   >   
   >   
   >   * [!DNL Mac]：使用[!UICONTROL Command + Z]撤消和[!UICONTROL Command + Shift + Z]重做。
   >   * [!DNL Windows]： [!UICONTROL 使用Ctrl + Z]撤消和[!UICONTROL Ctrl + Y]重做。
   >   
   >

1. 单击&#x200B;**[!UICONTROL 保存]** 。

## 更改任务的开始和结束日期

1. 转到要修改的项目。
1. 在&#x200B;**[!UICONTROL 任务]**&#x200B;区域中，单击&#x200B;**[!UICONTROL 甘特图]**&#x200B;图标。

   启用&#x200B;**[!UICONTROL 自动保存]**&#x200B;选项后，将自动保存所有更改。 默认情况下，它处于启用状态。

   ![单击甘特图图标](assets/click-gantt-chart-icon.png)

1. （可选）单击&#x200B;**[!UICONTROL 计划模式]**&#x200B;图标并选择&#x200B;**[!UICONTROL 手动保存标准]**&#x200B;或&#x200B;**[!UICONTROL 时间线计划]**&#x200B;以手动保存更改。

   ![手动设置已启用](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 将鼠标悬停在任务的中心上，并定位多方向箭头。
1. 单击任务并将其拖动到所需的日期。

   ![Change_start_end_date.png](assets/change-start-end-date.png)

1. 如果以影响任务限制的方式更改任务日期，请单击&#x200B;**[!UICONTROL 接受]**&#x200B;以确认任务限制更改。

   >[!NOTE]
   >
   >如果任务具有以下约束之一，系统将[!UICONTROL 任务约束]更新为[!UICONTROL 开始时间不早于]。如果项目计划从[!UICONTROL 开始日期]开始，或者[!UICONTROL 完成时间不晚于]（如果项目计划从[!UICONTROL 完成日期]开始）：
   >
   >   
   >   
   >   * [!UICONTROL 尽快]
   >   * [!UICONTROL 尽可能迟]
   >   * [!UICONTROL 最早可用时间]
   >   * [!UICONTROL 最新可用时间]
   >   
   >   
   >在某些情况下，前置任务关系可能会阻止任务提前开始，并且不允许任务移动。

1. （可选且有条件）如果您已选择手动保存更改，如果要取消或复制任何更改，请单击&#x200B;**[!UICONTROL 撤消]**&#x200B;或&#x200B;**[!UICONTROL 重做]**&#x200B;图标。

   >[!TIP]
   >
   >您可以使用以下键盘快捷键撤消或重做[!UICONTROL 甘特图]上的更改：
   >
   >   
   >   
   >   * [!DNL Mac]：使用[!UICONTROL Command + Z]撤消和[!UICONTROL Command + Shift + Z]重做。
   >   * [!DNL Windows]：使用[!UICONTROL Ctrl + Z]撤消和[!UICONTROL Ctrl + Y]重做。
   >   
   >

1. 单击&#x200B;**[!UICONTROL 保存]**。

## 更新完成百分比

1. 转到要修改的项目。
1. 在&#x200B;**[!UICONTROL 任务]**&#x200B;区域中，单击&#x200B;**[!UICONTROL 甘特图]**&#x200B;图标。

   ![单击甘特图图标](assets/click-gantt-chart-icon.png)

   启用&#x200B;**[!UICONTROL 自动保存]**&#x200B;选项后，将自动保存所有更改。 默认情况下，它处于启用状态。

1. （可选）单击&#x200B;**[!UICONTROL 计划模式]**&#x200B;图标并选择&#x200B;**[!UICONTROL 手动保存标准]**&#x200B;或&#x200B;**[!UICONTROL 时间线计划]**&#x200B;以手动保存更改。
1. 双击任务内部的百分比数字并输入数字。

   >[!IMPORTANT]
   >
   >您必须在[!UICONTROL 选项]对话框中选择[!UICONTROL %完成]，才能更新完成百分比。 为此，请单击&#x200B;**[!UICONTROL 选项]**&#x200B;图标并选择&#x200B;**[!UICONTROL %完成]**。
   >
   >
   >![update_percent_complete.png](assets/update-percent-complete-350x175.png)   >
   >

1. （可选且有条件）如果您选择手动保存更改，如果要取消或复制任何更改，请单击&#x200B;**[!UICONTROL 撤消]**&#x200B;或&#x200B;**[!UICONTROL 重做]**&#x200B;图标。

   >[!TIP]
   >
   >您可以使用以下键盘快捷键撤消或重做[!UICONTROL 甘特图]上的更改：
   >
   >   
   >   
   >   * [!DNL Mac]：使用[!UICONTROL Command + Z]撤消和[!UICONTROL Command + Shift + Z]重做。
   >   * [!DNL Windows]：使用[!UICONTROL Ctrl + Z]撤消和[!UICONTROL Ctrl + Y]重做。
   >   
   >

1. 单击&#x200B;**[!UICONTROL 甘特图]**&#x200B;右上角的[!UICONTROL 保存]。

## 均衡项目资源

您可以使用任务列表[!UICONTROL 甘特图]来均衡资源。

有关[!UICONTROL 甘特图]中资源均衡的信息，请参阅[甘特图[!UICONTROL 中的]](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md)级别资源。

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
