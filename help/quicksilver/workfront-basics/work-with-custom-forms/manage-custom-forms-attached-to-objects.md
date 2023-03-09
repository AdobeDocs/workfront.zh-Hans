---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: 管理附加到对象的自定义表单
description: 您可以更新附加到某个对象的自定义表单的显示顺序，删除它们，或者批量编辑自定义表单在多个对象上的显示方式。
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 23257f11b0795aa1f1e422923f6d596017c58126
workflow-type: tm+mt
source-wordcount: '1120'
ht-degree: 0%

---

# 管理附加到对象的自定义表单

<span class="preview">此页面上高亮显示的信息是指尚未公开发布的功能。 它仅在“预览”环境中可用。</span>

您可以更新附加到某个对象的自定义表单的显示顺序，删除它们，或者批量编辑自定义表单在多个对象上的显示方式。

## 访问要求

您必须具有以下权限才能执行本文中所述的操作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑您对其管理自定义表单的对象的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>为您管理自定义表单的对象分配权限或更高</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

* 您的Workfront管理员或对自定义表单具有管理访问权限的计划用户必须在您的环境中创建自定义表单。 有关更多信息，请参阅 [创建或编辑自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* 您必须将自定义表单附加到对象。

   有关如何将自定义表单应用于对象的信息，请参阅 [将自定义表单添加到对象](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 重新排序附加到对象的多个自定义表单 {#reorder-multiple-custom-forms-attached-to-an-object}

1. 转到要更改所添加自定义表单顺序的对象，然后开始编辑该对象。

   **示例：** 例如，要管理项目的自定义表单，请转到项目，单击 **更多** 菜单 ![](assets/more-icon.png)，然后单击 **编辑** .

1. 在 **自定义Forms** 项目、任务和问题的部分，单击 ![](assets/move-icon---dots.png) 自定义表单名称旁边的图标。 对于所有其他对象，单击 **管理Forms**. 仅当至少将一个自定义表单附加到对象时，才会显示此选项。
1. 拖动表单 ![](assets/move-icon---dots.png) 到列表中的新位置。
1. 对于项目、任务和问题自定义表单，请单击 **保存**.

   对于所有其他对象，单击 **我已完成管理** > **保存更改**.

## 从对象中删除自定义表单 {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>从对象中删除自定义表单时，在表单的自定义字段中捕获的所有信息都将丢失，并且无法恢复。

1. 转到要删除自定义表单的对象并开始编辑该对象。

   例如，转到某个项目，单击 **更多** 菜单 ![](assets/more-icon.png)，然后单击 **编辑** .

1. 单击 **自定义Forms**.
1. 对于项目、任务和问题自定义表单，单击 **X** 图标来将其从对象中删除。

   对于所有其他对象，单击 **管理Forms**，然后单击 **X** 图标来将其从对象中删除。

1. 单击&#x200B;**保存**。

## 管理包含相同自定义字段的多个自定义表单

同一字段可能显示在附加到同一对象的多个自定义表单上。 在这种情况下，请考虑以下事项：

* 字段的值在所有表单中都是相同的。

   对于附加到同一对象的不同表单上的相同字段，不能有不同的值。

* 如果两个不同对象具有相同的计算字段，则其计算必须相同以避免错误。 有关将计算字段添加到包含多个表单的自定义表单的信息，请参阅 [将计算的数据添加到自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) .

## 批量编辑对象时管理多个自定义表单

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
><span class="preview">有关在预览环境中批量管理项目自定义表单的信息，请参阅文章 [编辑项目](../../manage-work/projects/manage-projects/edit-projects.md)</span>.

批量编辑应用了多个自定义表单的对象时，您可以编辑自定义表单在这些对象上的显示方式，以及编辑自定义表单中的常用字段。

只有附加到所有选定对象的自定义表单才能进行批量编辑。

要在批量编辑对象时编辑多个自定义表单，请执行以下操作：

1. 在列表对象中，选择附加了自定义表单的对象，然后单击 **编辑** 图标 ![](assets/edit-icon.png).
1. 单击 **自定义Forms**.

   您只能编辑附加到所有选定对象的自定义表单。

   仅附加到某些对象的自定义表单不显示。

1. 开始编辑自定义表单上的字段。

   编辑字段时，该字段上会显示一个可视指示符，表示该字段已编辑。

   如果一个字段包含在多个自定义表单中，则当您更新其中一个表单中的字段时，这些字段的所有值都会在每个表单中更新。

1. 单击 **进行选择** 下拉菜单，并选择要添加到所有选定对象的其他表单。

   应用其他表单时，请考虑以下事项：

   * 对象最多可以有10个自定义表单。
   * 仅当尚未将表单应用于正在编辑的任何对象时，才可以应用表单。 已附加到其中一个对象的表单不会显示在下拉菜单中。
   * 应用附加表单后，该表单与其他表单共有的所有字段都将显示在 **常用字段** 区域，并且可以编辑它们。

1. （可选）如果已将自定义表单添加到所有对象，但尚未保存这些对象，则可以更改自定义表单在对象上的显示顺序。

   有关更改表单顺序的更多信息，请参阅 [重新排序附加到对象的多个自定义表单](#reorder-multiple-custom-forms-attached-to-an-object) 本文章中。

1. 单击 **删除表单** 从对象中删除自定义表单。

   有关从对象中删除自定义表单的更多信息，请参阅 [从对象中删除自定义表单](#remove-a-custom-form-from-an-object).

   从多个对象中批量删除表单时，请考虑以下事项：

   * 如果您对表单进行了更改，则删除它会导致更改丢失，并且无法恢复。
   * 删除表单后，该表单中位于以下位置的任何字段： **常用字段** 部分将从此部分中删除，无法再在此处编辑。

1. 单击 **恢复表单** 将表单恢复到编辑对象之前所处的状态。
1. （可选）单击表单名称旁边的折叠箭头，一次折叠一个表单。

   或

   单击 **折叠Forms** 以同时折叠所有表单。

1. （可选）单击表单名称旁边的展开箭头，一次展开一个表单。

   或

   单击 **展开Forms** 以同时展开所有表单。 

1. 单击 **保存更改**.
