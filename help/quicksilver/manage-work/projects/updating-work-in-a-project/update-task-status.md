---
product-area: projects
navigation-topic: update-work-in-a-project
title: 更新任务状态
description: 您可以更新任务的状态，以告知其他人该任务在何处（以及整个项目）以及进展如何。
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: 1eb1e919bede7e366956d8c0bd969329a641123f
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 1%

---

# 更新任务状态

<!--Audited: 10/2024-->

您可以更新任务的状态，以告知其他人该任务在何处（以及整个项目）以及进展如何。

默认状态为“新建”、“进行中”和“完成”。 Adobe Workfront管理员可以为您的组织添加自定义状态。 有关详细信息，请参阅[创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

您可以手动更新任务状态，也可以让Workfront在某些操作发生时自动更新任务状态。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能手动更新任务：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>新增：标准</p> 
   或
   <p>当前：工作或更高</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑任务访问权限</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 有关更新任务状态的注意事项

* 将任务标记为“完成”时，任务的完成百分比将更新为100%。
* 父任务存在以下方案：
   * 当项目的“摘要完成模式”设置为“自动”且子任务未完成时，不能将父任务的状态更新为“完成”。
   * 当项目的“摘要完成模式”设置为“手动”并且子任务已完成或未完成时，您可以将父任务的状态更新为“完成”。

  有关详细信息，请参阅[编辑项目](../manage-projects/edit-projects.md)。

## 手动更新任务状态

您可以在Workfront的以下区域中更新任务状态：

* 任务页面上的任务标题。
* 编辑任务时显示的编辑任务框。
* 任务页面上的“任务详细信息”部分。
* 在任务列表或报告中，当状态字段在视图中可见时。
* 在任务的“摘要”面板中。

要在任务标题中手动更新任务状态，请执行以下操作：

1. 转到要更新其状态的任务。
1. 单击任务标题中的&#x200B;**状态**&#x200B;字段并选择新状态。
1. 要提供任务完成的可视指示，请拖动或双击任务标题中&#x200B;**完成百分比**&#x200B;下的气泡

   或

   在任务标题中的气泡内单击以输入百分比。

   ![](assets/percent-complete-status-widgets-task-header.png)

1. （可选）执行以下任一操作以提供有关更新的其他信息：

   * 若要添加有关更新的注释，请转到&#x200B;**更新**&#x200B;部分，然后单击&#x200B;**新建注释**，然后键入注释。

     ![](assets/add-update-to-task.png)

   * 若要将更新通知给某些用户，请在键入评论时显示的&#x200B;**标记人员或团队**&#x200B;字段中键入其名称。 有关详细信息，请参阅[为其他人标记更新](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)。
   * 要更新任务的提交日期，请单击&#x200B;**任务详细信息**，然后编辑&#x200B;**提交日期**&#x200B;字段。 有关信息，请参阅[编辑任务](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md)。


   >[!IMPORTANT]
   >
   >  只有任务被分配者才能更新提交日期。

<!--old functionality in old commenting: 

1. Go to a task that you are assigned to for which you want to update the status.
1. Click the **Status** field in the task header and select a new status. 
1. (Optional) Do any of the following to provide additional information about the update, then click **Update** or, if the task has the **Complete** status, click **Done:**

   * To add a note about the update, go to the **Updates** area and click **Start a new update**, then type your note.  

   * To notify certain users about the update, type their names in the **Notify** box that appears when you type a note about the update. For more information, see [Tag others on updates](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md). 
   * To update the condition of the task, click **Select Condition** to the right of the **Notify** box (these appear when you type a note about the update), then select the condition that best reflects the current condition of the task.
   
   * To update the Commit Date of the task, expand the **Commit Date** drop-down calendar, and select a new Commit Date. 
   * To provide a visual indication of task completion, drag the bubble under Percent Complete or double-click it to enter a percent value.   
     ![](assets/drag-the-progress-bar-350x155.png)-->

## 自动更新任务状态

当下表列出的操作发生时，Workfront会自动将任务的现有状态更新为其他状态。

>[!NOTE]
>
>下表中的状态是默认的系统状态。 您的Workfront管理员或组管理员可以重命名Workfront实例中的状态。 有关在Workfront中创建和管理状态的信息，请参阅[创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>操作</b></td> 
   <td><b>原始状态</b></td> 
   <td><b>新建状态</b></td> 
  </tr> 
  <tr> 
   <td>将任务完成百分比更新为100%</td> 
   <td>新建或进行中</td> 
   <td>完成</td> 
  </tr> 
  <tr> 
   <td>将任务完成百分比从100%更新为较低数字</td> 
   <td>完成</td> 
   <td>正在进行中</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>单击“开始任务”按钮接受处理分配给您的任务</span> </td> 
   <td><span>新建</span> </td> 
   <td> <p>与“主团队”设置中的“开始任务”按钮关联的任何状态。</p> <p>有关将“处理此项工作”按钮替换为“开始任务”按钮的信息，请参阅<span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">将“处理此项工作”按钮替换为“开始”按钮</a></span>。</p> <p>提示：单击“开始任务”后，<span>单击</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">撤消按钮</span>会将状态还原为“新建”。 </p> </td> 
  </tr> 
 </tbody> 
</table>
