---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 使用旧版表单生成器定位自定义表单中的自定义字段和小部件
description: 您可以在自定义表单中重新定位自定义字段和小部件。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f96425e3-8e20-43ac-8340-915538ae5886
source-git-commit: ac5b7e0237dbcaea14010eda658f7d5a6be089cc
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# 使用旧版表单生成器定位自定义表单中的自定义字段和小部件

您可以在自定义表单中重新定位自定义字段和小部件。

有关自定义表单中的自定义字段和小部件的信息，请参阅 [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 和 [在自定义表单中添加或编辑资源小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

## 在自定义表单中放置自定义字段和小部件

1. 开始创建或编辑自定义表单，如中所述 [使用旧版表单生成器创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 向表单中添加自定义字段和小部件，如中所述 [使用旧版表单生成器将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 和 [使用旧版表单生成器添加或编辑自定义表单中的资产小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

1. （可选）要将自定义字段和小组件放置在同一行，请将一个字段和小组件拖动到彼此旁边，直到它们之间出现一行。

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* 您可以使用 **预览** 按钮，了解自定义字段和小组件在表单中的显示方式。
>* 描述性文本字段不能共享行。
>* 自定义字段和小组件在表单中的显示方式可能并不总是相同，具体取决于用户查看时可用的屏幕空间量。 例如，如果水平空间有限，则一行字段中的第三个字段可能会换成下一行字段。


1. （可选）要将自定义字段或构件放置到另一个字段的上方或下方，请将其拖动到上面或下方，直到项目之间出现一条水平蓝色线。
1. 单击 **应用**.
1. 如果要继续以其他方式构建自定义表单，请继续阅读以下文章之一：

   * [使用旧版表单生成器将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [使用旧版表单生成器添加或编辑自定义表单中的资产小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [使用旧版表单生成器将计算数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [使用旧版表单生成器向自定义表单添加分区界限](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [使用旧版表单生成器将显示逻辑和跳过逻辑添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [使用旧版表单生成器预览并完成自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
