---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 管理任务的用户和角色分配小时数
description: 在为任务分配用户或角色时，会将用户或角色分配到特定的小时数以完成任务。 当任务持续时间类型为“简单”时，您可以手动修改在分配给任务时每个用户或作业角色所分配的小时数。
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# 管理任务的用户和角色分配小时数

在为任务分配用户或角色时，会将用户或角色分配到特定的小时数以完成任务。 当任务持续时间类型为“简单”时，您可以手动修改在分配给任务时每个用户或作业角色所分配的小时数。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑任务访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>为任务提供或更高权限</p> <p>在“编辑任务”框中编辑用于更新分配小时数的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 修改任务分配时数的注意事项

>[!IMPORTANT]
>
>在您手动修改任务上每个分配的分配后，任务的“计划小时数”可能会相应地更新。 有关更多信息，请参阅 [管理用户分配时更新任务计划小时数](../../../manage-work/tasks/task-information/planned-hours.md#update) 在文章中 [计划时数概述](../../../manage-work/tasks/task-information/planned-hours.md).

* 分配给分配给任务的单个资源的总小时数表示任务的计划小时数。
* 如果某个任务有一个用户或角色分配，则分配给该用户或角色的小时数与任务的计划小时数相匹配。
* 在多个分配的情况下，如果任务持续时间类型为“简单”，则默认情况下，会为每个用户或任务角色分配等量的小时数来处理任务。 有关更多信息，请参阅以下文章：

   * [任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [持续时间类型概述：简单](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* 当任务具有简单持续时间类型时，您可以手动更改每个用户或作业角色的分配小时数，以指示某些任务分配者可能比其他任务拥有更多时间来处理任务。
* 您无法修改分配给分配给任务的团队的小时数。
* 您无法手动修改问题的用户或作业角色分配。
* 您还可以使用负载平衡器管理用户对任务或问题的每日、每周或每月分配。 有关更多信息，请参阅 [在工作负载平衡器中管理用户分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## 修改任务的用户或角色分配小时数

1. 转到要更改其分配小时数的任务。
1. 单击 **更多** 菜单 ![](assets/qs-more-icon-on-an-object.png) 在任务名称旁边，单击 **编辑**，则 **分配**.

   或

   单击 **分配** 区域，然后单击 **高级**.

1. 确保 **持续时间类型** 任务是 **简单**.
1. 修改 **分配** 每个任务被分派人。 这些是在整个任务期间对此任务的每个分配进行的整体分配。 这也可能会更新任务的总计划小时数。

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. 单击&#x200B;**保存**。
