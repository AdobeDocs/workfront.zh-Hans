---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: “错误消息：有个小问题。 该字段用于多表单配置中”
description: 当您在自定义表单的计算自定义字段中更改计算时，如果出现一条错误消息，告知您该字段已用在多表单配置中，则需要将该字段替换为包含您要使用的计算的新字段。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 43668525-5572-4d82-8eed-0e320249f296
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 0%

---

# 错误消息：有个小问题。 该字段用于多表单配置

## 问题

在自定义表单上更改计算的自定义字段的计算时， [!DNL Adobe Workfront] 可能会显示以下警告：

存在较小问题

[字段] 在多表单配置中使用，如果要更改此公式，则需要删除此字段并将其替换为包含所需计算的新字段。

## 原因

您尝试更改的包含计算自定义字段的至少两个自定义表单会附加到 [!DNL Workfront] 实例。

**示例：** 自定义表单A和B均附加到同一任务。 这两个表单都包含一个名为Profit的计算自定义字段。 尝试在自定义表单A的“利润”字段中编辑计算时，会遇到该错误。

无法更改其中一个表单中自定义字段的计算，因为这将与另一个表单中同一字段中的公式冲突。
要解决此冲突，您必须找到附加具有相同计算自定义字段的多个表单的对象，然后执行以下操作之一：

* 从对象中删除其中一个表单。
* 根据需要更改计算，但在附加到对象的所有自定义表单中执行此操作。
* 在附加到对象的所有自定义表单中，添加一个包含您需要的计算的新计算自定义字段，并将旧计算的自定义字段标记为过时。

本文就如何找到对象，然后通过这三种方法中的一种来解决问题。

## 查找附加自定义表单的对象 {#find-the-object-where-the-custom-forms-are-attached}

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 用户]** ![](assets/users-icon-in-main-menu.png).

1. 单击 **[!UICONTROL 自定义Forms]** > **[!UICONTROL 字段]**.
1. 应用 **[!UICONTROL 字段列表]** 查看以查找您尝试修改的计算字段，并记下使用该字段的每个自定义表单（例如，表单1、表单2、表单3）。
1. 单击 **[!UICONTROL Forms]**，然后应用 **[!UICONTROL 表单列表]** 中。
1. 单击 **[!UICONTROL 过滤器]** 下拉列表，然后 **[!UICONTROL 新建过滤器]**.

1. 单击 **[!UICONTROL 添加过滤器规则]**，然后开始键入“自定义表单名称”，并在该值显示在列表中时选择此值。
1. 选择 **[!UICONTROL 等于]** 对于过滤器修饰符，开始键入您在步骤1中记录的每个表单的名称，然后在显示时选择该名称。

   **示例：** 自定义表单名称等于表单1、表单2、表单3。

1. 单击 **[!UICONTROL 保存过滤器]**，然后命名新过滤器，并单击 **[!UICONTROL 保存过滤器]**.

1. 在表单列表中，记下显示在 **[!UICONTROL 类型]** 列。
1. 在步骤1中找到的每个自定义表单上，创建一个新的复选框自定义字段，其单个默认值为“是”。

   **示例：** 表单1上的字段1 =是，表单2上的字段2 =是，表单3上的字段3 =是。 这表示“表单1上存在计算的自定义字段”或“表单2上存在计算的自定义字段”等。

1. 在 **[!UICONTROL “搜索”图标]** ![](assets/search-icon.png) 在屏幕的右上角，单击 **[!UICONTROL 高级搜索]**.
1. 单击自定义表单的对象（如问题），然后单击 **[!UICONTROL 筛选结果]**，然后单击 **[!UICONTROL 添加过滤器]**.
1. 开始在 **[!UICONTROL 开始键入字段名称]** 字段，并在其显示在列表中时将其选中，然后选择 **[!UICONTROL 等于]** 和类型 **[!UICONTROL 是]** （无引号）。

   **示例：** 字段1等于（区分大小写）是。

1. 单击 **[!UICONTROL 添加过滤器]** 并将所有复选框字段添加到高级搜索。

   寻找所有可能的组合。

   **示例：** 使用您找到的组合构建多个过滤器，如下所示。 您应该找到具有多个附加自定义表单的对象，这些表单包含相同的计算字段。 您可能会发现以下情况：

   * 字段1=是+字段2 =是+字段3 =是（例如，无对象）
   * 字段1=是+字段2 =是（例如，无对象）
   * 字段1=是+字段3 =是（例如两个对象）

   这表示计算字段同时存在于表单1和表单3中，因为对应的复选框字段（字段1和字段3）存在于这些对象中。

   字段2 =是+字段3 =是（例如，无对象）

1. 继续阅读本文的以下章节之一：

   * [从对象中删除其中一个自定义表单，并在其中编辑计算](#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there)
   * [在所有附加的自定义表单的计算中进行相同的编辑](#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms)
   * [将包含已编辑计算的新计算字段添加到一个或多个附加的自定义表单中](#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms)

## 从对象中删除其中一个自定义表单，并在其中编辑计算 {#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there}

1. 查找附加自定义表单的对象，如 [查找附加自定义表单的对象](#find-the-object-where-the-custom-forms-are-attached) 在本文中，打开对象。
1. 从对象中删除其中一个自定义表单，然后保存该对象。

   >[!NOTE]
   >
   >要从从对象中删除的表单中添加字段，您可能需要编辑保留附加到对象的自定义表单。 这样，您就可以保留对象上的自定义数据信息。

1. 在删除的自定义表单中，编辑您最初尝试更新的自定义字段的计算，然后单击 **[!UICONTROL 保存]**.

   这次， [!DNL Workfront] 不应遇到冲突。

1. （可选）从自定义表单中删除复选框字段，或从 [!DNL Workfront].

## 在所有附加的自定义表单的计算中进行相同的编辑 {#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms}

>[!IMPORTANT]
>
>按照这些步骤操作时，数据会在已附加自定义表单的对象中丢失。 但是，如果计算字段引用的是静态字段，而不是计算字段，则可以使用 [!UICONTROL 重新计算自定义表达式] 对象上用于恢复丢失数据的选项

1. 查找附加自定义表单的对象，如 [查找附加自定义表单的对象](#find-the-object-where-the-custom-forms-are-attached) 在本文中。
1. 从附加到对象的所有自定义表单中删除该字段，然后保存表单。

1. 将包含新计算的自定义字段添加回自定义表单。

   >[!IMPORTANT]
   >
   >所有附加的自定义表单中的计算必须相同。

1. （可选）从表单中删除复选框字段或将其从 [!DNL Workfront].

## 将包含已编辑计算的新计算字段添加到一个或多个附加的自定义表单中 {#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms}

为避免丢失现有计算自定义字段中的数据，或者如果您只需要在附加到您找到对象的其中一个自定义表单中进行编辑计算，请执行以下操作：

1. 查找附加自定义表单的对象，如 [查找附加自定义表单的对象](#find-the-object-where-the-custom-forms-are-attached) 在本文中。
1. 向一个或多个表单中添加新的计算量度自定义字段，其中包含您需要的计算。
1. 重命名旧的计算自定义字段 **过时**.

   在附加到对象的所有表单上，此旧的计算量度自定义表单会保留其历史数据，但用户将停止使用该数据。

   >[!IMPORTANT]
   >
   >较旧的字段可能在其他计算的自定义字段中引用，因此您需要在更改其名称后更新这些计算。

1. （可选）从表单中删除复选框字段或从Workfront中删除它们。

<!--
<blockquote data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Problem</h2>
<p>You get the following error while editing a calculated Custom Field on a custom form: </p>
<p><em>"<Name of custom field> field is used in a multi-form configuration, if you would like to change this formula you will need to remove this field and replace it with a new one containing the desired calculation."</em> </p>
<h2>Cause</h2>
<p>The error occurs because the following setup exists: currently you have at least one object in your system that has multiple custom forms attached. The calculated field you are editing exists on multiple forms attached to these objects.</p>
<p>You cannot have the same calculated field with different calculations on the same object. For this reason, the system does not allow you to make a change which will result in calculations being different.</p>
<p><a href="../../Resources/Images/Admin and setup/Tips, Tricks, and Troubleshooting/Calculated_field_error.png" class="MCXref xref" xrefformat="{para}"><img src="assets/calculated-field-error.png" alt="" width="542" height="272"></a> </p>
<p>For example, you have a task with custom forms A and B attached to it. Both forms contain the same calculated field, Field 1. You encounter this error when you try to edit the calculation for Field 1 on custom form A. </p>
<h2>Solution</h2>
<p>Remove the field from the custom form and replace it with a new one containing the desired calculation.  </p>
<p>To understand what custom forms are attached to objects, you can build a report for those objects and reference the Category Name field in the view of the report.<br>For more information about referencing custom forms in reports, see the "Referencing Custom Forms in a Report View (Column)" section in <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/reference-custom-form-report.md" class="MCXref xref" xrefformat="{para}">Reference a custom form in a report</a>.</p>
<p>To understand what custom form contains a Custom Field, see the "Accessing Custom Forms and Fields" section in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md" class="MCXref xref" xrefformat="{para}">Custom forms overview</a>.</p>
<p>For more information about creating a custom form and adding or removing fields from it, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Create or edit a custom form</a>.</p>
</blockquote>
-->
