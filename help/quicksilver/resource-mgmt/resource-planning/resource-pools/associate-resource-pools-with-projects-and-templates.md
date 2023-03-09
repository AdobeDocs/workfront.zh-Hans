---
product-area: resource-management
navigation-topic: resource-pools
title: 将资源池与项目和模板关联
description: 资源池是用户的集合，可帮助您管理Adobe Workfront中的资源。
author: Alina
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: 23257f11b0795aa1f1e422923f6d596017c58126
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# 将资源池与项目和模板关联


<!-- drafted for bulk editing projects: keep this in yellow till this releases to ALL customers - May 1, 2023

Also - take out all the references to Preview and Prod at prod final
-->

<span class="preview">此页面上高亮显示的信息是指尚未公开发布的功能。 它仅在“预览”环境中可用。</span>


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
</div>
-->

资源池是用户的集合，可帮助您管理Adobe Workfront中的资源。

创建资源池后，您可以将其与项目或模板相关联，以便以后在项目上预算资源。

我们建议您提前创建资源池，将其与项目关联，并在项目开始之前对资源进行预算。

有关资源池的信息，请参见 [资源池概述](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

有关创建资源池的信息，请参见 [创建资源池](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业及更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对资源管理的访问权限，其中包括对管理资源池的访问权限</p> <p>编辑对项目、模板和用户的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理您与资源池关联的项目、模板和用户的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 将资源池与一个项目或模板关联

您可以使用与将资源池与项目关联相同的方式将资源池与模板关联。 本文介绍了如何将资源池与项目关联。

1. 转到项目，然后单击 **更多** 图标 ![](assets/more-icon.png)在项目名称旁边，然后单击 **编辑**.

1. 单击 **项目设置**.

1. 开始键入资源池的名称 **资源池** 字段，然后在其出现时从列表中选择它。\
   您可以将多个资源池与一个项目或模板关联。

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. 单击&#x200B;**保存**。

有关如何编辑项目并将其与资源池关联的更多信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

有关如何编辑模板并将其与资源池关联的更多信息，请参阅 [编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## 将资源池与多个项目或模板批量关联

您可以批量编辑多个项目或模板，并同时将同一资源池与它们的所有项目或模板相关联。

您可以使用与将资源池与项目关联相同的方式将资源池与模板关联。

要将资源池与多个项目批量关联，请执行以下操作：

1. 转到项目列表。
1. 选择多个项目，然后单击 **编辑** 图标 ![](assets/edit-icon.png) 位于列表顶部。

1. 单击 **设置**.
1. 开始键入资源池的名称 **资源池** 字段，然后在其出现时从列表中选择它。\
   您可以将多个资源池与项目或模板关联。

   >[!NOTE]
   >
   >* 在生产环境中，当您批量编辑项目或模板时，此字段仅显示所有选定项目或模板通用的资源池。 如果所选项目没有共享资源池，则此字段将为空。 您在此处指定的资源池将覆盖项目或模板的单个资源池。
   >
   >* <span class="preview">在“预览”环境中，当您批量编辑项目时，如果所选项目具有不同的资源池，则会显示“多个值”指示符。 如果批量添加资源池，则所有池都将添加到所选项目中，并覆盖原始资源池。</span>


   <span class="preview">![add_resource_pools_to_multiple_projects.png](assets/add-resource-pools-to-multiple-projects-350x358.png)</span>

1. 单击 **保存更改**.\
   当资源池与项目或模板关联时，您可以在资源规划者内为项目预算用户分配。\
   有关资源规划者的详细信息，请参阅 [资源规划者概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

有关如何批量编辑项目的更多信息，请参阅中的“批量编辑项目”部分 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

有关如何批量编辑模板的详细信息，请参阅中的“批量编辑模板”部分 [编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
