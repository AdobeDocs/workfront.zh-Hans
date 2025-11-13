---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 在任务中管理用户和角色分配小时数
description: 将用户或角色分配给任务时，会为其分配特定小时数的工作以完成任务。 当任务持续时间类型为简单时，您可以手动修改每个用户或工作角色分配给任务的小时数。
author: Lisa
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: 1f9a0e6064f83c6f0947e3c7ef596e96c934a687
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 在任务中管理用户和角色分配小时数

<!--Audited: 10/2025-->

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->


<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

分配小时数表示已分配资源在任务中计划工作的总时间。 小时表示在任务的整个持续时间内，用户在某个给定的日期或工作日、周或月上分配的时间。

在任务中进行高级分配时，您可以修改分配小时数。

>[!NOTE]
>
>在分配用户进行工作时，其根据时间表的可用性会影响任务和问题的计划和预计日期。 有关计划的信息，请参阅[创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td> <p>标准</p>
   <p>工作或更高</p>
   </td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>编辑任务访问权限</td> 
  </tr> 
  <tr> 
   <td>对象权限</td>
   <td><p>为任务分配或更高权限</p>
   <p>编辑权限可在使用旧体验编辑任务时，在“编辑任务”框中更新分配小时数。 在新版Experience中编辑任务时，您无法再在“编辑”任务框中管理分配小时数。</p> <p>有关信息，请参阅<a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">编辑任务</a>。</p></td>
  </tr>
 </tbody>
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Take this piece out of the table above when we remove the new experience/ after production release in the task box: 

<p>Edit permissions to update allocation hours in the Edit Task box when editing tasks using the old experience. <span class="preview">You can no longer manage allocation hours in the Edit task box when editing tasks in the new experience.</span></p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a></p>.-->


## 修改任务的分配小时数的注意事项

>[!IMPORTANT]
>
>在手动修改任务的每个分配的分配后，任务的已计划小时数可能会相应地更新。 有关详细信息，请参阅文章[计划小时概述](../../../manage-work/tasks/task-information/planned-hours.md#update)中的[管理用户分配时更新任务计划小时数](../../../manage-work/tasks/task-information/planned-hours.md)部分。

* 分配给分配给任务的各个资源的总小时数表示任务的计划小时数。
* 如果任务分配了用户或角色，则分配给用户或角色的小时数与任务的计划小时数匹配。
* 如果任务持续时间类型为“简单”，则在进行多个分配时，每个用户或工作角色将获得相等的小时数，以处理任务。 有关更多信息，请参阅以下文章：

   * [任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [持续时间类型概述：简单](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* 当任务具有简单持续时间类型时，您可以手动更改每个用户或工作角色的分配小时数，以指示某些任务分配人可能比其他任务分配人有更多的时间处理任务。
* 您无法修改分配给分配给任务的团队的小时数。
* 您无法手动修改问题的用户或工作角色分配。
* 您还可以使用工作负载均衡器管理每日、每周或每月分配给任务或问题的用户。 有关详细信息，请参阅[在工作负载均衡器](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)中管理用户分配。

## 修改任务的用户或角色分配小时数

1. 转到您要为其更改分配小时数的任务。
1. 单击任务标题中的&#x200B;**任务**&#x200B;区域，然后单击&#x200B;**高级**。
1. 确保任务的&#x200B;**持续时间类型**&#x200B;是&#x200B;**简单**。
1. 修改每个任务被分派人的&#x200B;**分派工作**&#x200B;字段。 这些是整个任务持续时间内此任务的每个分配的总体分配。 这也可能更新任务的整体&#x200B;**计划小时数**。

   ![修改分配](assets/advanced-assignments-duration-type-allocations.png)

1. 单击&#x200B;**保存**。
