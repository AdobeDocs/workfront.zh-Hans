---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “报表或列表：显示与对象关联的用户
description: 您可以显示与报表或列表中的对象关联的用户、作业角色和团队，并在过滤器中引用它们。 不能按与对象关联的用户、作业角色或团队进行分组。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 9abdaafb-da2c-4b5d-9117-59afa4a1e71f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 2%

---

# 报表或列表：显示与对象关联的用户

您可以显示与报表或列表中的对象关联的用户、作业角色和团队，并在过滤器中引用它们。 不能按与对象关联的用户、作业角色或团队进行分组。

您可以按与以下对象关联的用户、作业角色或团队显示或过滤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">对象</td> 
   <td>关联的用户或作业角色</td> 
  </tr> 
  <tr> 
   <td role="rowheader">项目</td> 
   <td> <p>您可以在项目报表中显示所有用户及其在项目中履行的作业角色。 无法在项目报表中按用户或其关联的作业角色进行过滤。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">任务</td> 
   <td>您可以按任务报表中分配给任务的所有用户、作业角色和团队显示和过滤任务。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">问题</td> 
   <td>您可以按分配给问题报表中问题的所有用户、工作角色和团队显示和过滤问题。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">项目组合</td> 
   <td>您可以在项目报表中显示所有用户及其在项目中履行的职务角色，并按Portfolio对报表进行分组。 无法在项目报表中按用户或其关联的作业角色进行过滤。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">项目群</td> 
   <td>您可以在项目报表中显示所有用户及其在项目中履行的职务角色，并按项目对报表进行分组。 无法在项目报表中按用户或其关联的作业角色进行过滤。</td> 
  </tr> 
 </tbody> 
</table>

## 显示与项目关联的所有用户和作业角色

您可以在项目列表或报表的视图中显示与项目中关联的所有用户。 这包括项目“人员”部分中列出的所有用户。 在项目报表中，您还可以查看在分配给项目任务或问题时与它们关联的角色。

![](assets/project-with-user-and-role-information-report-350x100.png)

有关构建项目报告以显示项目中所有用户及其角色的信息，请参阅 [查看：具有作业角色的项目用户列表](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

您无法在项目筛选器中筛选与项目关联的用户或作业角色。

## 显示分配给任务的所有用户、工作角色或团队

通过将“分配”(Assignments)字段添加到视图，您可以在任务列表或报表的视图中显示分配给任务的所有用户、角色或团队。

![](assets/assignments-field-task-view-350x124.png)

您可以通过引用任务筛选器中的以下字段，按分配给任务的用户、作业角色或团队进行筛选：

* 任务用户
* 任务角色
* 团队

![](assets/assignment-users-roles-task-filter-350x334.png)

## 显示分配给问题的所有用户、工作角色或团队

通过将“分配”字段添加到视图，您可以在问题列表或报表的视图中显示分配给问题的所有用户、角色或团队。

您可以通过在问题筛选器中引用以下字段，按分配给问题的用户、作业角色或团队进行筛选：

* 任务用户
* 任务角色
* 团队

## 显示与组合关联的所有用户和工作角色

您可以显示与项目组合关联的所有用户和角色，方法是在项目报表中显示这些用户和角色，然后按Portfolio对报表进行分组。

有关构建项目报告以显示项目中所有用户及其角色的信息，请参阅 [查看：具有作业角色的项目用户列表](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

您无法在项目组合或项目筛选器中筛选与项目关联的用户或作业角色。

## 显示与项目关联的所有用户和工作角色

您可以显示与项目关联的所有用户和角色，方法是在项目报表中显示这些用户和角色，然后按项目对报表进行分组。

有关构建项目报告以显示项目中所有用户及其角色的信息，请参阅 [查看：具有作业角色的项目用户列表](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md).

您无法在项目或项目筛选器中筛选与项目关联的用户或作业角色。
