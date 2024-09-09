---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 通过拖放在工作负载均衡器中分配工作
description: 您可以通过将工作项拖放到正确用户，使用Adobe Workfront工作负载均衡器分配工作项。
author: Lisa
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 0%

---

# 通过拖放在工作负载均衡器中分配工作

您可以通过将工作项拖放到正确用户，使用Adobe Workfront工作负载均衡器分配工作项。

有关使用工作负载均衡器将工作分配给用户的一般信息，请参阅[在工作负载均衡器中分配工作的概述](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)。

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
       <p>当前：计划，用于在“资源”区域的工作负载均衡器中分配工作；</br>
       工作，用于在团队或项目的工作负载均衡器中分配工作</p></td>
  </tr>
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对以下内容的访问权限：</p> 
    <ul> 
     <li>资源管理</li> 
     <li>项目</li> 
     <li>任务</li> 
     <li>问题</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>Contribute对项目、任务和问题（包括制定工作）的权限或更高</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 通过拖放方式分配项目

您可以将未分配工作区域中的项目分配给用户，也可以将已分配的项目重新分配给已分配工作区域中的另一个用户。

1. 转到要分配工作的工作负载均衡器。

   您可以在项目或团队级别使用“资源”区域的工作负载均衡器将工作分配给用户。 有关工作负载均衡器在Workfront中的位置的更多信息，请参阅[找到工作负载均衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)。

1. （可选）转到&#x200B;**未分配的工作**&#x200B;区域并应用筛选器以查看未分配给用户的任务和问题

   或

   转到&#x200B;**已分配的工作**&#x200B;区域并展开用户的名称以查看分配给他们的工作项（如果要重新分配其项目）。

1. （视情况而定）在项目的工作负载均衡器中，单击&#x200B;**显示所有用户**&#x200B;图标![](assets/show-all-users-icon-project-workload-balancer.png)以显示所有Workfront用户。

   这会显示您有权查看的所有用户。

   同时属于项目团队并已分配到项目项的用户在“已分配工作”区域的名称右侧具有项目图标。

   ![](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)


   >[!TIP]
   >
   >* 显示所有用户选项仅在项目的工作负载均衡器中可用。
   >* 使用筛选器可仅显示对您重要的用户。 例如，使用筛选器可仅显示团队或组中的用户。



1. 单击工作项指示计划或预计时间线的栏，并将其拖动到&#x200B;**已分配**&#x200B;区域中的用户名称上。

   将鼠标悬停在其上以将工作项放置到的用户会突出显示。

   >[!TIP]
   >
   >您悬停在该工作项上的用户的计划小时数将实时更新为每日计划小时数，以指示添加新项目可能会对其总体分配产生的影响。

   ![](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. 准备就绪后，将所选工作项拖放到与已分配区域中的用户名相同的行中。 已分配项目，并且使用工作项目中的新小时数为用户更新分配的计划小时数。

   如果将该项目分配给用户无法完成的工作角色，则该项目将显示在“已分配的工作”区域中该用户名称的下面，并且该项目还会留在“未分配的工作”区域中，以指示与其关联的工作角色尚未被用户替换。

   >[!TIP]
   >
   >* 如果在“设置”区域中启用了“按项目分组” ，则分配的任务将显示在相应的项目下。 如果禁用该设置，则分配的任务将显示在用户区域中。
   >
   >
   >     此项根据工作负载均衡器标准显示以排序工作项。 有关详细信息，请参阅[导航工作负载均衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。
   >
   >
   >* 如果启用了在项目的工作负载均衡器中显示所有用户，并将项目分配给之前未分配给项目项目的用户，则该用户将会添加到项目团队。 有关详细信息，请参阅[管理项目团队](../../manage-work/projects/planning-a-project/manage-project-team.md)。


1. （可选）单击已分配工作区域中的用户名称下的工作项栏，并将其拖放到未分配工作区域上以取消分配。 该项目已从用户取消分配，但仍可能分配给工作角色，在此情况下，该项目会显示在“未分配的工作”区域中。 如果将项目分配给另一个用户，该项目将保留在“已分配工作”区域中，且位于仍被分配的用户名下。
1. （可选）单击&#x200B;**显示分派图标** ![](assets/show-allocations-icon-small.png)，然后单击&#x200B;**更多菜单** ![](assets/qs-more-menu.png) > **编辑分派**。

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   或

   双击每日或每周分配，以修改将用户分配给工作项的时间量。

   有关在工作负载均衡器中修改用户分配的信息，请参阅在工作负载均衡器](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)中管理用户分配一文[中的“修改用户分配”一节。

   有关使用工作负载均衡器从工作项中删除分配的信息，请参阅工作负载均衡器中的[取消分配工作](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md)。

