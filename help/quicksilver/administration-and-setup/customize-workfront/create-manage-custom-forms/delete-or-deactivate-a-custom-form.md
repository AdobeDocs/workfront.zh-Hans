---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 删除或停用自定义表单
description: 您可以从系统中删除或停用自定义表单。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d97badf-b6d0-4e7c-bff8-9ff63e83586b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# 删除或停用自定义表单

您可以从系统中删除或停用自定义表单。

>[!CAUTION]
>
>删除自定义表单还会删除与表单关联的对象上的所有自定义数据。 无法恢复已删除的数据。 请考虑停用自定义表单 — 停用不再使用的自定义表单时，将保留所有关联的历史数据。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront计划*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>计划</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>对自定义表单的管理访问权限</p> <p>有关Workfront管理员如何授予此访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问级别配置，请联系您的Workfront管理员。

## 删除自定义表单

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms。**
1. 选择自定义表单，然后单击 **删除**.
1. 如果确定要永久删除自定义表单以及附加该表单的对象上的所有关联数据，请单击 **是，删除它**.

## 停用自定义表单

您可以在不丢失其关联的历史数据的情况下停用不再使用的自定义表单。 用户无法向对象添加不活动的自定义表单，但他们仍可以查看已附加对象的数据并将其添加到其字段中。

非活动自定义表单上的字段仍可用于在视图中进行内联编辑。 如果用户在内联编辑期间从不活动的自定义表单添加字段，则表单会自动附加到对象，即使已停用自定义表单也是如此。

如果您重新激活自定义表单，它将保留之前的设置，用户可以像从未停用一样与其进行交互。

要停用自定义表单，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击要停用的自定义表单的名称。
1. 单击 **表单设置** 选项卡。
1. 禁用 **处于活动状态** 选项。
1. 单击 **保存并关闭**.
