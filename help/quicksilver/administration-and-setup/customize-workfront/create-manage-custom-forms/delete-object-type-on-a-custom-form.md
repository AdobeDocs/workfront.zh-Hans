---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 删除自定义表单上的对象类型
description: 在现有的自定义表单上，您可以删除与该表单关联的对象类型。 执行此操作后，用户无法再将表单附加到该类型的对象。
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# 删除自定义表单上的对象类型

在现有的自定义表单上，您可以删除与该表单关联的对象类型。 执行此操作后，用户无法再将表单附加到该类型的对象。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront计划*</p> </td> 
   <td>任何</td> 
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

&#42;要了解您拥有的计划、许可证类型或访问级别配置，请与Workfront管理员联系。

## 删除自定义表单上的对象类型

您可以从现有自定义表单中删除对象类型。

自定义表单必须至少具有一个对象类型。

>[!CAUTION]
>
>如果人们已经将自定义表单附加到要删除的类型的对象并向其添加数据，则当您删除表单上的该对象类型时，将会永久删除该数据。 它可能包含用户以后需要的历史信息。
>
>通常，我们建议最大限度地减少编辑已使用的自定义表单的次数。 没有通知系统来提醒使用自定义表单的人员您的更改。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms** 在左侧面板中。
1. 选择要编辑的自定义表单，然后单击 **编辑**.
1. 单击任意 **对象类型** 要从表单中删除的项目，然后单击 **删除** 在显示的警告消息上。

   ![](assets/click-x-object-types.jpg)

1. （可选）对要从表单中删除的任何其他对象类型重复上一步骤。
1. 单击 **完成**，然后单击 **关闭并保存**.
