---
user-type: administrator
product-area: system-administration
keywords: 创建，自定义，表单，复制，基础，其他
navigation-topic: create-and-manage-custom-forms
title: 复制自定义表单以使用旧版生成器创建新表单
description: 您可以基于现有自定义表单创建新的自定义表单。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 946a726e-af88-413c-abe3-55fbc7486380
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 复制自定义表单以使用旧版生成器创建新表单

<span class="preview">此页面上高亮显示的信息是指尚未普遍可用的功能。 它只能在“预览”环境中用于所有客户，或者在“生产”环境中用于启用快速版本的客户。</span>

<span class="preview">有关快速版本的信息，请参阅 [为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">有关当前版本的信息，请参阅 [2024年第二季度发行版概述](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

您可以基于现有自定义表单创建新的自定义表单。

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

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 复制自定义表单以创建新表单

{{step-1-to-setup}}

1. 单击 **自定义Forms。**
1. 选择要用作新自定义表单基础的自定义表单，然后单击 **复制** <span class="preview">或 ![“复制”图标](assets/copy-icon.png).</span>
1. 在 **自定义表单复制** 在出现的框中，键入以下信息：

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
      <td> <p>在 <b>表单类型</b> 框中，选择要使用自定义表单的对象类型，然后单击要删除的任何类型旁边的X。 列表中已禁用与表单关联的类型。</p> 
      <p><img src="assets/copy-form-obj-types.png"></p> 
      <p>表单必须至少与一个对象类型关联。</p> 
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
   * [使用旧版表单生成器将计算的数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [使用旧版表单生成器将自定义字段和小组件放置在自定义表单中](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [使用旧版表单生成器添加或编辑自定义表单中的资产小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [使用旧版表单生成器重新使用自定义表单中现有的计算自定义字段](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [使用旧版表单生成器向自定义表单添加显示逻辑和跳过逻辑](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [使用旧版表单生成器预览并完成自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

1. （可选）单击之后 **保存+关闭**，将表单附加到要使用该表单的对象，如中所述 [向对象添加自定义表单](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
