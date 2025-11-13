---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 管理任务的用户或角色分配百分比
description: 分配百分比表示已分配资源在一天内计划处理一项任务的时间量。 它是任务整个持续时间中资源分配的工作日百分比（根据用户或项目计划）。
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 1f9a0e6064f83c6f0947e3c7ef596e96c934a687
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 1%

---

# 管理任务的用户或角色分配百分比

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->


分配百分比表示已分配资源在一天内计划处理一项任务的时间量。 它是任务整个持续时间中资源分配的工作日百分比（根据用户或项目计划）。

在任务中进行高级分配时，您可以修改分配百分比。

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
   <p>编辑权限可在使用旧体验编辑任务时，在编辑任务框中更新分配百分比。 在新版Experience中编辑任务时，您无法再在“编辑”任务框中管理分配百分比。</p> <p>有关信息，请参阅<a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">编辑任务</a>。</p></td>
  </tr>
 </tbody>
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
Take this piece out of the table above when we remove the new experience/ after production release in the task box: 

<p>Edit permissions to update allocation percentage in the Edit Task box when editing tasks using the old experience. <span class="preview">You can no longer manage allocation percentage in the Edit task box when editing tasks in the new experience.</span></p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a></p>.
-->

## 有关修改任务的百分比分配的注意事项

* 默认情况下，分配给用户的任务时间比例相同。
* 仅当任务的持续时间类型为计算的工作或投入比导向时，您才可以手动修改分配给任务的用户和工作角色的分配百分比。

  有关信息，请参阅[任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

* 您无法修改分配给任务的团队的百分比分配。
* 您无法修改分配给问题的用户和工作角色的百分比分配。

## 修改任务的用户或角色百分比分配

1. 转到要为其更改百分比分配的资源的任务。
1. 单击任务标题中的&#x200B;**任务**&#x200B;区域，然后单击&#x200B;**高级**。

1. 确保任务的&#x200B;**持续时间类型**&#x200B;是以下类型之一：

   * 计算的工作量
   * 投入比导向

   >[!TIP]
   >
   >* 对于已计算的分配持续时间类型，Workfront使用以下公式计算每个被分配人的分配百分比： `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`。
   >* 对于简单持续时间类型，您可以估计分配给每个资源的小时数，而不是分配百分比。

1. 修改每个任务被分派人的&#x200B;**分派工作**&#x200B;字段。

   您只能修改用户和工作角色分配的分配百分比。

   您无法修改分配给任务的团队的分配百分比。

   ![修改分配百分比](assets/advanced-assignments-allocation-percentage.png)

1. 单击&#x200B;**保存**。
