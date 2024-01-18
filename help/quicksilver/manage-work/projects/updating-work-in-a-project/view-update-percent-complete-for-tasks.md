---
product-area: projects
navigation-topic: update-work-in-a-project
title: 查看和更新任务的完成百分比
description: 您可以更新任务的完成百分比，以指明完成任务的进度。
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# 查看和更新任务的完成百分比

<!--Audited:01/2024-->

您可以更新任务的完成百分比，以指明完成任务的进度。

## 访问要求

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

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## 您可以更新任务的完成百分比的区域

您可以在以下任意区域更新任务的完成百分比：

* **在任务列表中**：当显示完成百分比列时，您可以更新任务的完成百分比。\
  有关内联编辑的更多信息，请参阅 [Adobe Workfront中列表的内联编辑项目](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **在里程碑视图中**：在项目列表或项目报告中使用里程碑视图时，您可以更新任务的完成百分比。 有关更多信息，请参阅 [使用里程碑视图](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

<!--only in legacy commenting: 
* **As you update the task**:  You can update the percent complete option of a task when adding an update to the task.

  >[!IMPORTANT]
  >
  >This option displays only after you enable the Show Percent Complete option.  
  >To enable the percent complete update bar for tasks, do the following:   
  >
  >1. Go to the **Main** menu>your name>**More** icon next to your name >**Edit** > select **Show percent complete on update status**.   
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >-->

* **在任务标题中**：您可以在任务标题中更新任务的完成百分比。 有关信息，请参阅 [编辑任务](../../tasks/manage-tasks/edit-tasks.md).

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)


## 有关更新任务完成百分比的注意事项

* 当您将任务标记为100%完成时，任务状态将更新为“完成”。
* 父任务存在以下方案：
   * 当项目的“摘要完成模式”设置为“自动”并且子任务未完成时，不能将父任务的完成百分比更新为100%。
   * 当项目的“摘要完成模式”设置为“手动”并且子任务已完成或不完成时，您可以将父任务的完成百分比更新为100%。

  有关更多信息，请参阅 [编辑项目](../manage-projects/edit-projects.md).

## 更新任务的完成百分比

1. 转到Workfront中的以下任意区域：

   * 任务列表
   * 项目列表并应用里程碑视图
   * 通过访问任务页面执行任务
1. 找到 **完成百分比** 要更新其完成百分比的任务的字段。
1. 单击完成百分比字段，然后键入介于0和100之间的数字

   或

   单击并拖动 **完成百分比** 栏中显示的必要数字，以指示您完成了多少任务（如果可用）。

   >[!NOTE]
   >
   >当您指示100%的任务已完成时，任务的状态也会更新为“完成”。


1. 在键盘中按Enter键以保存完成百分比。

项目的完成百分比也会自动更新。

