---
user-type: administrator
product-area: system-administration
keywords: 创建，自定义，表单，复制，基本，其他
navigation-topic: create-and-manage-custom-forms
title: 复制自定义表单以使用旧版生成器创建新表单
description: 您可以基于现有表单创建新的自定义表单。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 946a726e-af88-413c-abe3-55fbc7486380
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# 复制自定义表单以使用旧版生成器创建新表单

您可以基于现有表单创建新的自定义表单。

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

## 复制自定义表单以创建新表单

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms。**
1. 选择要用作新自定义表单基础的自定义表单，然后单击 **复制**.
1. 在 **自定义表单复制** 框中，键入以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">表单名称</td> 
      <td>为复制的表单键入名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">表单类型 </p> </td> 
      <td> <p>在 <b>表单类型</b> 框中，选择要使用自定义表单的对象类型，然后单击要删除的任何类型旁边的X。 列表中已禁用与该表单关联的类型。</p> 
      <p><img src="assets/copy-form-obj-types.png"></p> 
      <p>表单必须至少与一种对象类型关联。</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **复制表单**.

   在原始表单中，如果计算字段引用与您添加到新表单的对象类型不兼容的字段，则会出现一条消息，提示您更改这些字段中的计算。

   同样，如果原始表单上分区界限的访问选项与您添加到新表单的对象类型不兼容，则会出现一条消息，提示您调整该选项。

1. 选择您刚刚复制的表单，然后单击 **编辑**.
1. 对表单进行任何更改，如以下文章所述：

   * [复制自定义表单以使用旧版表单生成器创建新表单](#Add2)
   * [使用旧版表单生成器将计算数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [使用旧版表单生成器定位自定义表单中的自定义字段和小部件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [使用旧版表单生成器添加或编辑自定义表单中的资产小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [使用旧版表单生成器重新使用自定义表单中现有的计算自定义字段](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [使用旧版表单生成器将显示逻辑和跳过逻辑添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [使用旧版表单生成器预览并完成自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

1. （可选）单击之后 **保存+关闭**，将表单附加到要使用该表单的对象，如中所述 [将自定义表单添加到对象](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
