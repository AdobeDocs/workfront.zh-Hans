---
product-area: projects
navigation-topic: plan-a-project
title: 在角色分配面板中查看项目计划小时数
description: 您可以在项目的“角色分配”面板中查看分配给项目中工作项的所有工作角色的角色分配。
author: Alina, Lisa
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 1%

---

# 在角色分配面板中查看项目计划小时数

您可以在项目的“角色分配”面板中查看分配给项目中工作项的所有工作角色的角色分配。

>[!NOTE]
>
>本文指的是查看与项目中的任务和问题相关的工作角色，以及它们在项目的“角色分配”面板中分配的已计划小时数。 有关在使用Adobe Workfront Scenario Planner时通过“角色分配”面板将计划小时数与计划小时数进行协调的信息，请参阅以下内容：
>
>* [在任务列表中显示项目和计划的角色分配](../../../scenario-planner/show-role-allocation-task-list-nwe.md)
>* [在工作负载均衡器中显示项目和计划的角色分配](../../../scenario-planner/show-role-allocation-workload-balancer.md)
>
>  您必须具有Scenario Planner许可证才能在“角色分配”面板中查看计划小时数。 有关Scenario Planner的信息，请参阅[Scenario Planner入门](../../../scenario-planner/get-started-with-scenario-planning.md)。
>
>如果您的公司以前购买过Adobe Scenario Planner，则它已被保留。 Scenario Planner不再可供购买。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>Adobe Workfront Ultimate</p>
   <p>Adobe工作流程Ultimate</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>浅色或更高</p>
   <p>审核或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看项目或授予更高的项目访问权限</p>
   <p>编辑对Scenario Planner的访问权限以更新计划小时</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目或更高权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

able style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 先决条件

您必须具备以下条件：

* 分配给工作角色或与工作角色关联的用户的任务或问题。

  >[!TIP]
  >
  >如果任务或问题被取消分配、分配给团队或分配给没有工作角色的用户，则项目在“角色分配”面板中的计划小时数为零。

* 持续时间大于零的任务和问题。

## 在角色分配面板中查看项目计划小时数

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**项目**。
1. 单击项目名称以访问它。 这将打开“项目”页面。
1. 在左侧面板中单击以下选项之一：

   * **任务**
   * **工作负载平衡器**

1. 单击&#x200B;**显示角色分配**&#x200B;图标![显示角色分配图标](assets/show-role-allocation-icon.png)。

   此时将显示“角色分配”面板。

   ![仅具有计划小时数的角色分配面板](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. 查看&#x200B;**角色分配**&#x200B;面板中的以下信息：

   | 字段 | 描述 |
   |---|---|
   | **工作角色** | 分配给项目任务和问题的工作角色。 这些角色可以是直接分配给任务和问题的工作角色，也可以是与分配给项目任务和问题的用户相关联的工作角色。 |
   | **计划小时数** | 任务和问题中的已计划小时数总数，这些任务和问题分配给与项目中的工作角色相关联的工作角色或用户。 |

