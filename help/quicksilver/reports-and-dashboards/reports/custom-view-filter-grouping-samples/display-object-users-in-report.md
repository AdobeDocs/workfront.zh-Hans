---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 报告或列表：显示与对象关联的用户
description: 您可以在报告或列表中显示与对象关联的用户、工作角色和团队，并在筛选器中引用它们。 您无法按用户、工作角色或与对象关联的团队进行分组。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 9abdaafb-da2c-4b5d-9117-59afa4a1e71f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 2%

---

# 报告或列表：显示与对象关联的用户

您可以在报告或列表中显示与对象关联的用户、工作角色和团队，并在筛选器中引用它们。 您无法按用户、工作角色或与对象关联的团队进行分组。

您可以按与以下对象关联的用户、工作角色或团队来显示或筛选：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">对象</td> 
   <td>关联的用户或工作角色</td> 
  </tr> 
  <tr> 
   <td role="rowheader">项目</td> 
   <td> <p>您可以在项目报告中显示所有用户及其在该项目上履行的工作角色。 您不能按项目报告中的用户或其关联的工作角色进行筛选。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">任务</td> 
   <td>您可以在任务报告中按分配给任务的所有用户、工作角色和团队进行显示和筛选。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">问题</td> 
   <td>您可以在问题报告中按分配给问题的所有用户、工作角色和团队进行显示和过滤。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">项目组合</td> 
   <td>您可以在项目报告中显示所有用户及其在该项目上履行的工作角色，并按Portfolio对该报告进行分组。 您不能按项目报告中的用户或其关联的工作角色进行筛选。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">项目群</td> 
   <td>您可以在项目报告中显示所有用户及其在该项目上履行的工作角色，并按项目群对该报告进行分组。 您不能按项目报告中的用户或其关联的工作角色进行筛选。</td> 
  </tr> 
 </tbody> 
</table>

## 显示与项目关联的所有用户和职位角色

您可以在项目列表或报告的视图中显示与项目相关联的所有用户。 这包括项目的“人员”部分中列出的所有用户。 在项目报告中将其分配给项目中的任务或问题时，您还可以查看它们关联的角色。

![包含用户和角色信息的项目](assets/project-with-user-and-role-information-report-350x100.png)

有关生成项目报告以显示项目中的所有用户及其角色的信息，请参阅[查看：具有工作角色的项目用户列表](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md)。

您无法筛选与项目筛选器中的项目关联的用户或工作角色。

## 显示分配给任务的所有用户、工作角色或团队

通过将“工作总揽”字段添加到视图，可以在任务列表或报表的视图中显示分配给任务的所有用户、角色或团队。

![任务字段](assets/assignments-field-task-view-350x124.png)

您可以通过引用任务筛选器中的以下字段，按分配给任务的用户、工作角色或团队进行筛选：

* 任务用户
* 任务角色
* 团队

![任务筛选器中的工作用户和角色](assets/assignment-users-roles-task-filter-350x334.png)

## 显示分配给问题的所有用户、工作角色或团队

您可以通过将“工作总揽”字段添加到问题列表或报告的视图，来显示分配给问题的所有用户、角色或团队。

您可以按分配给问题的用户、工作角色或团队进行筛选，方法是引用问题筛选器中的以下字段：

* 任务用户
* 任务角色
* 团队

## 显示与项目组合关联的所有用户和职位角色

您可以显示与项目组合关联的所有用户和角色，方法是在项目报表中显示它们，然后按照Portfolio对报表进行分组。

有关生成项目报告以显示项目中的所有用户及其角色的信息，请参阅[查看：具有工作角色的项目用户列表](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md)。

您无法筛选与项目组合或项目筛选器中的项目关联的用户或工作角色。

## 显示与项目群关联的所有用户和工作角色

您可以显示与项目群相关的所有用户和角色，方法是在项目群报表中显示它们，然后按项目群分组报表。

有关生成项目报告以显示项目中的所有用户及其角色的信息，请参阅[查看：具有工作角色的项目用户列表](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-project-user-list.md)。

您无法筛选与项目群或项目筛选器中的项目关联的用户或工作角色。
