---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 使用工作负载均衡器手动分配工作
description: 您可以使用Adobe Workfront工作负载均衡器手动将工作项分配给用户。
author: Alina
feature: Resource Management
role: User
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 1%

---

# 使用工作负载均衡器手动分配工作

您可以使用Adobe Workfront工作负载均衡器手动将工作项分配给用户。

有关使用工作负载均衡器将工作分配给用户的一般信息，请参阅 [在工作负载均衡器中分配工作概述](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>规划，在资源区中使用工作负载均衡器时</p>
   <p>工作，使用团队或项目的工作负载均衡器时</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对以下内容的访问权限：</p> 
    <ul> 
     <li> <p>资源管理</p> </li> 
     <li> <p>项目</p> </li> 
     <li> <p>任务</p> </li> 
     <li> <p>问题</p> </li> 
    </ul> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改您的访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>包含分配的项目、任务和问题的Contribute权限或更高版本</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 在工作负载均衡器中手动分配工作

您可以在工作负载均衡器中分配尚未分配给用户的工作项，或重新分配已分配给用户的项。

1. 转到要分配工作的工作负载均衡器。

   您可以在项目或团队级别使用“资源”区域中的“工作负载均衡器”将工作分配给用户。 有关工作负载均衡器在Workfront中的位置的更多信息，请参阅 [找到工作负载均衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. （可选）转到 **未分配的工作** 区域并应用过滤器以查看任务或问题

   或

   转到 **已分派的工作** 区域并展开用户的名称以查看分配给他们的工作项（如果要重新分配其项目）。

1. 单击 **“更多”菜单** ![](assets/qs-more-menu.png) （在工作项名称左侧），然后单击 **将此项分配给**.

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >您还可以使用以下快捷方式分配任务或问题：
   >
   >* 在Windows中：按住CTRL并单击任务栏或问题栏。
   >* 在Mac中：按住CMD并单击任务栏或问题栏。

1. 执行下列操作之一：

   * 开始键入要分配给项目的用户、工作角色或团队的名称 **搜索人员、角色或团队** 字段，将其选中并在列表中显示时，然后单击 **保存**.

   >[!TIP]
   >
   >添加用户时，请注意头像、用户的主要角色及其电子邮件地址，以区分具有相同名称的用户。
   >
   >用户必须与至少一个工作角色关联，才能在添加时查看该角色。
   >
   > 您必须在访问级别中启用“查看联系人信息”设置，用户才能查看用户的电子邮件。 有关信息，请参阅 [授予用户访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > 如果您的Workfront或组管理员在环境中启用了委托，请使用“工作总揽”选项卡将用户分配给任务或问题。 使用“委托”选项卡可查看被委托给工作项目的用户。 有关委派工作的信息，请参阅 [管理任务和问题委派](../../manage-work/delegate-work/how-to-delegate-work.md).


   这会将工作项指派或重新指派给指定的被分派人。

   如果将项目仅分配给团队或工作角色，则该项目仅显示在“未分配的工作”区域中。 您必须将工作项分配给用户，才能在工作负载均衡器的已分配工作区域显示它们。

   >[!TIP]
   >
   >您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
   >
   >
   >如果在停用用户、工作角色或团队之前分配了用户、工作角色或团队，则他们仍会分配到工作项。 在这种情况下，我们建议执行以下操作：
   >
   >   
   >   
   >   * 将工作项重新分配给有效资源。
   >   * 将已停用团队中的用户与活动团队相关联，并将工作项重新分配给活动团队。
   >   
   >

   * 单击 **高级** 以访问高级分配。

     有关进行高级分配的更多信息，请参阅 [创建高级分配](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. （可选）单击 **显示分派图标** ![](assets/show-allocations-icon-small.png)，然后单击 **“更多”菜单** ![](assets/qs-more-menu.png) > **编辑分派项**.

   或

   双击每日或每周分配，以修改将用户分配给工作项的时间量。

   有关在工作负载均衡器中修改用户分配的信息，请参阅文章中的“修改用户分配”部分 [在工作负载均衡器中管理用户分配](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   有关使用工作负载均衡器从工作项中删除分配的信息，请参阅 [在工作负载均衡器中取消分配工作](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
