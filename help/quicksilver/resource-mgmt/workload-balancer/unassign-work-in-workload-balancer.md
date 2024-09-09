---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 在工作负载均衡器中取消分配工作
description: 您可以在Adobe Workfront工作负载均衡器的“已分配工作”区域将用户取消分配，或将其重新分配给其他用户、角色或团队。
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 196d0aa4ed67cf564c823625515ef49d811e0e06
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 2%

---

# 在工作负载均衡器中取消分配工作

您可以在Adobe Workfront工作负载均衡器的“已分配工作”区域将用户取消分配，或将其重新分配给其他用户、角色或团队。

您可以通过手动、拖放或批量方式从工作项中取消分配用户。 本文介绍了如何手动取消分配用户。

有关通过拖放取消分配用户的信息，请参阅[通过拖放在工作负载均衡器中分配工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

有关批量取消分配用户的信息，请参阅[使用工作负载均衡器批量分配工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何 </p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：计划，在资源区域使用工作负载均衡器时；</br>
       工作，使用团队或项目的工作负载均衡器时</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对以下内容的访问权限：</p> 
    <ul> 
     <li>资源管理</li> 
     <li>项目</li> 
     <li>任务</li> 
     <li>问题</li> 
    </ul></td>
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>Contribute对项目、任务和问题（包括制定工作）的权限或更高</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在工作负载均衡器中取消分配工作项

您可以从用户中取消分配项目并将它们移动到“未分配工作”区域，或将其重新分配给其他用户。

要从用户中取消分配工作项，请执行以下操作：

1. 在工作负载均衡器中，转到&#x200B;**已分配的工作**&#x200B;区域并展开用户。
1. 执行下列操作之一：

   * 在用户的区域中查找要取消分配的项目，单击该项目，然后将其拖放到未分配区域或其他用户的区域中。
   * 单击工作项名称右侧的&#x200B;**更多**&#x200B;图标![](assets/more-icon-task-list.png)，单击&#x200B;**将此工作项分配给**，然后移除分配给该工作项的实体的名称或输入其他名称，然后单击&#x200B;**保存**。

     ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   如果项目符合未分配工作区域的筛选条件，且未分配给任何其他用户，则该项目会显示在未分配的工作区域中；如果项目分配给其他用户，则该项目会显示在用户区域中。

   有关在工作负载均衡器中过滤信息的信息，请参阅在工作负载均衡器中[过滤信息](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)。
