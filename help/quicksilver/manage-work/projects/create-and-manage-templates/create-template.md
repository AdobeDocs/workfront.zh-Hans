---
product-area: templates
navigation-topic: templates-navigation-topic
title: 创建项目模板
description: 您可以在“模板”区域中创建和删除模板。 在构建新模板时，您可以为所有任务和未来项目设置输入信息。 然后，此信息将传输到您从模板创建的任何项目。
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 2%

---

# 创建项目模板

<!-- Audited: 1/2024 -->

您可以在“模板”区域中创建和删除模板。 在构建新模板时，您可以为所有任务和未来项目设置输入信息。 然后，此信息将传输到您从模板创建的任何项目。

>[!NOTE]
>
>模板及其任务没有实际日期，而是指示任务可能从哪天（从未来项目可能开始的时间）开始以及任务可能需要在哪一天完成。 使用模板创建未来项目时，项目将接收实际日期。 有关信息，请参阅[创建项目](../create-projects/create-project.md)。


您可以通过以下方式创建新模板：

* 从头开始，如本文所述。
* 从现有项目中，通过将项目另存为模板。

  有关从现有项目创建模板的详细信息，请参阅[将项目另存为模板](../../../manage-work/projects/manage-projects/save-project-as-template.md)。

* 通过从另一个模板复制它。

  有关复制现有模板的详细信息，请参阅[复制项目模板](../../../manage-work/projects/create-and-manage-templates/copy-template.md)。

* 通过导入Blueprint。 您必须是Workfront管理员才能导入Blueprint。 有关信息，请参阅[配置Blueprint](../../../administration-and-setup/blueprints/configure-template-package.md)。

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
   <td> <p>标准 </p><p>规划</p> <p>您必须是系统管理员才能从Blueprint导入模板</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对模板的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>默认情况下，您对创建的模板具有管理权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p><p>Or </p><p>Current: Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You must be a system administrator to import templates from Blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>You have Manage permissions to the templates you create, by default</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## 创建模板

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**模板**。

1. 单击&#x200B;**新建模板**。

   模板未命名。

   ![新模板](assets/create-template-nwe-2022-350x102.png)

1. 在模板标题中指定新模板的名称，然后按&#x200B;**Enter。**
1. 单击左侧面板中的&#x200B;**模板任务**&#x200B;部分。
1. 单击&#x200B;**开始添加模板任务**。

   或

   单击&#x200B;**新建模板任务**&#x200B;以开始向模板添加任务。

   将模板任务添加到模板与将任务添加到项目相同。

   有关将任务添加到项目的详细信息，请参阅[在项目中创建任务](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)。

   >[!NOTE]
   >
   >您无法将周期性任务添加到模板。

1. （可选）单击任务列表右上角的&#x200B;**甘特图**&#x200B;图标以查看模板任务列表的可视表示形式。

   >[!TIP]
   >
   >不能直接从该甘特图编辑任务。

1. 若要向新模板添加信息，请单击&#x200B;**更多**&#x200B;菜单![更多图标](assets/more-icon.png)，然后单击&#x200B;**编辑**。

   有关编辑模板的信息，请参阅[编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)。

1. 单击&#x200B;**保存更改**。
1. （可选）如果要向模板添加其他项，请参阅文章[编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#add-additional-items-to-a-template)中的[向模板添加其他项](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)部分。

## 由组关联确定的模板设置

项目模板与组（或缺少组）的关联会影响项目、任务和问题首选项如何确定模板中的某些设置。 有关详细信息，请参阅文章[创建和修改组的项目模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#create-and-modify-a-groups-project-templates)中的[创建和修改组的项目模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md)部分。
