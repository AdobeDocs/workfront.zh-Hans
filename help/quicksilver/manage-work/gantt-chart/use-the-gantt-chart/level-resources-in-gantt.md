---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: '[!UICONTROL 甘特图]中的均衡资源'
description: 有关如何在甘特图中调配资源的信息。
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# [!UICONTROL 甘特图]中的均衡资源

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

如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何修改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>[！UICONTROL Manage]对项目的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 资源均衡概览

如果将同一资源分配给两个不同的任务，则可以使用资源均衡调整任务的时间表，以使它们不会同时发生。

在项目上调配资源时，请考虑以下事项：

* 资源均衡仅适用于一个项目，因此[!DNL Adobe Workfront]不会一次跨多个项目均衡资源。
* 如果选择&#x200B;**[!UICONTROL 投入比驱动]**&#x200B;作为&#x200B;**[!UICONTROL 持续时间类型]**，则[!DNL Workfront]将不均衡资源。
* 将多个用户分配到同一任务时，将取消均衡。
* **[!UICONTROL 任务约束]**&#x200B;类型的条件优先于资源均衡。 例如，如果选择&#x200B;**[!UICONTROL 固定日期]**&#x200B;作为[!UICONTROL 任务约束]，则资源均衡将不会更改任务日期。
* 前置任务关系将优先于资源均衡。
* 项目的&#x200B;**[!UICONTROL 资源均衡]**&#x200B;需要设置为&#x200B;**[!UICONTROL 手动]**，才能在[!UICONTROL 甘特图]中调整均衡。 如果您拥有项目的管理权限，则可以通过调整项目的此设置并在&#x200B;**[!UICONTROL 编辑项目]**&#x200B;框中选择“**[!UICONTROL 自动]**”而不是“**[!UICONTROL 手动]**”，让系统自动调配资源。

  ![](assets/resource-leveling-mode-350x177.png)

* 作为项目所有者或任务受让人，您可以为任务引入均衡延迟，以表示任务极有可能需要额外的时间。 有关向任务添加均衡延迟的信息，请参阅[更新任务均衡延迟](../../../manage-work/tasks/task-information/task-leveling-delay.md)。

## 在[!UICONTROL 甘特图]中应用资源均衡

您可以使用任务列表[!UICONTROL 甘特图]来均衡资源。

1. 转到要均衡的项目。
1. 在&#x200B;**[!UICONTROL 任务]**&#x200B;区域中，单击&#x200B;**[!UICONTROL 甘特图]**&#x200B;图标。

   启用&#x200B;**[!UICONTROL 自动保存]**&#x200B;选项后，将自动保存所有更改。 默认情况下处于启用状态。

1. （可选）单击&#x200B;**[!UICONTROL 计划]模式**&#x200B;图标并选择&#x200B;**[!UICONTROL 手动保存标准]**&#x200B;或&#x200B;**[!UICONTROL 时间线计划]**&#x200B;以手动保存更改。

   >[!TIP]
   >
   >启用[!UICONTROL 自动保存]选项时，无法在[!UICONTROL 甘特图]中调配资源。

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 单击&#x200B;**[!UICONTROL 级资源]**&#x200B;下拉菜单。

   ![Level_resources.png](assets/level-resouces.png)

1. 选择以下选项之一：

   * **[!UICONTROL 立即级别]**：将资源均衡应用于所选任务。
   * **[!UICONTROL 清除均衡]**：从选定任务中删除所有资源均衡。

   >[!NOTE]
   >
   >如果将资源分配给同一时间范围内发生的多个任务，则这些资源可能会过度分配。

1. （可选且有条件）如果已禁用“自动保存”选项，则如果要取消或复制任何更改，请单击&#x200B;**[!UICONTROL 撤消]**&#x200B;或&#x200B;**[!UICONTROL 重做]**&#x200B;图标。

   >[!TIP]
   >
   >您可以使用以下键盘快捷键撤消或重做[!UICONTROL 甘特图]上的更改：
   >
   >* [!DNL Mac]：使用[!UICONTROL Command + Z]撤消和[!UICONTROL Command + Shift + Z]重做。
   >* Windows：使用[!UICONTROL Ctrl + Z]撤消和[!UICONTROL Ctrl + Y]重做。


1. 单击[!UICONTROL 甘特图]右上角的&#x200B;**[!UICONTROL 保存]**。

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
