---
title: 使用表单设计器从现有自定义表单中添加或删除对象类型
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以使用表单设计器从自定义表单中添加或删除对象类型。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: c0082dd73e3db8123f9cc08f1798ef8e70730625
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---


# 使用表单设计器从现有自定义表单中添加或删除对象类型

{{highlighted-preview-article-level}}

您可以使用表单设计器从现有自定义表单中添加或删除对象类型。

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
   <td>
   <p>当前计划：标准</p>
   <p>或</p>
   <p>传统计划：计划</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td><p>对自定义表单的管理访问权限</p> <p>有关Workfront管理员如何授予此访问权限的信息，请参阅 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;要了解您拥有哪些计划、许可证类型或访问级别配置，请与Workfront管理员联系。

## 将对象类型添加到现有自定义表单

您可以将其他对象类型添加到表单，以便将其附加到多个对象。

>[!NOTE]
>
>分区界限权限可能受对象类型影响。 自定义表单分区界限的“有限编辑”权限仅适用于“项目”、“任务”、“问题”和“用户”对象类型。
>
>有关更多信息，请参阅 [多个对象类型如何影响分区界限权限](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms** （在左侧面板中）。

   在显示的视图中，您可以查看为您的组织创建的所有自定义表单。 您还可以查看每个表单的创建者、表单使用的对象类型以及表单是否处于活动状态。

1. 选择要向其中添加其他对象类型的自定义表单，然后单击 **编辑**.

1. 单击表单顶部的加号+之后 **对象类型**，然后在显示的菜单中选择所需的类型。 您可以重复此操作，以添加所需数量的对象类型。

   ![](assets/add-new-object.png)

1. 单击 **保存并关闭**.

   >[!TIP]
   >
   >您可以单击 **应用** 创建自定义表单时，可随时保存更改并保持表单打开。

## 删除自定义表单上的对象类型

您可以从现有自定义表单中删除对象类型。 自定义表单必须至少有一个对象类型。

>[!CAUTION]
>
>如果人们已经将自定义表单附加到要删除的类型的对象并向其添加数据，则当您删除表单上的该对象类型时，将会永久删除该数据。 它可能包含用户以后需要的历史信息。
>
>通常，我们建议最大限度地减少编辑已使用的自定义表单的次数。 没有通知系统来提醒使用自定义表单的用户您所做的更改。

要删除对象类型，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms** （在左侧面板中）。
1. 选择要编辑的自定义表单，然后单击 **编辑**.
1. 单击任意 **对象类型** 要从表单中删除的条目，然后单击 **删除** 在显示的警告消息上。

   ![](assets/delete-object-types.png)

1. （可选）对要从表单中删除的任何其他对象类型重复上一步骤。
1. 单击 **完成**，然后单击 **关闭并保存**.
