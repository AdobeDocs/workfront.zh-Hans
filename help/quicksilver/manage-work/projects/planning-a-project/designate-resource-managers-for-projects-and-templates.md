---
product-area: projects;templates
navigation-topic: plan-a-project
title: 为项目或模板指定资源管理器
description: 您可以为项目指定资源管理器，以指明谁负责管理项目上的资源。
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# 为项目或模板指定资源管理器

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

您可以为项目指定资源管理器，以指明谁负责管理项目上的资源。 这是一个信息性字段，它未与任何资源管理工具连接。

<!-- drafted for res scheduling deprecation blurb for preview release
Designating Resource Managers for a project is a prerequisite for using the Scheduling tools in Adobe Workfront, in the Production environment.
  
>[!CAUTION]  
>  
>  
> <span class="preview">Some of the information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span>  
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span>  
>  
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../../resource-mgmt/workload-balancer/workload-balancer.md).</span>  
>  
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

## 访问要求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Templates</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project or template</p> 
   
   <p><b>NOTE</b>
   
   Users who are added as Resource Managers to a project or a template immediately gain Manage permissions on the project or the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目和模板的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目或模板的权限</p>

<p><b>注释</b>

作为资源管理器添加到项目或模板的用户会立即获得对项目或模板的管理权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td>
</tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 关于资源管理器的考虑

>[!NOTE]
>
>资源管理器不是作业角色；它是项目或模板上可用的字段，您可以手动更新该字段。

* 您最多可以为单个项目或模板指定30个用户作为资源管理器。

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Overview of the Workload Balancer](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* 不能将团队或组指定为资源管理器。 您只能将用户指定为资源管理器。

* 在项目或模板中指定为资源管理员的用户不会自动成为项目团队的一部分。

   有关项目团队的信息，请参阅 [管理项目团队](../../../manage-work/projects/planning-a-project/manage-project-team.md).

* 您可以为项目或项目模板指定资源管理器。 在项目模板上指定“资源管理器”时，在模板上指定为“资源管理器”的任何用户都会自动成为使用该模板创建的任何项目上的“资源管理器”。
* 您可以在以下区域中查看“资源管理器”字段：

   * 编辑项目时（如本文所述）。
   * 编辑模板时，如本文所述。
   * 构建项目或模板报告时。 有关构建报表的信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
   * 创建或自定义列表的项目或模板视图时。 有关更多信息，请参阅 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* 您可以快速在多个项目或模板上添加或删除资源管理器，方法是：将“资源管理器”字段添加到列表或项目的视图，然后使用内嵌编辑功能编辑此字段。

## 为项目指定资源管理器

1. 执行以下任一操作：

   * 要将“资源管理器”添加到单个项目，请转到要指定一个或多个资源管理器的项目，然后单击 **“更多”菜单** 项目名称旁边，然后 **编辑。**

   * 要同时将资源管理器添加到多个项目，请导航到项目列表，选择要指定一个或多个资源管理器的项目，然后单击 **编辑**.

      不会从您正在编辑的项目中删除现有资源管理器；通过这种方式添加的任何用户，除了任何现有的资源管理器之外，还会作为资源管理器添加到项目中。

   * 要将资源管理器添加到新项目，请开始创建新项目。

      有关创建项目的信息，请参阅 [创建项目](../../../manage-work/projects/create-projects/create-project.md).

1. 在 **概述** ，单击 **资源管理器** 字段。
1. 开始键入要作为项目资源管理器添加的用户的名称，然后在该名称显示在列表中时单击该名称。

   重复此步骤为项目添加多个资源管理器。

1. 单击 **保存更改**.

## 为模板指定资源管理器

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 **模板**.

1. 执行以下任一操作：

   * 要将资源管理器添加到单个模板，请转到要在其中指定一个或多个资源管理器的模板，然后单击 **“更多”菜单** 在模板名称旁边， **编辑。**

   * 要同时将资源管理器添加到多个模板，请转到模板列表，选择要在其中指定一个或多个资源管理器的模板，然后单击 **编辑**.

      不会从正在编辑的模板中删除现有资源管理器；通过这种方式添加的任何用户，除了任何现有的资源管理器之外，都将作为资源管理器添加到模板中。

   * 要将资源管理器添加到新模板，请单击 **新模板**，然后单击 **“更多”菜单** 在模板名称旁边， **编辑。**

1. 在 **概述** 中，单击 **资源管理器** 字段。
1. 开始键入要作为模板资源管理器添加的用户的名称，然后在该名称显示在列表中时单击该名称。

   重复此步骤以向模板添加多个资源管理器。

1. 单击 **保存更改**.
