---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 使用工作负载平衡器手动分配工作
description: 您可以使用Adobe Workfront工作负载平衡器手动为用户分配工作项。
author: Alina
feature: Resource Management
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 2%

---

# 使用工作负载平衡器手动分配工作

您可以使用Adobe Workfront工作负载平衡器手动为用户分配工作项。

有关使用工作负载平衡器将工作分配给用户的一般信息，请参阅 [工作负载平衡器中分配工作的概述](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

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
   <td> <p>在为团队或在“资源”区域使用工作负载平衡器时进行计划 </p>
   <p>使用项目的负载平衡器时工作 </p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对以下项的访问权限：</p> 
    <ul> 
     <li> <p>资源管理</p> </li> 
     <li> <p>项目</p> </li> 
     <li> <p>任务</p> </li> 
     <li> <p>问题</p> </li> 
    </ul> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>对包含“进行分配”的项目、任务和问题具有或更高的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 在工作负载平衡器中手动分配工作

您可以分配尚未分配给用户的工作项，或重新分配已分配给负载平衡器中用户的项。

1. 转到要分配工作的工作负载平衡器。

   您可以在“资源”区域、项目或团队级别使用负载平衡器将工作分配给用户。 有关工作负载平衡器在Workfront中的位置的详细信息，请参阅 [找到工作负载平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. （可选）转到 **未分配的工作** 区域，并应用过滤器以查看任务或问题

   或

   转到 **分配的工作** 区域并展开用户的名称，以查看分配给他们的工作项目（如果要重新分配他们的项目）。

1. 单击 **“更多”菜单** ![](assets/qs-more-menu.png) 在工作项名称的左侧，然后单击 **将其分配给**.

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >您还可以使用以下快捷键来分配任务或问题：
   >
   >* 在Windows中：按住Ctrl并单击任务或问题栏。
   >* 在Mac:按住CMD并单击任务或问题栏。


1. 执行下列操作之一：

   * 开始键入要在 **搜索人员、角色或团队** 字段中，当其显示在列表中时将其选中，然后单击 **保存**.
   >[!TIP]
   >
   >添加用户时，请注意头像、用户的主要角色及其电子邮件地址，以区分名称相同的用户。 用户必须至少与一个作业角色关联，才能在您添加时查看该角色。

   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > 如果您的Workfront或组管理员在您的环境中启用了委派，请使用“分配”选项卡将用户分配到该任务或问题。 使用“委派”选项卡可查看已委派到工作项的用户。 有关委派工作的信息，请参阅 [管理任务和问题委派](../../manage-work/delegate-work/how-to-delegate-work.md).


   这会将工作项分配或重新分配给指定的受分配者。

   如果您仅将项目分配给团队或职务角色，则该项目仅在“未分配工作”区域中显示。 必须向用户分配工作项，以便在工作负载平衡器的“已分配的工作”区域中显示它们。

   >[!TIP]
   >
   >您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
   >
   >
   >如果在停用用户、作业角色或团队之前已分配它们，则它们仍会被分配到工作项。 在这种情况下，我们建议执行以下操作：
   >
   >   
   >   
   >   * 将工作项重新分配给活动资源。
   >   * 将已停用团队中的用户与活动团队相关联，并将工作项重新分配给活动团队。


   * 单击 **高级** 以访问高级分配。

      有关进行高级分配的详细信息，请参阅 [创建高级分配](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).


1. （可选）单击 **显示分配图标** ![](assets/show-allocations-icon-small.png)，然后单击 **“更多”菜单** ![](assets/qs-more-menu.png) > **编辑分配**.

   或

   双击每日或每周分配，以修改用户被分配到工作项的时间。

   有关在负载平衡器中修改用户分配的信息，请参阅文章中的“修改用户分配”部分 [在工作负载平衡器中管理用户分配](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   有关使用工作负载平衡器从工作项中删除分配的信息，请参阅 [在负载平衡器中取消分配工作](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
