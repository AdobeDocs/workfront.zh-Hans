---
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: 在“计划”区域中，不考虑角色和组成员资格，允许用户分配
description: 在“资源计划”中，只能为在用户配置文件上定义了与分配给任务或问题的角色分配相匹配的角色的用户分配分配任务。
author: Alina
feature: Resource Management
exl-id: 0f90ffde-6f07-4c3c-b963-de28b1b55dc1
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---

# 在“计划”区域中，不考虑角色和组成员资格，允许用户分配

>[!IMPORTANT]
>  
><span class="preview">自2023年1月的23.1版本开始，本文中描述的计划功能已弃用并从Adobe Workfront中删除。   </span>
>  
> <span class="preview"> 2023年初23.1版发布后不久，也将删除本文。 此时，我们建议您相应地更新任何书签。 </span>
> 
><span class="preview"> 您现在可以使用负载平衡器来计划资源的工作。 </span>
>  
> <span class="preview">有关使用工作负载平衡器计划资源的信息，请参阅一节 [工作负载平衡器](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer.</span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;***LINKED TO THE UI FROM Resource Scheduling (People> Teams>Working On>Settings>Limit Assignments to the Group Associated with the Project) - ALSO FROM THE WORKING ON TAB OF TEAMS and AT THE PROJECT STAFFING TAB TOO)</p>
<p>NOTE: Alina; broken off the original article; retitle, reformat, relink sections) </p>
</div>
-->

默认情况下，只能为在用户配置文件上定义了与分配给他们的任务或问题的角色分配相匹配的角色的用户分配分配资源。

您可以将Adobe Workfront配置为允许将任务和问题分配给任何用户，而不管该用户在其用户配置文件中定义的角色是否与分配给他们的任务或问题的角色分配相匹配。 当您将用户分配给任务或问题，并且该用户没有与任务或问题上的角色分配相匹配的角色时，将删除原始角色分配，并且角色分配将更改为您分配的用户的角色。

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>查看或更高程度地访问项目、任务和问题</p> <p><strong>注释</strong>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>为更新的项目、任务和问题提供权限或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 不论角色如何，都允许向用户分配

1. 转到多个项目、单个项目或团队的计划时间轴：

   * **对于多个项目**:  单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **资源配置>工作负载平衡器**，然后选择 **计划** 中。
   * **对于单个项目**:转到项目，单击 **工作负载平衡器** ，然后选择 **计划** 从左上角的下拉菜单中。
   * **对于团队**:单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **团队**，选择团队，单击 **工作负载平衡器** 在左侧面板中，选择 **计划** 从左上角的下拉菜单中。

1. 单击 **设置** 图标。
1. 禁用选项 **将分配限制为具有匹配角色的用户**.
1. 单击 **返回计划**.

## 允许向用户分配任何组成员资格

<!--
<p>(NOTE: Alina: **^ This section is linked to the UI in a tooltip inside the Settings of the scheduler. do not rename/ remove/ edit the tag!!) </p>
-->

默认情况下，只能向属于与项目关联的组的成员用户（这是编辑项目时定义的组）分配。

>[!IMPORTANT]
>
>此设置仅考虑与项目关联的组的成员，而不考虑该组任何子组的任何成员。

您可以将Workfront配置为允许将任务和问题分配给任何用户，而不管该用户是否是与任务或问题所在项目相关联的组的成员。

1. 转到多个项目、单个项目或团队的计划时间轴：

   * **对于多个项目**:  单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **资源配置>工作负载平衡器**，然后选择 **计划** 中。
   * **对于单个项目**:转到项目，单击 **工作负载平衡器** ，然后选择 **计划** 从左上角的下拉菜单中。
   * **对于团队**:单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **团队**，选择团队，单击 **工作负载平衡器** 在左侧面板中，选择 **计划** 从左上角的下拉菜单中。

1. 单击 **设置** 图标。
1. 禁用选项 **将分配限制为与项目关联的组**.
1. 单击 **返回计划**.

 
