---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 从系统中删除自定义字段或构件
description: 为了提高系统性能并使表单更易于用户使用，您可能希望从系统中删除不再使用的自定义字段和小部件。
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# 从系统中删除自定义字段或构件

为了提高系统性能并使表单更易于用户使用，您可能希望从系统中删除不再使用的自定义字段和小部件。

>[!CAUTION]
>
>删除自定义字段也会在填写附加到对象的自定义表单时删除用户在该字段输入的所有自定义数据。 已删除的数据将无法恢复。
>
>您可以查看所有使用要删除的自定义字段的自定义表单和报表，以评估可能会产生的影响。 有关更多信息，请参阅 [查看使用特定自定义字段或小部件的所有自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) 和 [查看使用特定自定义字段或小部件的所有报表](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>或者，有关可用于避免丢失不再使用字段中数据的解决方法，请参阅 [删除自定义字段而不丢失用户输入的数据](#remove-a-custom-field-without-losing-data-that-users-have-entered) 本文章中。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront计划*</p> </td> 
   <td>任何</td> 
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

&#42;要了解您拥有的计划、许可证类型或访问级别配置，请与Workfront管理员联系。

## 从系统中删除自定义字段或构件

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms。**
1. 单击 **字段** 选项卡。
1. 选择自定义字段或构件，然后单击 **删除**.
1. 如果您确实想要永久删除项目，并（对于自定义字段）删除所附加对象的全部关联数据，请单击 **是的，删除它**.

## 删除自定义字段而不丢失用户输入的数据 {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>从自定义表单中删除包含500多个字段和小部件的自定义字段无法撤消。 如果移除该字段，则在表单中的字段和小组件少于500个之前，无法重新添加它。

1. 确定要从原始自定义表单中删除的自定义字段，但此时不要删除它们。
1. 创建新的自定义表单：

   1. 将自定义字段添加到要从原始自定义表单中删除的新表单。

      * 如果您使用的是自定义表单生成器，请参阅 [在自定义表单中重用自定义字段或小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).
      * 如果您使用的是表单设计器，请参阅 [向自定义表单中添加新字段或现有字段](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form).

   1. 保存新的自定义表单。

1. 将自定义表单的访问权限限制为仅授予具有管理访问权限的用户，如中所述 [共享自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
1. 将新的自定义表单应用于已应用原始自定义表单的对象，如中所述 [向对象添加自定义表单](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   将新的自定义表单应用于这些对象可确保历史报表数据不受影响。

1. 修改原始自定义表单，并删除添加到新表单中的自定义字段（在步骤2中）。

   您从原始自定义表单中删除的字段现在仅可用于您创建的新自定义表单。 用户可以在对象上查看自定义表单，但具有管理访问权限的用户无法修改自定义表单。
