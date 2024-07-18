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

有关将用户分配到布局模板的信息，请参阅[将用户分配到布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)。

有关布局模板的更多信息，请参阅[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

有关组的布局模板的信息，请参阅[创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td><p>系统管理员访问级别</p><p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 授予对布局模板的管理访问权限

1. 开始处理布局模板，如[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。
1. 在页面顶部单击&#x200B;**授予对**&#x200B;的访问权限。
1. 在出现的框中，单击&#x200B;**添加组**，开始键入组的名称，在组出现时单击该名称，然后单击&#x200B;**完成**。

   指定为指定组的组管理员的任何用户都可以管理布局模板。 但是，不会将模板分配给组的成员以供使用。 有关将布局模板分配给组的信息，请参阅本文中的[将布局模板分配给用户](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md#assign)。

   >[!NOTE]
   >
   >* 当组管理员创建布局模板时，必须分配管理访问权限。 布局模板是为指定的组而指定的，并且仅对指定的组可见。 有关详细信息，请参阅[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。 有关组管理员的信息，请参阅[组管理员](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)。
   >   
   >* 如果不向特定组中的组管理员授予管理权限，则所有可以编辑用户帐户的用户，都具有对布局模板的管理权限。 有些Workfront管理员特意选择不授予对布局模板的管理访问权限，以使布局模板成为系统级别的布局模板。

1. 您可以随时单击保存以保存进度，然后继续修改模板。
