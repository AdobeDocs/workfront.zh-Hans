---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: 均衡资源  [!UICONTROL 甘特图]
description: 有关如何在甘特图中调配资源的信息。
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# 均衡资源 [!UICONTROL 甘特图]

在项目中均衡资源有两个目的：

* 自动调整被分配人的时间过度分配。
* 为项目自动创建现实的任务计划。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] 许可证*</td> 
   <td> <p>[！UICONTROL计划] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>[！UICONTROL Edit]对项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>[！UICONTROL Manage]对项目的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 资源均衡概览

如果将同一资源分配给两个不同的任务，则可以使用资源均衡调整任务的时间表，以使它们不会同时发生。

在项目上调配资源时，请考虑以下事项：

* 资源均衡仅适用于一个项目，因此 [!DNL Adobe Workfront] 不会一次跨多个项目调配资源。
* 如果 **[!UICONTROL 投入比导向]** 已选为 **[!UICONTROL 持续时间类型]**， [!DNL Workfront] 不会均衡资源。
* 将多个用户分配到同一任务时，将取消均衡。
* 以下类型的条件 **[!UICONTROL 任务限制]** 将优先于资源均衡。 例如，如果 **[!UICONTROL 固定日期]** 已选为 [!UICONTROL 任务限制]，资源均衡不会更改任务日期。
* 前置任务关系将优先于资源均衡。
* **[!UICONTROL 资源均衡]** 需要设置为 **[!UICONTROL 手动]** 用于项目，以便调整中的均衡 [!UICONTROL 甘特图]. 如果您拥有项目的管理权限，则可以通过调整项目上的此设置并选择 **[!UICONTROL 自动]** 而不是 **[!UICONTROL 手动]** 在 **[!UICONTROL 编辑项目]** 盒子。

  ![](assets/resource-leveling-mode-350x177.png)

* 作为项目所有者或任务受让人，您可以为任务引入均衡延迟，以表示任务极有可能需要额外的时间。 有关向任务添加均衡延迟的信息，请参见 [更新任务均衡延迟](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## 在中应用资源均衡 [!UICONTROL 甘特图]

您可以使用任务列表 [!UICONTROL 甘特图] 以调配资源。

1. 转到要均衡的项目。
1. 在 **[!UICONTROL 任务]** 区域，单击 **[!UICONTROL 甘特图]** 图标。

   所有更改都会在 **[!UICONTROL 自动保存]** 选项。 默认情况下处于启用状态。

1. （可选）单击 **[!UICONTROL 计划] 模式** 图标并选择 **[!UICONTROL 手动保存标准]** 或 **[!UICONTROL 时间线规划]** 以手动保存更改。

   >[!TIP]
   >
   >您无法在中调配资源  [!UICONTROL 甘特图] 当 [!UICONTROL 自动保存] 选项。

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 单击 **[!UICONTROL 均衡资源]** 下拉菜单。

   ![Level_resources.png](assets/level-resouces.png)

1. 选择以下选项之一：

   * **[!UICONTROL 立即均衡]**：将资源均衡应用于所选任务。
   * **[!UICONTROL 清除均衡]**：从选定任务中删除所有资源均衡。

   >[!NOTE]
   >
   >如果将资源分配给同一时间范围内发生的多个任务，则这些资源可能会过度分配。

1. （可选且视情况而定）如果已禁用自动保存选项，请单击 **[!UICONTROL 还原]** 或&#x200B;**[!UICONTROL 重做]** 图标来取消或复制任何更改。

   >[!TIP]
   >
   >您可以使用以下键盘快捷键撤消或重做对 [!UICONTROL 甘特图]：
   >
   >* [!DNL Mac]：使用 [!UICONTROL Command + Z] 撤消并 [!UICONTROL Command + Shift + Z] 以重做。
   >* Windows：使用 [!UICONTROL Ctrl + Z] 撤消并 [!UICONTROL Ctrl + Y] 以重做。


1. 单击 **[!UICONTROL 保存]** 位于的右上角 [!UICONTROL 甘特图].

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Overview of Leveling Delay</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article: /Content/Manage work/Tasks/Task information/task-leveling-delay.htm) </p>
<p>At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic schedule. </p>
<p>As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels the tasks a more realistic schedule overcomes resource conflicts.</p>
<p>To manually add a Leveling Delay to a task:</p>
<ol>
<li value="1">Navigate to a task for which you want to add a Leveling Delay.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the <strong>More icon</strong> to the right of the task name, then click <strong>Edit</strong>. </p>  </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
