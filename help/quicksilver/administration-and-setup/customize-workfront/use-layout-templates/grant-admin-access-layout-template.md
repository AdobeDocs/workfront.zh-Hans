---
title: 授予对布局模板的管理访问权限
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: 作为Adobe Workfront管理员，您可以向特定组的组管理员授予对布局模板的管理访问权限，以便他们能够编辑该模板。 这不会将模板分配给组中的用户。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 066a55ef-1904-4678-8866-c59428f78bc1
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# 授予对布局模板的管理访问权限

作为Adobe Workfront管理员，您可以向特定组的组管理员授予对布局模板的管理访问权限，以便他们能够编辑该模板。 这不会将模板分配给组中的用户。

有关将用户分配到布局模板的信息，请参阅 [将用户分配给布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

有关布局模板的详细信息，请参阅 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

有关组的布局模板的信息，请参阅 [创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td><p>系统管理员访问级别</p><p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 授予对布局模板的管理访问权限

1. 开始使用布局模板，如中所述 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 单击 **授予对的访问权限** （在页面的顶部）。
1. 在出现的框中，单击 **添加组**，开始键入组的名称，在组出现时单击该名称，然后单击 **完成**.

   任何指定为指定组的组管理员的用户都可以管理布局模板。 但是，不会将模板分配给组的成员以供使用。 有关将布局模板分配给组的信息，请参阅 [为用户分配布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md#assign) 本文章中。

   >[!NOTE]
   >
   >* 当组管理员创建布局模板时，必须分配管理访问权限。 布局模板是为指定的组而设计的，并且仅对指定的组可见。 有关更多信息，请参阅 [编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). 有关组管理员的信息，请参见 [组管理员](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).
   >   
   >* 如果您不向特定组中的组管理员授予管理访问权限，则所有可以编辑用户帐户的用户，都具有对布局模板的管理访问权限。 有些Workfront管理员特意选择不授予对布局模板的管理访问权限，以便使其成为系统级别的布局模板。

1. 您可以随时单击保存以保存进度，然后稍后继续修改模板。
