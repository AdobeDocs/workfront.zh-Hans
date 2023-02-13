---
product-area: templates
navigation-topic: templates-navigation-topic
title: 创建项目模板
description: 您可以从“模板”区域创建和删除模板。 在构建新模板时，您可以输入所有任务的信息以及将来项目设置的所有信息。 然后，当您从模板创建项目时，此信息将被传输到项目。
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# 创建项目模板

您可以从“模板”区域创建和删除模板。 在构建新模板时，您可以输入所有任务的信息以及将来项目设置的所有信息。 然后，当您从模板创建项目时，此信息将被传输到项目。

您可以通过以下方式创建新模板：

* 从头开始，如本文所述。
* 从现有项目，将项目另存为模板。

   有关从现有项目创建模板的更多信息，请参阅 [将项目另存为模板](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* 从其他模板复制模板。

   有关复制现有模板的更多信息，请参阅 [复制项目模板](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* 如果您是Workfront管理员，则可以通过导入Blueprint来创建模板。 有关信息，请参阅 [配置Blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## 访问要求

您必须具备以下条件：

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
   <td> <p>计划 </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">从Blueprint导入模板的系统管理员</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对模板的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>默认情况下，您拥有所创建模板的“管理”权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建模板

1. 从 **主菜单** ![](assets/main-menu-icon.png) 单击 **模板**.

1. 单击 **新模板**.

   模板未命名。

   ![新模板](assets/create-template-nwe-2022-350x102.png)

1. 在模板标题中指定新模板的名称，然后按 **输入。**
1. 单击 **模板任务** 的子菜单。
1. 单击&#x200B;**开始添加模板任务**.

   或

   单击 **新建模板任务** 开始向模板添加任务。

   向模板添加模板任务与向项目添加任务相同。

   有关向项目添加任务的更多信息，请参阅 [在项目中创建任务](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >不能向模板添加循环任务。

1. （可选）单击 **甘特图** 图标，以查看模板任务列表的可视表示形式。

   >[!TIP]
   >
   >不能直接从此甘特图编辑任务。

1. 要向新模板添加信息，请单击 **更多** 菜单 ![](assets/more-icon.png)，然后单击 **编辑**.

   有关编辑模板的信息，请参阅 [编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. 单击 **保存更改**.
1. （可选）如果要向模板添加其他项目，请参阅部分 [向模板添加其他项目](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#adding-items-to-template) 在文章中 [编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## 由组关联确定的模板设置

项目模板与组的关联（或缺少它们）会影响项目、任务和问题首选项确定模板中特定设置的方式。 有关更多信息，请参阅 [创建和修改组的项目模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#template2) 在文章中 [创建和修改组的项目模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
