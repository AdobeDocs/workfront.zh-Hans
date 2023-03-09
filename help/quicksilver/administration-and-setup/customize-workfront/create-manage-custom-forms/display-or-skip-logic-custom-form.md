---
title: 使用旧版表单生成器将显示逻辑和跳过逻辑添加到自定义表单
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以根据用户在填写自定义表单时所做的选择，决定应显示或跳过自定义表单的哪些部分。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c687c4a8-a99d-4ac0-b785-5bfe503a7e2c
source-git-commit: 7835b5f9b5903e19b03cb7e25bfae37c9739f064
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 0%

---

# 使用旧版表单生成器将显示逻辑和跳过逻辑添加到自定义表单

您可以根据用户在填写自定义表单时所做的选择，决定应显示或跳过自定义表单的哪些部分。

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

## 使用显示逻辑和跳过逻辑的注意事项

* 要在自定义字段、小组件或分区界限中添加显示逻辑，必须在表单上至少一个多选字段（单选按钮、下拉列表或复选框）之前放置。

   有关自定义表单中的自定义字段和小部件的信息，请参阅 [使用旧版表单生成器将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 和 [使用旧版表单生成器添加或编辑自定义表单中的资产小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* 无法将跳过逻辑添加到构件或分区界限中。 您只能将其添加到多选字段（单选按钮、下拉列表或复选框）。

* 您可以将显示逻辑和跳过逻辑添加到自定义字段中。对于自定义字段，以下全部为true：

   * 它是一个多选字段（单选按钮、下拉列表或复选框）
   * 它前面有一个多选字段
   * 后跟另一个自定义字段

* 复制带有显示逻辑或跳过逻辑的表单时，该逻辑将会复制到新的自定义表单中。
* 为自定义表单创建显示逻辑规则时，请牢记以下几点

   * 默认情况下，显示逻辑语句中未包含的自定义字段会显示在自定义表单中。
   * 您可以创建多字段显示逻辑语句。

* 批量编辑对象时，所有自定义字段都会显示在“编辑对象”框中，包括跳过了或隐藏的字段。

## 创建具有显示和跳过逻辑的示例自定义表单

要了解如何向自定义表单添加显示和跳过逻辑，最好的方法是通过以下两个部分中说明的实际示例：

* [显示逻辑](#display-logic)
* [跳过逻辑](#skip-logic)

### 显示逻辑 {#display-logic}

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **自定义Forms** ![](assets/custom-forms-icon.png).

1. 创建示例自定义表单：

   1. 单击 **新建自定义表单**，然后单击 **项目** 下拉列表中。

   1. 在 **表单标题** 框，键入 **自定义表单示例 — 学习显示逻辑和跳过逻辑**.

   1. 单击 **添加字段** 左上角。
   1. 添加一个名为的下拉字段 *问题字段* 通过单击 **下拉列表**，然后键入 **问题字段** 在 **标签** 盒子。

   1. 下 **选项**，请在文本框中添加以下选项：

      需要研究

      不再做研究

   1. 单击 **保存+关闭** 左下角。

1. 选择新的 **自定义表单示例 — 学习显示逻辑和跳过逻辑** 自定义表单，然后单击 **编辑**.

1. 添加名为的新单行文本字段 *其他研究* 通过单击 **单行文本字段**，然后键入 **其他研究** 在 **标签** 盒子。

1. 单击 **添加逻辑** 左下角附近 **编辑自定义表单** 屏幕。

1. 在显示的框中，使用 **显示逻辑** 选项卡打开时，设置逻辑 **其他研究** 字段将通过单击显示在表单上 **问题字段** 在第一个下拉菜单中， **需要研究** 在第二个下拉菜单中，以及 **已选择** 在第三个下拉菜单中。
1. 单击 **保存** 关闭 **字段逻辑** 窗口，然后单击 **完成** 在 **字段设置** 区域。

   现在，当有人选择 **需要研究** 在 **问题字段** 下拉列表 **其他研究** 将显示字段。

1. 单击 **预览** 以确保逻辑以您所需的方式显示在表单上。
1. 单击 **结束预览** 发现逻辑按预期工作时。
1. 单击 **保存+关闭** 在 **编辑自定义表单** 窗口以保存表单，然后继续到 [跳过逻辑](#skip-logic) 下面的。

### 跳过逻辑 {#skip-logic}

跳过逻辑的功能与显示逻辑类似，但起相反的作用：不要根据特定选择显示特定的自定义多选字段，而是根据用户的选择确定应跳过哪些字段。

要了解此信息，请继续使用您在部分创建的示例自定义表单 [显示逻辑](#display-logic) 在本文中：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms**.
1. 选择表单 **自定义表单示例 — 学习显示逻辑和跳过逻辑** 之前创建的页面名称，然后单击 **编辑**.

1. 选择您创建的下拉字段，名为 *问题字段*.
1. 单击 **添加逻辑** 中的按钮 **字段设置** 侧栏。

1. 在 **字段逻辑** 框，确保 **跳过逻辑** 选项卡处于选中状态。

1. 将第一个下拉列表设置为 **不再做研究** 第二个下拉列表为 **已选择**.

1. 在 **然后跳至** 下拉列表，选择 **表单结尾。**

   现在，当有人选择 **不再做研究** 在 **问题字段** 下拉字段中，表单将直接跳至表单的结尾，而不显示 **其他研究** 字段。

1. 单击&#x200B;**保存**。
1. 单击 **预览**  以确保逻辑按您所需的方式应用。
1. 单击 **完成** 在表单的左下角。
