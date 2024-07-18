---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''错误消息：存在轻微问题。 该字段用于多表单配置'
description: 在自定义表单的计算自定义字段中更改计算时，如果出现一则错误消息，告知您该字段已在多表单配置中使用，则需要将该字段替换为包含要使用的计算的新字段。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 43668525-5572-4d82-8eed-0e320249f296
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 0%

---

# 错误消息：存在轻微问题。 该字段用于多表单配置

## 问题

在自定义表单上更改计算自定义字段的计算时，[!DNL Adobe Workfront]可能会显示以下警告：

存在较小问题

[字段]用于多表单配置，如果要更改此公式，您需要删除此字段并用包含所需计算的新字段替换它。

## 原因

至少两个包含您尝试更改的计算自定义字段的自定义表单被附加到[!DNL Workfront]实例中的单个对象。

**示例：**&#x200B;自定义表单A和B都附加到同一任务。 两个表单都包含一个名为“利润”的计算自定义字段。 当您尝试在自定义表单A的利润字段中编辑计算时，会遇到错误。

您无法更改其中一个表单中自定义字段的计算，因为这将与另一个表单中相同字段中的公式冲突。
要解决此冲突，您必须找到附加了具有相同计算自定义字段的多个表单的对象，然后执行以下操作之一：

* 从对象中删除其中一个表单。
* 根据需要更改计算，但在附加到对象的所有自定义表单中更改计算。
* 在附加到对象的所有自定义表单中，添加新的计算自定义字段（包含所需的计算），并将旧的计算自定义字段标记为过时。

本文介绍如何通过这三种方法之一找到对象并解决问题。

## 查找附加自定义表单的对象 {#find-the-object-where-the-custom-forms-are-attached}

1. 单击[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 用户]** ![](assets/users-icon-in-main-menu.png)。

1. 单击&#x200B;**[!UICONTROL 自定义Forms]** > **[!UICONTROL 字段]**。
1. 应用&#x200B;**[!UICONTROL 字段列表]**&#x200B;视图以查找您尝试修改的计算字段，并记下使用它的每个自定义表单（例如，表单1、表单2、表单3）。
1. 单击&#x200B;**[!UICONTROL Forms]**，然后应用&#x200B;**[!UICONTROL 表单列表]**&#x200B;视图。
1. 单击&#x200B;**[!UICONTROL 筛选器]**&#x200B;下拉列表，然后单击&#x200B;**[!UICONTROL 新筛选器]**。

1. 单击&#x200B;**[!UICONTROL 添加筛选器规则]**，然后开始输入“自定义表单名称”，并在该名称显示在列表时将其选定。
1. 为筛选器修饰符选择&#x200B;**[!UICONTROL 等于]**，开始键入您在步骤1中记下的每个表单的名称，然后在显示时将其选定。

   **示例：**&#x200B;自定义表单名称等于表单1、表单2、表单3。

1. 单击&#x200B;**[!UICONTROL 保存筛选器]**，为新筛选器命名，然后单击&#x200B;**[!UICONTROL 保存筛选器]**。

1. 在表单列表中，记下&#x200B;**[!UICONTROL 类型]**&#x200B;列中显示的过滤器对象类型，如“任务”或“问题”。
1. 在步骤1中找到的每个自定义表单上，创建一个新的复选框自定义字段，其单个默认值是“是”。

   **示例：**&#x200B;表单1上的字段1 =是，表单2上的字段2 =是，表单3上的字段3 =是。 这意味着“表单1上存在计算自定义字段”，或者“表单2上存在计算自定义字段”等。

1. 在屏幕右上角的&#x200B;**[!UICONTROL 搜索图标]** ![](assets/search-icon.png)中，单击&#x200B;**[!UICONTROL 高级搜索]**。
1. 单击自定义表单的对象（如问题），单击&#x200B;**[!UICONTROL 筛选结果]**，然后单击&#x200B;**[!UICONTROL 添加筛选器]**。
1. 开始在&#x200B;**[!UICONTROL 开始键入字段名称]**&#x200B;字段中键入复选框字段的名称，并在该字段显示在列表中时将其选中，然后选择&#x200B;**[!UICONTROL 等于]**&#x200B;并在以下框中键入&#x200B;**[!UICONTROL 是]**（不带引号）。

   **示例：**&#x200B;字段1等于（区分大小写）是。

1. 单击&#x200B;**[!UICONTROL 添加筛选器]**&#x200B;并将所有复选框字段添加到高级搜索。

   寻找所有可能的组合。

   **示例：**&#x200B;使用您找到的组合生成多个筛选器，如下所示。 您应该查找具有多个附加自定义表单的对象，这些表单包含相同的计算字段。 您可能会发现以下场景：

   * 字段1 =是+字段2 =是+字段3 =是（例如，无对象）
   * 字段1 =是+字段2 =是（例如，无对象）
   * 字段1 =是+字段3 =是（例如，两个对象）

   这表示计算字段在表单1和表单3中均存在，因为相应的复选框字段（字段1和字段3）存在于这些对象中。

   字段2 =是+字段3 =是（例如，无对象）

1. 继续阅读本文中的以下章节之一：

   * [从对象中删除其中一个自定义表单，并在其中编辑计算](#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there)
   * [在所有附加的自定义表单中进行相同的编辑](#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms)
   * [将包含已编辑计算的新计算字段添加到一个或多个附加的自定义表单](#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms)

## 从对象中删除其中一个自定义表单，并在其中编辑计算 {#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there}

1. 查找附加自定义表单的对象，如[在本文章中查找附加自定义表单的对象](#find-the-object-where-the-custom-forms-are-attached)中所述，然后打开该对象。
1. 从对象中删除其中一个自定义表单，然后保存该对象。

   >[!NOTE]
   >
   >若要从从对象中删除的表单添加字段，您可能需要编辑仍附加到对象的自定义表单。 这样，您可以保留对象上的自定义数据信息。

1. 在您删除的自定义表单中，编辑您最初尝试更新的自定义字段的计算，然后单击&#x200B;**[!UICONTROL 保存]**。

   此时，[!DNL Workfront]不应遇到冲突。

1. （可选）从自定义表单中删除复选框字段或从[!DNL Workfront]中删除它们。

## 在所有附加的自定义表单中进行相同的编辑 {#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms}

>[!IMPORTANT]
>
>执行这些步骤时，已附加自定义表单的对象中的数据将丢失。 但是，如果计算字段引用了静态字段而不是计算字段，则可以在对象上使用[!UICONTROL 重新计算自定义表达式]选项来还原丢失的数据

1. 查找附加自定义表单的对象，如本文中[查找附加自定义表单的对象](#find-the-object-where-the-custom-forms-are-attached)中所述。
1. 从附加到对象的所有自定义表单中删除字段，然后保存表单。

1. 将包含新计算的自定义字段添加回自定义表单。

   >[!IMPORTANT]
   >
   >所有附加的自定义表单中的计算必须相同。

1. （可选）从表单中删除复选框字段或从[!DNL Workfront]中删除它们。

## 将包含已编辑计算的新计算字段添加到一个或多个附加的自定义表单 {#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms}

为避免丢失现有计算自定义字段中的数据，或者如果您只需在附加到所找到对象的其中一个自定义表单中进行编辑计算，请执行以下操作：

1. 查找附加自定义表单的对象，如本文中[查找附加自定义表单的对象](#find-the-object-where-the-custom-forms-are-attached)中所述。
1. 将包含所需计算的新计算自定义字段添加到一个或所有表单。
1. 重命名旧的计算自定义字段&#x200B;**过时**。

   在附加到对象的所有表单上，此旧的计算自定义表单会保留其历史数据，但用户会停止使用它。

   >[!IMPORTANT]
   >
   >旧字段可能会被其他计算自定义字段引用，因此您需要在更改其名称后更新这些计算。

1. （可选）从表单中删除复选框字段或从Workfront中删除这些字段。

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
</blockquote>
-->
