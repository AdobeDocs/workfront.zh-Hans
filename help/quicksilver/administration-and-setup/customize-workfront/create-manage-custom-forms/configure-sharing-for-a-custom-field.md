---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 使用旧版表单生成器配置自定义字段和小部件的共享
description: 默认情况下，向自定义表单添加新的自定义字段或构件时，系统中有权访问自定义表单的任何人都可以编辑该项目的属性，例如其标签和名称。 您可以通过控制可与谁共享来更改此设置。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 2%

---

# 使用旧版表单生成器配置自定义字段和小部件的共享

默认情况下，向自定义表单添加新的自定义字段或构件时，系统中有权访问自定义表单的任何人都可以编辑该项目的属性，例如其标签和名称。 您可以通过控制可与谁共享来更改此设置。

有关自定义表单中的自定义字段和小部件的信息，请参阅 [使用旧版表单生成器将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 和 [使用旧版表单生成器添加或编辑自定义表单中的资产小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

&#42;要了解您拥有哪些计划、许可证类型或访问级别配置，请与Workfront管理员联系。

## 为自定义字段或构件配置共享

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **自定义Forms**.
1. 如果您要为组织的Workfront实例中的自定义字段或构件配置共享，请执行以下操作：

   1. 单击 **字段** 选项卡。
   1. 选择要为其配置共享的项目，然后单击 **共享**.

   或者，如果您要为现有自定义表单中的自定义字段或构件配置共享，请执行以下操作：

   1. 选择自定义表单，然后单击 **编辑**.
   1. 在右侧的表单编辑区域中，选择要为其配置共享的项目。
   1. 在左侧面板中，单击 **共享字段**.


1. 在 **自定义字段访问** 框，指定要与谁共享项目以及共享项目的方式：

   1. 在左下角附近 **自定义字段访问** 框，下 **将自定义字段访问权限授予**，开始键入要与之共享项目的用户、团队、工作角色、组或公司的名称，然后单击显示的名称。

      ![](assets/share-field-give-access-to.jpg)

   1. 如果您想更详细地了解要如何共享该项目，请单击该名称右侧的下拉列表，然后使用以下任一选项：

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">查看它</td> 
         <td> <p>您可以单击 <strong>高级设置</strong> 指定您是否希望用户能够使用其访问权限将项目添加到自定义表单或与其他用户共享。</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">管理它</td> 
         <td> <p>允许访问以编辑自定义字段，并在字段库和构建自定义表单的页面上查看它。</p> <p>您可以单击 <strong>高级设置</strong> 指定您是否希望用户能够使用其访问权限从系统中删除项目或与其他用户共享该项目。</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. （可选）重复上一步骤向列表中添加其他名称并配置其选项。
1. （可选）单击齿轮图标 ![](assets/gear-icon-settings.png) （如果要为字段选择系统范围的共享选项）。

   以下选项并非全部同时显示在此下拉菜单中。 例如，仅当选择其他两个变量之一时，才会显示第二个变量。

   * **使其在系统范围内可编辑，以便Workfront中的每个人都可以编辑它** （默认选项）

      当您添加自定义字段或小组件，并且没有限制其共享时，系统中有权访问自定义表单的每个人都可以查看并编辑其属性。

   * **移除系统范围编辑权限**

      仅限您添加到列表中的用户访问。

   * **使其在系统范围内可见，以供 Workfront 中的每个用户查看**

1. 单击 **保存** 或 **保存+关闭**.

## 共享自定义表单时继承对自定义字段和小部件的访问权限

当有人与组、工作角色、团队或公司共享自定义表单时，收件人将继承对表单上任何自定义字段和小部件的查看访问权限。 始终保留对表单上这些项目的这种访问级别，以便表单可以按创建者的预期为收件人运行。 即使收件人拥有表单的编辑权限，也是如此。

您可以查找继承了自定义字段或构件访问权限的用户，并且可以删除对它的访问权限。

>[!NOTE]
>
>如果收件人拥有对共享自定义表单上的自定义字段或小部件的管理访问权限，则该访问权限将保留给收件人。

* [了解谁继承了自定义字段或小部件的访问权限](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [删除对已共享自定义表单中的自定义字段或小部件的访问权限](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### 了解谁继承了自定义字段或小部件的访问权限 {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **自定义Forms**.
1. 单击 **字段** 选项卡，然后选择字段、图像或访问构件。
1. 在显示的框中，单击 **继承的权限** 和查看显示的名称。
1. 单击 **取消**.

### 删除对已共享自定义表单中的自定义字段或小部件的访问权限 {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

如果您需要删除对已共享自定义表单中的自定义字段或小部件的访问权限，则需要取消共享表单。 有关说明，请参阅部分中的 [删除对自定义表单的访问权限](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) 在文章中 [共享自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
