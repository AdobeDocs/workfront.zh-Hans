---
title: 向自定义表单添加显示逻辑和跳过逻辑
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以根据用户在填写自定义表单时所做的选择，决定应显示或跳过自定义表单的哪些部分。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c687c4a8-a99d-4ac0-b785-5bfe503a7e2c
source-git-commit: 59e3b958dd81f2f068bc06c3fe439de0084f9ce4
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# 向自定义表单添加显示逻辑和跳过逻辑

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

&#42;要了解您拥有的计划、许可证类型或访问级别配置，请联系您的Workfront管理员。

## 使用显示逻辑和跳过逻辑的注意事项

* 要在自定义字段、小组件或区域中断中添加显示逻辑，必须在表单上至少放置一个多选字段（单选按钮、下拉列表或复选框）。

   有关自定义表单中的自定义字段和小组件的信息，请参阅 [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 和 [在自定义表单中添加或编辑资产小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* 无法向小组件或区域中断添加跳过逻辑。 您只能将其添加到多个选择字段（单选按钮、下拉列表或复选框）。

* 您可以将显示逻辑和跳过逻辑添加到自定义字段中，有关自定义字段，所有以下情况均为true:

   * 它是一个多选字段（单选按钮、下拉列表或复选框）
   * 前面有一个多选字段
   * 其后是另一个自定义字段

* 在复制具有显示逻辑或跳过逻辑的表单时，该逻辑将复制到新的自定义表单。
* 在为自定义表单创建显示逻辑规则时，请记住以下事项

   * 默认情况下，显示逻辑语句中未包含的自定义字段显示在自定义表单上。
   * 您可以创建多字段显示逻辑语句。

* 批量编辑对象时，所有自定义字段都会显示在“编辑对象”框中，包括跳过或隐藏的字段。

## 创建具有显示和跳过逻辑的示例自定义表单

了解如何向自定义表单添加显示和跳过逻辑的最佳方式，是通过以下两节中介绍的实用示例：

* [显示逻辑](#display-logic)
* [跳过逻辑](#skip-logic)

### 显示逻辑 {#display-logic}

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **自定义Forms** ![](assets/custom-forms-icon.png).

1. 创建示例自定义表单：

   1. 单击 **新建自定义表单**，然后单击 **项目** 中。

   1. 在 **表单标题** 框，文字 **自定义表单示例 — 学习显示逻辑和跳过逻辑**.

   1. 单击 **添加字段** 中。
   1. 添加一个名为 *问题字段* 单击 **下拉列表**，然后键入 **问题字段** 在 **标签** 框中。

   1. 在 **选择**，在文本框中添加以下选项：

      所需研究

      不再进行研究

   1. 单击 **保存并关闭** 在左下角。

1. 选择新 **自定义表单示例 — 学习显示逻辑和跳过逻辑** 自定义表单，然后单击 **编辑**.

1. 添加名为 *其他研究* 单击 **单行文本字段**，然后键入 **其他研究** 在 **标签** 框中。

1. 单击 **添加逻辑** 靠近 **编辑自定义表单** 屏幕。

1. 在显示的框中，使用 **显示逻辑** 选项卡，设置 **其他研究** 字段 **问题字段** 在第一个下拉菜单中， **所需研究** 在第二个下拉菜单中， **已选择** 第三个下拉框中。
1. 单击 **保存** 关闭 **字段逻辑** 窗口，然后单击 **完成** 在 **字段设置** 的上界。

   现在，当有人选择 **所需研究** 在 **问题字段** 下拉菜单， **其他研究** 字段。

1. 单击 **预览** 以确保逻辑在表单中以您希望的方式显示。
1. 单击 **结束预览** 当您发现逻辑可按预期工作时。
1. 单击 **保存并关闭** 在 **编辑自定义表单** 窗口以保存表单，然后继续 [跳过逻辑](#skip-logic) 下。

### 跳过逻辑 {#skip-logic}

跳过逻辑函数与显示逻辑类似，但却起到反作用：您可以根据用户的选择确定应跳过哪些字段，而不是根据特定选择显示特定的自定义多选字段。

要了解此信息，请继续处理您在部分中创建的示例自定义表单 [显示逻辑](#display-logic) 在本文中：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms**.
1. 选择表单 **自定义表单示例 — 学习显示逻辑和跳过逻辑** 创建的URL，然后单击 **编辑**.

1. 选择您创建的下拉字段，该字段名为 *问题字段*.
1. 单击 **添加逻辑** 按钮 **字段设置** 侧栏。

1. 在 **字段逻辑** 框，确保 **跳过逻辑** 选项卡。

1. 将第一个下拉列表设置为 **不再进行研究** 第二个下拉 **已选择**.

1. 在 **然后跳到** 下拉列表，选择 **表单结尾。**

   现在，当有人选择 **不再进行研究** 在 **问题字段** 下拉字段中，表单将直接跳到表单的结尾，而不显示 **其他研究** 字段。

1. 单击&#x200B;**保存**。
1. 单击 **预览**  以确保逻辑按您所需的方式应用。
1. 单击 **完成** 的下方。
