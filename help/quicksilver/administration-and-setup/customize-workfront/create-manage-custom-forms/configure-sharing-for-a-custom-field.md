---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 配置自定义字段和小组件的共享
description: 默认情况下，在向自定义表单添加新的自定义字段或小组件时，系统中任何有权访问自定义表单的人都可以编辑该项目的属性，如其标签和名称。 您可以通过控制可以与谁共享的来更改此设置。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '943'
ht-degree: 2%

---

# 配置自定义字段和小组件的共享

默认情况下，在向自定义表单添加新的自定义字段或小组件时，系统中任何有权访问自定义表单的人都可以编辑该项目的属性，如其标签和名称。 您可以通过控制可以与谁共享的来更改此设置。

有关自定义表单中的自定义字段和小组件的信息，请参阅 [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 和 [在自定义表单中添加或编辑资产小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

## 配置自定义字段或小组件的共享

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **自定义Forms**.
1. 如果要在组织的Workfront实例中为自定义字段或小组件配置共享，请执行以下操作：

   1. 单击 **字段** 选项卡。
   1. 选择要配置共享的项目，然后单击 **共享**.

   或者，如果要为现有自定义表单中的自定义字段或小组件配置共享，请执行以下操作：

   1. 选择自定义表单，然后单击 **编辑**.
   1. 在右侧的表单编辑区域中，选择要为其配置共享的项目。
   1. 在左侧面板中，单击 **共享字段**.


1. 在 **自定义字段访问** 框中，指定要与谁共享该项目以及要如何共享该项目：

   1. 在 **自定义字段访问** 框中 **授予对的自定义字段访问权限**，开始键入要与其共享项目的用户、团队、职务角色、组或公司的名称，然后在显示该名称时单击该名称。

      ![](assets/share-field-give-access-to.jpg)

   1. 如果您想要更具体地了解如何共享项目，请单击名称右侧的下拉列表，然后使用以下任意选项：

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">查看它</td> 
         <td> <p>您可以单击 <strong>高级设置</strong> 以指定您希望用户还是用户能够使用其访问权限将项目添加到自定义表单，还是与其他用户共享该项目。</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">管理它</td> 
         <td> <p>允许访问以编辑自定义字段，并在字段库和构建自定义表单的页面上查看该字段。</p> <p>您可以单击 <strong>高级设置</strong> 指定您希望用户还是用户能够使用其访问权限从系统中删除项目，还是与其他用户共享该项目。</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. （可选）重复上一步，将其他名称添加到列表并配置其选项。
1. （可选）单击齿轮图标 ![](assets/gear-icon-settings.png) ，以选择全系统共享选项。

   以下选项并非全部同时显示在此下拉菜单中。 例如，仅当选择了另外两个选项之一时，才会显示第二个选项。

   * **在系统范围内创建此可编辑的变量，以便Workfront中的每个人都可以对其进行编辑** （默认选项）

      添加自定义字段或小组件并且不限制共享该字段或小组件时，系统中有权访问自定义表单的每个人都可以查看和编辑其属性。

   * **移除系统范围编辑权限**

      限制仅对您添加到列表中的用户的访问权限。

   * **使其在系统范围内可见，以供 Workfront 中的每个用户查看**

1. 单击 **保存** 或 **保存并关闭**.

## 在共享自定义表单时继承对自定义字段和小组件的访问权限

当某人与组、职务角色、团队或公司共享自定义表单时，收件人将继承查看表单上任何自定义字段和小组件的访问权限。 表单上这些项目的访问权限始终保持不变，这样表单就可以按照创建者的意图为收件人正常运行。 即使对于具有表单编辑访问权限的收件人，也是如此。

您可以了解谁继承了对自定义字段或小组件的访问权限，并可以删除对该字段或小组件的访问权限。

>[!NOTE]
>
>如果收件人在共享的自定义表单上拥有对自定义字段或小组件的管理访问权限，则该访问权限将保留给收件人。

* [了解谁继承了对自定义字段或小组件的访问权限](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [删除共享的自定义表单中对自定义字段或小组件的访问权限](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### 了解谁继承了对自定义字段或小组件的访问权限 {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **自定义Forms**.
1. 单击 **字段** ，然后选择字段、图像或访问小组件。
1. 在显示的框中，单击 **继承权限** 并查看显示的名称。
1. 单击 **取消**.

### 删除共享的自定义表单中对自定义字段或小组件的访问权限 {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

如果您需要删除在已共享的自定义表单中对自定义字段或小组件的访问权限，则需要取消共享该表单。 有关说明，请参阅 [删除对自定义表单的访问权限](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) 在文章中 [共享自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
