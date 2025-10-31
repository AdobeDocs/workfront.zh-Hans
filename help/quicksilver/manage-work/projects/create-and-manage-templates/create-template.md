---
product-area: templates
navigation-topic: templates-navigation-topic
title: 创建项目模板
description: 您可以在“模板”区域中创建和删除模板。 在构建新模板时，您可以为所有任务和未来项目设置输入信息。 然后，此信息将传输到您从模板创建的任何项目。
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 5%

---

# 创建项目模板

<!-- Audited: 10/2025 -->

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

{{step1-to-templates}}

1. 单击&#x200B;**新建模板**。

   模板未命名。

   ![新模板](assets/create-template-nwe-2022-350x102.png)

1. 在模板标题中指定新模板的名称，然后按&#x200B;**Enter。**
1. 单击左侧面板中的&#x200B;**模板任务**&#x200B;部分。
1. 单击&#x200B;**开始添加模板任务**&#x200B;以添加内联任务

   或

   单击&#x200B;**新建模板任务**，开始在&#x200B;**新建模板任务**&#x200B;框中将任务添加到模板。

   ![新模板任务框](assets/new-template-task-box.png)

1. 更新以下方面的信息：

   * 概述
   * 财务
   * 设置
   * 任务
   * 自定义表单
   * 附加文档

     更新模板任务的信息与编辑项目中的任务类似。 有关详细信息，请参阅[编辑任务](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md)。

   >[!NOTE]
   >
   >您无法将周期性任务添加到模板。

1. 单击下列选项之一：

   * **保存模板任务**&#x200B;以保存当前模板任务并关闭“新建模板任务”框。
   * **保存模板任务并启动另一个模板任务**&#x200B;以保存当前模板任务并打开另一个新模板任务框以添加另一个任务。
   * **取消**&#x200B;关闭该框而不保存模板任务。
1. （可选）添加模板任务后，在“模板任务”部分中，单击任务列表右上角的&#x200B;**甘特图**&#x200B;图标，查看模板任务列表的可视表示形式。

   >[!TIP]
   >
   >不能直接从该甘特图编辑任务。

1. 若要向新模板添加信息，请单击标题中模板名称左侧的&#x200B;**更多**&#x200B;菜单![更多图标](assets/more-icon.png)，然后单击&#x200B;**编辑**。

   有关编辑模板的信息，请参阅[编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)。

   >[!NOTE]
   >
   >   项目模板与组（或缺少组）的关联会影响项目、任务和问题首选项如何确定模板中的某些设置。
   >
   >有关详细信息，请参阅[创建和修改组的项目模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md)一文中的“首选项如何应用于模板和模板任务”一节。

1. 单击&#x200B;**保存**。
1. （可选）将以下项目添加到模板

   * 文档
   * 风险
   * 审批流程
   * 记帐费率
   * 费用
   * 队列详细信息
   * 主题组和队列主题

1. （可选）将以下项目添加到模板中的任务：

   * 文档
   * 费用
   * 审批

   有关信息，请参阅[编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)一文中的“向模板添加更多项”一节。




