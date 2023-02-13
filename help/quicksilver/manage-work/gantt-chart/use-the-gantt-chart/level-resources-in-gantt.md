---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: 中的级别资源  [!UICONTROL 甘特图]
description: 有关如何在甘特图中对资源进行分级的信息。
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 0%

---

# 中的级别资源 [!UICONTROL 甘特图]

在项目上调整资源有两个用途：

* 自动调整分配人的超量分配时间。
* 自动为项目创建实际的任务计划。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL计划] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>对项目的[!UICONTROL编辑]访问权限</p> <p><b>注释</b>

如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>对项目的[!UICONTROL管理]访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 资源平衡概述

如果将同一资源分配给两个不同的任务，则可以使用资源平整来调整任务的时间轴，这样它们就不会同时发生。

在项目上调平资源时，请考虑以下事项：

* 资源调平仅适用于一个项目，因此 [!DNL Adobe Workfront] 不会一次跨多个项目进行资源级别。
* 如果 **[!UICONTROL 努力驱动]** 作为 **[!UICONTROL 持续时间类型]**, [!DNL Workfront] 不会对资源进行分级。
* 当将多个用户分配到同一任务时，将取消调平。
* 类型的条件 **[!UICONTROL 任务约束]** 将优先于资源的均等。 例如，如果 **[!UICONTROL 固定日期]** 作为 [!UICONTROL 任务约束]，则资源调平不会更改任务日期。
* 前置关系优先于资源平衡。
* **[!UICONTROL 资源平衡]** 需要将 **[!UICONTROL 手动]** 为了在 [!UICONTROL 甘特图]. 如果您对项目具有“管理”权限，则可以让系统通过调整项目中的此设置并选择 **[!UICONTROL 自动]** 而不是 **[!UICONTROL 手动]** 在 **[!UICONTROL 编辑项目]** 框中。

   ![](assets/resource-leveling-mode-350x177.png)

* 作为项目所有者或任务代理人，您可以为任务引入调平延迟，以指明任务极有可能需要额外时间。 有关向任务添加调平延迟的信息，请参阅 [更新任务调平延迟](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## 在 [!UICONTROL 甘特图]

您可以使用任务列表 [!UICONTROL 甘特图] 来提升您的资源级别。

1. 转到要级别的项目。
1. 在 **[!UICONTROL 任务]** 区域，单击 **[!UICONTROL 甘特图]** 图标。

   所有更改在 **[!UICONTROL 自动保存]** 选项。 默认情况下处于启用状态。

1. （可选）单击 **[!UICONTROL 计划] 模式** 图标，选择 **[!UICONTROL 手动保存Standard]** 或 **[!UICONTROL 时间轴规划]** 以手动保存更改。

   >[!TIP]
   >
   >不能在  [!UICONTROL 甘特图] 当 [!UICONTROL 自动保存] 选项。

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 单击 **[!UICONTROL 级别资源]** 下拉菜单。

   ![Level_resources.png](assets/level-resouces.png)

1. 选择以下选项之一：

   * **[!UICONTROL 立即级别]**:将资源平整应用于选定的任务。
   * **[!UICONTROL 清除调平]**:从选定任务中删除所有资源均等。

   >[!NOTE]
   >
   >如果资源被分配到同一时间范围内发生的多个任务，则它们可能会被过度分配。

1. （可选并视情况而定）如果已禁用自动保存选项，请单击 **[!UICONTROL 撤消]** 或&#x200B;**[!UICONTROL 重做]** 图标。

   >[!TIP]
   >
   >您可以使用以下键盘快捷键撤消或重做 [!UICONTROL 甘特图]:
   >
   >* [!DNL Mac]:使用 [!UICONTROL Command + Z] 撤消和 [!UICONTROL Command + Shift + Z] 重做。
   >* Windows:使用 [!UICONTROL Ctrl + Z] 撤消和 [!UICONTROL Ctrl + Y] 重做。



1. 单击 **[!UICONTROL 保存]** 的右上角 [!UICONTROL 甘特图].

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Overview of Leveling Delay</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article: /Content/Manage work/Tasks/Task information/task-leveling-delay.htm) </p>
<p>At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic schedule. </p>
<p>As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels the tasks a more realistic schedule overcomes resource conflicts.</p>
<p>To manually add a Leveling Delay to a task:</p>
<ol>
<li value="1">Navigate to a task for which you want to add a Leveling Delay.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the <strong>More icon</strong> to the right of the task name, then click <strong>Edit</strong>. </p> <p> <img src="assets/qs-task-edit-icon-highlighted-350x154.png" style="width: 350;height: 154;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
