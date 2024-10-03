---
product-area: projects
navigation-topic: update-work-in-a-project
title: 查看和更新任务的完成百分比
description: 您可以更新任务的完成百分比，以指明完成任务的进度。
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: 1eb1e919bede7e366956d8c0bd969329a641123f
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# 查看和更新任务的完成百分比

<!--Audited:01/2024-->

您可以更新任务的完成百分比，以指明完成任务的进度。

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
   <td> <p>新许可证： Standard</p> 
   或
   <p>当前许可证：工作或更高</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑任务访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 您可以更新任务的完成百分比的区域

您可以在以下任意区域更新任务的完成百分比：

* **在任务列表中**：显示“完成百分比”列时，您可以更新任务的完成百分比。\
  有关内联编辑的更多信息，请参阅[在Adobe Workfront的列表中内联编辑项目](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md)。

* **在里程碑视图**&#x200B;中：在项目列表或项目报告中使用里程碑视图时，您可以更新任务的完成百分比。 有关详细信息，请参阅[使用里程碑视图](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md)。

<!--only in legacy commenting: 
* **As you update the task**:  You can update the percent complete option of a task when adding an update to the task.

  >[!IMPORTANT]
  >
  >This option displays only after you enable the Show Percent Complete option.  
  >To enable the percent complete update bar for tasks, do the following:   
  >
  >1. Go to the **Main** menu>your name>**More** icon next to your name >**Edit** > select **Show percent complete on update status**.   
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >-->

* **在任务标题中**：您可以在任务标题中更新任务的完成百分比。 有关信息，请参阅[编辑任务](../../tasks/manage-tasks/edit-tasks.md)。

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)

* **在任务的“摘要”面板中**：您可以在查看以下区域中的任务时更新摘要面板顶部的任务完成百分比：

   * 任务列表或报告
   * 时间表
   * 工作负载均衡器

  ![](assets/update-percent-complete-in-task-summary-highlighted.png)

  有关详细信息，请参阅[摘要概述](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)

* **主页**：您可以从“主页”区域的“摘要”面板或“我的工作”小组件更新任务或问题的完成百分比。

有关信息，请参阅[新主页入门](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md)。

## 有关更新任务完成百分比的注意事项

* 当您将任务标记为100%完成时，任务状态将更新为“完成”。
* 父任务存在以下方案：
   * 当项目的“摘要完成模式”设置为“自动”并且子任务未完成时，不能将父任务的完成百分比更新为100%。
   * 当项目的“摘要完成模式”设置为“手动”并且子任务已完成或不完成时，您可以将父任务的完成百分比更新为100%。

  有关详细信息，请参阅[编辑项目](../manage-projects/edit-projects.md)。

## 更新任务的完成百分比

1. 转到Workfront中的以下任意区域：

   * 任务列表
   * 项目列表并应用里程碑视图
   * 通过访问任务页面执行任务
1. 找到要更新其完成百分比的任务的&#x200B;**完成百分比**&#x200B;字段。

   >[!TIP]
   >
   >  完成百分比字段始终显示在摘要面板的顶部。


1. 单击&#x200B;**完成百分比**&#x200B;字段并键入一个介于0和100之间的数字

   或

   单击并拖动&#x200B;**完成百分比**&#x200B;栏至必要的数字，以指示您完成了多少任务（如果可用）。

   >[!NOTE]
   >
   >当您指示100%的任务已完成时，任务的状态也会更新为“完成”。


1. 在键盘中按Enter键以保存完成百分比。

项目的完成百分比也会自动更新。

