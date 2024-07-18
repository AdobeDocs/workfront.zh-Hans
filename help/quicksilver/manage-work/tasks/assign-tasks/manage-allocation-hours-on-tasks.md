---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 在任务中管理用户和角色分配小时数
description: 将用户或角色分配给任务时，会为其分配特定小时数的工作以完成任务。 当任务持续时间类型为简单时，您可以手动修改每个用户或工作角色分配给任务的小时数。
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: dd015fc356f65cc3d00a1c88ca0a8f2268283606
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 0%

---

# 在任务中管理用户和角色分配小时数

将用户或角色分配给任务时，会为其分配特定小时数的工作以完成任务。 当任务持续时间类型为简单时，您可以手动修改每个用户或工作角色分配给任务的小时数。

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
   <td> <p>Contribute或对该任务的更高权限</p> <p>在“编辑任务”框中编辑更新分配小时数的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 修改任务的分配小时数的注意事项

>[!IMPORTANT]
>
>在手动修改任务的每个分配的分配后，任务的已计划小时数可能会相应地更新。 有关详细信息，请参阅文章[计划小时概述](../../../manage-work/tasks/task-information/planned-hours.md)中的[管理用户分配时更新任务计划小时数](../../../manage-work/tasks/task-information/planned-hours.md#update)部分。

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
1. 单击任务名称旁边的&#x200B;**更多**&#x200B;菜单![](assets/qs-more-icon-on-an-object.png)，然后单击&#x200B;**编辑**，然后单击&#x200B;**分配**。

   或

   单击任务标题中的&#x200B;**任务**&#x200B;区域，然后单击&#x200B;**高级**。

1. 确保任务的&#x200B;**持续时间类型**&#x200B;是&#x200B;**简单**。
1. 修改每个任务被分派人的&#x200B;**分派项**。 这些是整个任务持续时间内此任务的每个分配的总体分配。 这也可能更新任务的总体计划小时数。

   ![修改分配](assets/advanced-assignments-duration-type-allocations.png)

1. 单击&#x200B;**保存**。
