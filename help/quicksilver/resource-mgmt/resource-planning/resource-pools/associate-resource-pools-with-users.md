---
product-area: resource-management
navigation-topic: resource-pools
title: 将资源池与用户关联
description: 将资源池与用户关联
author: Alina
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# 将资源池与用户关联

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

资源池是用户的集合，可帮助您在Adobe Workfront中管理资源。

必须先创建资源池，然后才能将其与用户关联。

在创建资源池时，可以将用户与资源池关联。

如果您在创建资源池时不用用户填充它们，则在您编辑或创建新用户时，以后可以将它们与用户关联。

有关资源池的信息，请参阅 [资源池概述](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

有关创建资源池的信息，请参阅 [创建资源池](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业及更高级别</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对资源管理的访问权限，其中包括对管理资源池的访问权限</p> <p>编辑对项目、模板和用户的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理将资源池与之关联的项目、模板和用户的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 将资源池与一个用户关联

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 **用户**.
1. 选中列表中用户名称旁边的框，然后单击 **编辑**.
1. 单击 **资源计划**.
1. 开始键入要与 **资源池** 字段，然后在显示时从列表中选择该字段。\
   您可以将多个资源池与一个用户关联。\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. 单击 **保存更改**.

有关编辑用户的更多信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

有关创建新用户的更多信息，请参阅 [添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## 将资源池与用户批量关联

您可以批量编辑多个用户，并将同一资源池与所有这些用户都同时关联。

要将资源池与多个用户批量关联，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 **用户**.
1. 在列表中选择多个用户，然后单击 **编辑**.
1. 单击 **资源计划**.
1. 开始键入要与 **资源池** 字段，然后在显示时从列表中选择该字段。\
   您可以将多个资源池与多个用户关联。

   >[!NOTE]
   >
   >只有所有选定用户共有的资源池才会显示在此字段中。 如果选定的用户没有共享资源池，则此字段为空。 如果此字段为空，则此处指定的资源池将覆盖其各个资源池。

1. 单击 **保存更改**.

有关如何批量编辑用户的更多信息，请参阅 [批量编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
