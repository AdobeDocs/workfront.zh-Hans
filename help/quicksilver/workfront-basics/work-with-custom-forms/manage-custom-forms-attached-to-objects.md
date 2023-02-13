---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: 管理附加到对象的自定义表单
description: 您可以更新附加到一个对象的自定义表单的显示顺序，删除它们，或批量编辑自定义表单在多个对象上的显示方式。
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 6580fec18982215dbc2535d5f2ab159fc32ac3f5
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 0%

---

# 管理附加到对象的自定义表单

您可以更新附加到一个对象的自定义表单的显示顺序，删除它们，或批量编辑自定义表单在多个对象上的显示方式。

## 访问要求

您必须具有以下访问权限才能执行本文中描述的操作：

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
   <td> <p>编辑对您管理自定义表单的对象的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>为您管理自定义表单的对象贡献权限或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

* 您的Workfront管理员或对自定义表单具有管理访问权限的计划用户必须在您的环境中创建自定义表单。 有关更多信息，请参阅 [创建或编辑自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* 必须将自定义表单附加到对象。

   有关如何将自定义表单应用到对象的信息，请参阅 [将自定义表单添加到对象](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 对附加到对象的多个自定义表单重新排序 {#reorder-multiple-custom-forms-attached-to-an-object}

1. 转到要更改添加的自定义表单顺序的对象，然后开始编辑该对象。

   **示例：** 例如，要管理项目的自定义表单，请转到项目，单击 **更多** 菜单 ![](assets/more-icon.png)，然后单击 **编辑** .

1. 在 **自定义Forms** 部分，单击 ![](assets/move-icon---dots.png) 图标。 对于所有其他对象，单击 **管理Forms**. 仅当至少将一个自定义表单附加到对象时，才会显示此选项。
1. 拖动表单 ![](assets/move-icon---dots.png) 到列表中的新位置。
1. 对于项目、任务和问题自定义表单，请单击 **保存**.

   对于所有其他对象，单击 **我已经管好了** > **保存更改**.

## 从对象中删除自定义表单 {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>从对象中删除自定义表单时，表单的自定义字段中捕获的所有信息都将丢失，无法恢复。

1. 转到要删除自定义表单的对象，然后开始编辑该对象。

   例如，转到项目，单击 **更多** 菜单 ![](assets/more-icon.png)，然后单击 **编辑** .

1. 单击 **自定义Forms**.
1. 对于项目、任务和问题自定义表单，请单击 **X** 图标，以将其从对象中删除。

   对于所有其他对象，单击 **管理Forms**，然后单击 **X** 图标，以将其从对象中删除。

1. 单击&#x200B;**保存**。

## 管理包含相同自定义字段的多个自定义表单

同一字段可能显示在附加到同一对象的多个自定义表单上。 在这种情况下，请考虑以下事项：

* 所有形式中字段的值都相同。

   同一对象上不同表单上的相同字段不能具有不同的值。

* 如果两个不同对象具有相同的计算字段，则其计算必须相同，以避免出现错误。 有关将计算字段添加到包括多个表单的自定义表单的信息，请参阅 [将计算数据添加到自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) .

## 批量编辑对象时编辑多个自定义表单

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section will need to be edited when the bulk Edit box is released to NWE; add some screen shots for NWE) </p>
-->

在批量编辑应用了多个自定义表单的对象时，您可以编辑在这些对象上显示自定义表单的方式，以及编辑自定义表单中的常用字段。

只有附加到所有选定对象的自定义表单才能在批量编辑中进行编辑。

要在批量编辑对象时编辑多个自定义表单，请执行以下操作：

1. 在列表对象中，选择附加了自定义表单的对象，然后单击 **编辑** 图标 ![](assets/edit-icon.png).
1. 单击 **自定义Forms**.

   您只能编辑附加到所有选定对象的自定义表单。

   仅附加到某些对象的自定义表单不显示。

1. 开始编辑自定义表单上的字段。

   编辑字段时，该字段上会显示一个可视指示器，表示该字段已编辑。

   如果一个字段包含在多个自定义表单中，则当您更新其中一个表单上的字段时，每个表单上的这些字段的所有值都会更新。

1. 单击 **选择** 下拉菜单，然后选择要添加到所有选定对象的其他表单。

   在应用其他表单时，请考虑以下事项：

   * 对象最多可以有10个自定义表单。
   * 仅当表单尚未应用于您正在编辑的任何对象时，才能应用表单。 已附加到其中一个对象的表单不会显示在下拉菜单中。
   * 应用附加表单后，表单与其他表单具有共同关系的任何字段都会显示在 **常用字段** ，且可以编辑。

1. （可选）如果向所有对象添加了自定义表单，但尚未保存对象，则可以更改自定义表单在对象上的显示顺序。

   有关更改表单顺序的更多信息，请参阅 [对附加到对象的多个自定义表单重新排序](#reorder-multiple-custom-forms-attached-to-an-object) 在本文中。

1. 单击 **删除表单** 从对象中删除自定义表单。

   有关从对象中删除自定义表单的更多信息，请参阅 [从对象中删除自定义表单](#remove-a-custom-form-from-an-object).

   从多个对象中批量删除表单时，请考虑以下事项：

   * 如果您对表单进行了更改，删除该表单会导致您的更改丢失，并且无法恢复这些更改。
   * 删除表单后，该表单中 **常用字段** 部分将从此部分删除，在此不再进行编辑。

1. 单击 **还原表单** 要将表单恢复为编辑对象之前的状态，请执行以下操作：
1. （可选）单击表单名称旁边的折叠箭头可一次折叠一个表单。

   或

   单击 **折叠Forms** 可同时折叠所有表单。

1. （可选）单击表单名称旁边的展开箭头可一次展开一个表单。

   或

   单击 **展开Forms** 以同时展开所有表单。 

1. 单击 **保存更改**.
