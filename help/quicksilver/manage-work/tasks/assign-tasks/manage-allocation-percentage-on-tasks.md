---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 管理任务的用户或角色分配百分比
description: 分配百分比表示已分配资源在一天内计划处理一项任务的时间量。 它是任务整个持续时间中资源分配的工作日百分比（根据用户或项目计划）。
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 0d525df9beacc989ec3c1c695a7757dff0ad77b3
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 1%

---

# 管理任务的用户或角色分配百分比

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它只能在“预览”环境中用于所有客户，或者在“生产”环境中用于启用快速版本的客户。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

<span class="preview">有关当前版本的信息，请参阅[2024年第三季度版本概述](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md)。</span>

分配百分比表示已分配资源在一天内计划处理一项任务的时间量。 它是任务整个持续时间中资源分配的工作日百分比（根据用户或项目计划）。

>[!NOTE]
>
>在分配用户进行工作时，其根据时间表的可用性会影响任务和问题的计划和预计日期。 有关计划的信息，请参阅[创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑任务访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>Contribute或对该任务的更高权限</p> <p>在“编辑任务”框中编辑权限以更新分配百分比</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 有关修改任务的百分比分配的注意事项

* 默认情况下，分配给用户的任务时间比例相同。
* 仅当任务的持续时间类型为计算的工作或投入比导向时，您才可以手动修改分配给任务的用户和工作角色的分配百分比。

  有关信息，请参阅[任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

* 您无法修改分配给任务的团队的百分比分配。
* 您无法修改分配给问题的用户和工作角色的百分比分配。

## 修改任务的用户或角色百分比分配

1. 转到要为其更改百分比分配的资源的任务。
1. 单击任务名称旁边的&#x200B;**更多**&#x200B;菜单![](assets/qs-more-icon-on-an-object.png)，然后单击&#x200B;**编辑**。

   或

   单击任务标题中的&#x200B;**任务**&#x200B;区域，然后单击&#x200B;**高级**。

1. 确保任务的&#x200B;**持续时间类型**&#x200B;是以下类型之一：

   * 计算的工作量
   * 投入比导向

   >[!TIP]
   >
   >* 对于已计算的分配持续时间类型，Workfront使用以下公式计算每个被分配人的分配百分比： `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`。
   >* 对于简单持续时间类型，您可以估计分配给每个资源的小时数，而不是分配百分比。

1. 单击&#x200B;**分配**，然后修改每个任务被分配人的&#x200B;**分配**。

   您只能修改用户和工作角色分配的分配百分比。

   您无法修改分配给任务的团队的分配百分比。

   生产环境中的示例图像：
   ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

   <span class="preview">预览环境中的示例图像：</span>
   ![修改分配百分比](assets/advanced-assignments-allocation-percentage.png)

1. 单击&#x200B;**保存**。
