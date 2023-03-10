---
title: 停用或重新激活自定义表单
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以重新激活或取消激活自定义表单。 我们建议停用自定义表单，而不是删除不再用于保留历史数据的表单。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: c0082dd73e3db8123f9cc08f1798ef8e70730625
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---


# 停用或重新激活自定义表单

您可以重新激活或取消激活自定义表单。 我们建议停用自定义表单，而不是删除不再用于保留历史数据的表单。

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
   <td> <p>对自定义表单的管理访问权限</p> <p>有关Workfront管理员如何授予此访问权限的信息，请参阅 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;要了解您拥有哪些计划、许可证类型或访问级别配置，请与Workfront管理员联系。

## 取消激活自定义表单

您可以停用不再使用的自定义表单，而不会丢失其关联的历史数据。 用户无法将非活动的自定义表单添加到对象，但他们仍然可以查看数据并将其添加到已附加该表单的对象上的字段。

非活动自定义表单上的字段也仍可用于在视图中内联编辑。 如果用户在内联编辑期间从非活动自定义表单添加字段，即使自定义表单已停用，该表单也会自动附加到对象。

要停用自定义表单，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).
1. 在左侧面板中，选择 **自定义Forms**.
1. 在 **Forms** 选项卡，选择要取消激活的自定义表单。
1. 在“活动”列中，选择 **False** ，然后单击退出列。 该表单不再处于活动状态。

## 重新激活自定义表单

如果重新激活自定义表单，则它会保留以前拥有的设置，用户可以像从未停用它一样与它进行交互。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).
1. 在左侧面板中，选择 **自定义Forms**.
1. 在 **Forms** 选项卡，选择要重新激活的自定义表单。
1. 在“活动”列中，选择 **True** ，然后单击退出列。 该表单现在处于活动状态。