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
source-wordcount: '490'
ht-degree: 0%

---

# 将资源池与用户关联

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

资源池是用户集合，可帮助您管理Adobe Workfront中的资源。

必须先创建资源池，然后才能将其与用户关联。

在创建资源池时，可以将用户与资源池相关联。

如果创建资源池时没有向其中填充用户，则以后可以在编辑或创建新用户时将它们与用户相关联。

有关资源池的信息，请参阅[资源池概述](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)。

有关创建资源池的信息，请参阅[创建资源池](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)。

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
   <td> <p>编辑对资源管理的访问权限，其中包括对管理资源池的访问权限</p> <p>编辑对项目、模板和用户的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理您与资源池关联的项目、模板和用户的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 将资源池与一个用户关联

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)。

1. 单击&#x200B;**用户**。
1. 选中列表中用户名旁边的框，然后单击&#x200B;**编辑**。
1. 单击&#x200B;**资源计划**。
1. 在&#x200B;**资源池**&#x200B;字段中开始键入要与用户关联的资源池的名称，然后在该名称出现时从列表中选择它。\
   您可以将多个资源池与一个用户关联。\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. 单击&#x200B;**保存更改**。

有关编辑用户的详细信息，请参阅[编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

有关创建新用户的详细信息，请参阅[添加用户](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

## 将资源池与用户批量关联

您可以批量编辑多个用户，并同时将同一资源池与所有这些用户关联。

要将资源池与多个用户批量关联，请执行以下操作：

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)。

1. 单击&#x200B;**用户**。
1. 选择列表上的多个用户，然后单击&#x200B;**编辑**。
1. 单击&#x200B;**资源计划**。
1. 在&#x200B;**资源池**&#x200B;字段中开始键入要与用户关联的资源池的名称，然后在该名称出现时从列表中选择它。\
   您可以将多个资源池与多个用户关联。

   >[!NOTE]
   >
   >只有所有选定用户通用的资源池才会显示在此字段中。 如果所选用户没有共享资源池，则此字段为空。 如果此字段为空，则在此处指定的资源池将覆盖其各自的资源池。

1. 单击&#x200B;**保存更改**。

有关如何批量编辑用户的详细信息，请参阅[批量编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md)。
