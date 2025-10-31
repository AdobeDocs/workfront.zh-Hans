---
product-area: templates
navigation-topic: templates-navigation-topic
title: 删除项目模板
description: 我们建议您停用不再使用的模板，而不是删除它们，以便您可以保留有关您项目随时间变化的历史信息。
author: Alina
feature: Work Management
exl-id: 41e0979c-f8ef-4a07-8848-e4ee8cc212c5
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# 删除项目模板

我们建议您停用不再使用的模板，而不是删除它们，以便您可以保留有关您项目随时间变化的历史信息。 有关停用模板的信息，请参阅[编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)。

>[!IMPORTANT]
>
>删除模板时，使用该模板的项目不会以任何方式修改。 但是，您在项目的“模板”字段中无法再看到原始模板的名称。 此外，您无法再在任务视图中查看项目上任务的模板任务的名称。 删除最初与项目关联的模板后，项目上的模板字段和任务上的模板任务字段保持空白。

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
   <td> <p>编辑对模板的访问权限，其中包括删除权限</p> <td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对模板的权限，包括删除模板的权限</p></td> 
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
   <td> <p>Edit access to&nbsp;Templates that includes access to Delete</p> <p> <img src="assets/template-access-level-with-advanced-settings-350x113.png" style="width: 350;height: 113;"> </p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the template that includes permissions to Delete it</p> <p> <img src="assets/template-manage-permissions-with-advanced-settings-350x352.png" style="width: 350;height: 352;"> </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 删除模板的注意事项

* 在附加模板时添加到项目的任务保留在项目中。 但是，与任务关联的模板任务信息会被删除。
* 模板名称不再列在项目的&#x200B;**概述**&#x200B;子选项卡上的&#x200B;**模板**&#x200B;字段中。

* 您可以从回收站中恢复最近删除的模板。 有关从回收站恢复项目的信息，请参阅[恢复已删除的项目](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。

## 删除模板

{{step1-to-templates}}

这将打开一个模板列表

1. 通过单击模板名称左侧的复选框选择要删除的模板，然后单击&#x200B;**删除>是，删除它**&#x200B;以确认删除。

   或

   单击模板名称以访问模板，然后单击&#x200B;**更多**&#x200B;菜单![更多图标](assets/more-icon.png)，然后单击&#x200B;**删除模板>是，删除模板**。

   模板不再可用于与项目关联。
