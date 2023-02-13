---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 管理任务的用户或角色分配百分比
description: 分配百分比表示分配的资源计划在一天内处理任务的时间。 它是在整个任务期间分配资源的工作日的百分比（根据用户或项目计划）。
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 1%

---

# 管理任务的用户或角色分配百分比

分配百分比表示分配的资源计划在一天内处理任务的时间。 它是在整个任务期间分配资源的工作日的百分比（根据用户或项目计划）。

>[!NOTE]
>
>在将用户分配到工作时，根据其计划确定其可用性会影响任务和问题的计划日期和预计日期。 有关计划的信息，请参阅 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

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
   <td> <p>为任务提供或更高权限</p> <p>在“编辑任务”框中编辑用于更新分配百分比的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 有关修改任务百分比分配的注意事项

* 默认情况下，用户在分配给他们的任务的时间中所占的百分比相等。
* 仅当任务的“持续时间类型”为“计算工作”或“工作驱动”时，您才能手动修改分配给任务的用户和作业角色的分配百分比。

   有关信息，请参阅 [任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* 您无法修改分配给任务的团队的百分比分配。
* 您无法修改分配给问题的用户和作业角色的百分比分配。

## 修改任务的用户或角色百分比分配

1. 转到要更改其资源百分比分配的任务。
1. 单击 **更多** 菜单 ![](assets/qs-more-icon-on-an-object.png) 在任务名称旁边，单击 **编辑**.

   或

   单击 **分配** 区域，然后单击 **高级**.

1. 确保 **持续时间类型** 任务的以下任务之一：

   * 计算的工作量
   * 投入比导向

   >[!TIP]
   >
   >* 对于计算的分配持续时间类型，Workfront使用以下公式计算每个受分配人的分配百分比： `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* 对于简单持续时间类型，您可以估计分配给每个资源的小时数，而不是分配百分比。


1. 单击 **分配**，然后修改 **分配** 每个任务被分派人。

   您只能修改用户和职务角色分配的分配百分比。

   您无法修改分配给任务的团队的分配百分比。

   ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

1. 单击&#x200B;**保存**。
