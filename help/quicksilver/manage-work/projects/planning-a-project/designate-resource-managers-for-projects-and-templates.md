---
product-area: projects;templates
navigation-topic: plan-a-project
title: 为项目或模板指定资源经理
description: 您可以为项目指定资源管理器，以指明谁负责管理项目的资源。
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# 为项目或模板指定资源经理

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

您可以为项目指定资源管理器，以指明谁负责管理项目的资源。 这是信息字段，未连接到任何资源管理工具。

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

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p> 
   <p>规划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目和模板的访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目或模板的权限</p>

</td> 
  </tr> 
 </tbody> 
</table>

有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

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
   <td> <p>Plan </p> </td> 
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
</table>-->

## 关于资源管理器的注意事项

>[!NOTE]
>
>资源管理器不是工作角色；它是可在项目或模板中手动更新的字段。

* 您最多可以指定30个用户作为单个项目或模板的资源经理。

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Workload Balancer overview](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* 不能将团队或组指定为资源经理。 您只能将用户指定为资源管理器。

* 在项目或模板中指定为资源管理员的用户不会自动成为项目团队的一部分。

  有关项目团队的信息，请参阅[管理项目团队](../../../manage-work/projects/planning-a-project/manage-project-team.md)。

* 可以为项目或项目模板指定资源管理器。 在项目模板上指定资源管理器时，在该模板上指定为资源管理器的任何用户都会自动成为使用该模板创建的任何项目的资源管理器。
* 您可以在以下区域查看Resource Manager字段：

   * 在编辑项目时，如本文所述。
   * 在编辑模板时，如本文所述。
   * 构建项目或模板报表时。 有关生成报表的信息，请参阅[创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
   * 创建或自定义列表的项目或模板视图时。 有关详细信息，请参阅Adobe Workfront中的[视图概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

* 通过将资源管理器字段添加到列表或项目的视图中，并使用内联编辑编辑编辑此字段，可以快速在多个项目或模板中添加或删除资源管理器。

## 指定项目的资源经理

1. 执行以下任一操作：

   * 要将资源管理器添加到单个项目，请转到要指定一个或多个资源管理器的项目，然后单击项目名称旁边的&#x200B;**更多菜单**，然后&#x200B;**编辑。**

   * 要同时将资源管理器添加到多个项目，请导航到项目列表，选择要指定一个或多个资源管理器的项目，然后单击&#x200B;**编辑**。

     不会从正在编辑的项目中删除现有资源管理器；通过这种方式添加的任何用户都将添加为项目上的资源管理器，以及任何现有资源管理器。

   * 要向新项目添加资源管理器，请开始创建新项目。

     有关创建项目的信息，请参阅[创建项目](../../../manage-work/projects/create-projects/create-project.md)。

1. 在“编辑项目”对话框的&#x200B;**概述**&#x200B;部分中，单击&#x200B;**资源管理器**&#x200B;字段。
1. 开始键入要作为项目资源管理器添加的用户名称，然后在列表中出现该名称时单击该名称。

   重复此步骤为该项目添加多个资源管理器。

1. 单击&#x200B;**保存更改**。

## 为模板指定资源管理器

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)。

1. 单击&#x200B;**模板**。

1. 执行以下任一操作：

   * 要将资源管理器添加到单个模板，请转到要指定一个或多个资源管理器的模板，然后单击模板名称旁边的&#x200B;**更多菜单**，然后&#x200B;**编辑。**

   * 要同时向多个模板添加资源管理器，请转到模板列表并选择要指定一个或多个资源管理器的模板，然后单击&#x200B;**编辑**。

     不会从正在编辑的模板中删除现有资源管理器；通过这种方式添加的任何用户都将作为现有资源管理器之外的模板上的资源管理器。

   * 要将资源管理器添加到新模板，请单击“新建模板”****，再单击模板名称旁边的&#x200B;**“更多”菜单**，然后单击&#x200B;**“编辑”**。

1. 在&#x200B;**概述**&#x200B;部分中，单击&#x200B;**资源管理器**&#x200B;字段。
1. 开始键入要作为模板的资源管理器添加的用户名，然后在名称出现在列表中时单击该名称。

   重复此步骤，向模板中添加多个资源管理器。

1. 单击&#x200B;**保存更改**。
