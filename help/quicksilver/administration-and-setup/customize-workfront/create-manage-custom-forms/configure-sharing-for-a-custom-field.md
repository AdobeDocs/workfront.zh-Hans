---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 使用旧版表单生成器配置自定义字段和小部件的共享
description: 默认情况下，向自定义表单添加新的自定义字段或构件时，系统中有权访问自定义表单的任何人都可以编辑该项目的属性，例如其标签和名称。 您可以通过控制可与谁共享来更改此设置。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# 使用旧版表单生成器配置自定义字段和小部件的共享

{{form-designer-default}}

默认情况下，向自定义表单添加新的自定义字段或构件时，系统中有权访问自定义表单的任何人都可以编辑该项目的属性，例如其标签和名称。 您可以通过控制可与谁共享来更改此设置。

有关自定义表单中的自定义字段和小部件的信息，请参阅[使用旧版表单生成器将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)和[使用旧版表单生成器添加或编辑自定义表单中的资产小部件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront计划</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
   <p>新增：标准</p>
   <p>或</p>
   <p>当前：计划</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>对自定义表单的管理访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 为自定义字段或小组件配置共享

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**自定义Forms**。
1. 如果您在组织的Workfront实例中为自定义字段或构件配置共享，请执行以下操作：

   1. 单击&#x200B;**字段**&#x200B;以打开“字段”区域。
   1. 选择要为其配置共享的项目，然后单击![共享图标](assets/share-icon.png)。

   或者，如果您要为现有自定义表单中的自定义字段或构件配置共享，请执行以下操作：

   1. 选择自定义表单，然后单击![编辑图标](assets/edit-icon.png)。
   1. 在右侧的表单编辑区域中，选择要为其配置共享的项目。
   1. 在左侧面板中，单击&#x200B;**共享字段**。

1. 在显示的&#x200B;**自定义字段访问**&#x200B;框中，指定要与谁共享该项以及共享该项的方式：

   1. 在&#x200B;**自定义字段访问权限**&#x200B;框的左下角附近，在&#x200B;**将自定义字段访问权限授予**&#x200B;下，开始键入要与其共享项目的用户、团队、工作角色、组或公司的名称，然后单击显示的名称。

      ![](assets/share-field-give-access-to.jpg)

   1. 如果要更详细地了解要如何共享该项目，请单击名称右侧的下拉列表，然后使用以下任一选项：

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">查看它</td> 
         <td> <p>您可以单击<strong>高级设置</strong>，以指定您是否希望一个或多个用户能够使用其访问权限将项目添加到自定义表单或与其他用户共享。</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">管理它</td> 
         <td> <p>允许访问以编辑自定义字段，并在字段库和构建自定义表单的页面上查看它。</p> <p>您可以单击<strong>高级设置</strong>，以指定您是否希望一个或多个用户能够使用其权限从系统中删除项目或与其他用户共享该项目。</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. （可选）重复上一步骤向列表中添加其他名称并配置其选项。
1. （可选）如果要为字段选择系统范围的共享选项，请单击右上角的齿轮图标![](assets/gear-icon-settings.png)。

   以下选项并非全部同时显示在此下拉菜单中。 例如，仅当选择其他两个变量之一时，才会显示第二个变量。

   * **使其在系统范围内可编辑，以便Workfront中的每个人都可以编辑它**（默认选项）

     当您添加自定义字段或构件并且不限制其共享时，系统中有权访问自定义表单的每个人都可以查看并编辑其属性。

   * **删除系统范围编辑权限**

     仅限您添加到列表中的用户访问。

   * **使其在系统范围内可见，以便Workfront中的每个人都可以看到它**

1. 单击&#x200B;**保存**&#x200B;或&#x200B;**保存+关闭**。

## 共享自定义表单时继承对自定义字段和小部件的访问权限

当有人与组、工作角色、团队或公司共享自定义表单时，收件人将继承对表单上任何自定义字段和小部件的查看访问权限。 对表单上这些项目的这种访问级别始终会保留，以便表单能够按创建者的预期用于收件人。 即使对于拥有表单编辑访问权限的收件人也是如此。

您可以查明继承了自定义字段或构件访问权限的用户，并且可以移除对它的访问权限。

>[!NOTE]
>
>如果收件人拥有对共享自定义表单上的自定义字段或小部件的管理访问权限，则该访问权限将保留给收件人。

* [了解谁继承了自定义字段或小组件的访问权限](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [删除对已共享自定义表单中的自定义字段或小部件的访问权限](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### 了解谁继承了自定义字段或小部件的访问权限 {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**设置** ![](assets/gear-icon-settings.png)。

1. 在左侧面板中，单击&#x200B;**自定义Forms**。
1. 单击&#x200B;**字段**，然后选择该字段、图像或访问小组件。
1. 在显示的框中，单击&#x200B;**继承权限**&#x200B;并查看显示的名称。
1. 单击&#x200B;**取消**。

### 删除对已共享自定义表单中的自定义字段或小部件的访问权限 {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

如果您需要删除对已共享自定义表单中的自定义字段或小部件的访问权限，则需要取消共享该表单。 有关说明，请参阅[共享自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)一文中的[删除对自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare)的访问权限。
