---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 在工作负载均衡器中取消分配工作
description: 您可以在Adobe Workfront工作负载均衡器的“已分配工作”区域将用户取消分配，或将其重新分配给其他用户、角色或团队。
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 2%

---

# 在工作负载均衡器中取消分配工作

您可以在Adobe Workfront工作负载均衡器的“已分配工作”区域将用户取消分配，或将其重新分配给其他用户、角色或团队。

您可以通过手动、拖放或批量方式从工作项中取消分配用户。 本文介绍了如何手动取消分配用户。

有关通过拖放来取消分配用户的信息，请参阅 [通过拖放在工作负载均衡器中分配工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

有关批量取消分配用户的信息，请参阅 [使用工作负载均衡器批量分配工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>在资源区域使用工作负载均衡器时进行规划</p>
   <p>工作，使用团队或项目的工作负载均衡器时</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对以下内容的访问权限：</p> 
    <ul> 
     <li> <p>资源管理</p> </li> 
     <li> <p>项目</p> </li> 
     <li> <p>任务</p> </li> 
     <li> <p>问题</p> </li> 
    </ul> <p>如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改您的访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>包含制定工作分派的项目、任务和问题的Contribute权限或更高版本</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

 

## 在工作负载均衡器中取消分配工作项

您可以从用户中取消分配项目并将它们移动到“未分配工作”区域，或将其重新分配给其他用户。

要从用户中取消分配工作项，请执行以下操作：

1. 在工作负载均衡器中，转到 **已分派工作** 区域并展开用户。
1. 执行下列操作之一：

   * 在用户的区域中查找要取消分配的项目，单击该项目，然后将其拖放到未分配区域或其他用户的区域中。
   * 单击 **更多** 图标 ![](assets/more-icon-task-list.png) 在工作项名称的右侧，单击 **将此分派至**，然后移除分配给工作项的实体的名称或输入其他名称，然后单击 **保存**.

     ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   如果项目符合未分配工作区域的筛选条件，且未分配给任何其他用户，则该项目会显示在未分配的工作区域中；如果项目分配给其他用户，则该项目会显示在用户区域中。

   有关在工作负载均衡器中过滤信息的信息，请参见 [工作负载均衡器中的过滤器信息](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
