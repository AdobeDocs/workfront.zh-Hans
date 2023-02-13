---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 删除自定义表单中的对象类型
description: 在现有的自定义表单上，您可以删除与表单关联的对象类型。 执行此操作后，用户将无法再将表单附加到该类型的对象。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# 删除自定义表单中的对象类型

在现有的自定义表单上，您可以删除与表单关联的对象类型。 执行此操作后，用户将无法再将表单附加到该类型的对象。

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

## 删除自定义表单中的对象类型

您可以从现有自定义表单中删除对象类型。

自定义表单必须至少具有一个对象类型。

>[!CAUTION]
>
>如果用户已将自定义表单附加到要删除的类型对象并向其添加数据，则当您在表单上删除该对象类型时，该数据将被永久删除。 其中可能包含用户以后需要的历史信息。
>
>通常，我们建议最大限度地减少您编辑已在使用的自定义表单的次数。 没有通知系统可提醒使用自定义表单的人员您所做的更改。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms** 中。
1. 选择要编辑的自定义表单，然后单击 **编辑**.
1. 单击 **对象类型** 要从表单中删除的内容，然后单击 **删除** 显示的警告消息上。

   ![](assets/click-x-object-types.jpg)

1. （可选）对要从表单中删除的任何其他对象类型重复上一步。
1. 单击 **完成**，然后单击 **关闭并保存**.
