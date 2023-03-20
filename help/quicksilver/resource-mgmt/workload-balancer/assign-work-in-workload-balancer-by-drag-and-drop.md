---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 通过拖放在工作负载平衡器中分配工作
description: 您可以使用Adobe Workfront工作负载平衡器将工作项拖放到正确的用户，从而分配工作项。
author: Alina
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: bbd99435bb07d68bf9058bcd3e8c6ef5d9df75a9
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 1%

---

# 通过拖放在工作负载平衡器中分配工作

<!--remove production and preview preferences at release-->

您可以使用Adobe Workfront工作负载平衡器将工作项拖放到正确的用户，从而分配工作项。

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
   <td> <p>规划，在资源区的负载平衡器中分配工作</p>
   <p>工作，在团队或项目的负载平衡器中分配工作</p>
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

## 通过拖放来分配项目

您可以将“未分配的工作”区域中的项目分配给用户，也可以将已分配的项目重新分配给“已分配的工作”区域中的其他用户。

1. 转到要分配工作的工作负载平衡器。

   您可以在“资源”区域、项目或团队级别使用负载平衡器将工作分配给用户。 有关工作负载平衡器在Workfront中的位置的详细信息，请参阅 [找到工作负载平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. （可选）转到 **未分配的工作** 区域并应用过滤器，以查看未分配给用户的任务和问题

   或

   转到 **分配的工作** 区域并展开用户的名称，以查看分配给他们的工作项目（如果要重新分配他们的项目）。

1. （视情况而定）在项目的负载平衡器中，单击 **显示所有用户** 图标 ![](assets/show-all-users-icon-project-workload-balancer.png) 以显示所有Workfront用户。

   这会显示您有权查看的所有用户。

   此外，如果用户是项目团队的一员，并且已经分配到项目中的项目，则在“已分配的工作”区域中，其名称的右侧会显示项目图标。

   ![](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)


   >[!TIP]
   >
   >* “显示所有用户”选项仅在项目的负载平衡器中可用。
   >* 使用过滤器仅显示对您而言重要的用户。 例如，使用过滤器仅显示团队或群组中的用户。




1. 单击指示计划时间轴或预计时间轴的工作项目栏，并将其拖动到 **已分配** 的上界。

   将鼠标悬停在上方以将工作项拖放到的用户会突出显示。

   >[!TIP]
   >
   >您将鼠标悬停在工作项目的每日计划小时数上的用户的计划小时数，以指示添加新项目对其整体分配的影响。

   ![](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. 准备就绪后，将选定工作项拖放到“分配区域”中与用户名称相同的行中。 系统会为用户分配物料，并且会使用工作项中的新工时来更新分配的计划工时。

   如果已将项目分配给用户无法履行的作业角色，则该项目将显示在“已分配的工作”区域中用户名称下方，并且它还保留在“未分配的工作”区域，以指明与其关联的作业角色尚未被用户替换。

   >[!TIP]
   >
   >* 如果在“设置”区域中启用了按项目分组，则分配的任务将显示在相应项目下。 如果禁用了该设置，则分配的任务将显示在用户区域中。
      >
      >
      >     项目将根据用于对工作项进行排序的负载平衡器条件显示。 有关更多信息，请参阅 [导航工作负载平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).
   >
   >
   >* 如果启用了显示项目负载平衡器中的所有用户，以及将项目分配给之前未分配给项目中项目的用户，则会将这些用户添加到项目团队。 有关更多信息，请参阅 [管理项目团队](../../manage-work/projects/planning-a-project/manage-project-team.md).



1. （可选）在“已分配的工作”区域中单击用户名称下方工作项的栏，然后将其拖动到“未分配的工作”区域上以取消分配。 该项目未从用户中分配，但仍可能被分配到作业角色，在这种情况下，它会显示在“未分配的工作”区域。 如果项目已分配给其他用户，则它将保留在“已分配的工作”区域中，并由仍被分配的用户的名称来标识。
1. （可选）单击 **显示分配图标** ![](assets/show-allocations-icon-small.png)，然后单击 **“更多”菜单** ![](assets/qs-more-menu.png) > **编辑分配**.

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   或

   双击每日或每周分配，以修改用户被分配到工作项的时间。

   有关在负载平衡器中修改用户分配的信息，请参阅文章中的“修改用户分配”部分 [在工作负载平衡器中管理用户分配](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   有关使用工作负载平衡器从工作项中删除分配的信息，请参阅 [在负载平衡器中取消分配工作](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

