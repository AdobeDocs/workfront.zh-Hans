---
title: 从副本创建表单
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以使用表单设计器从副本创建自定义表单。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 578a8bd5-d93f-4327-bb4f-2c17b91b170a
source-git-commit: 15ac51cc13eeb57d2de194a9a6ceec7683acfbe6
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 1%

---

# 从副本创建表单

<!--add preview tags and see below in comment out-->

您可以基于现有自定义表单设计新的自定义表单。 您可以将自定义表单附加到不同的Workfront对象，以捕获有关这些对象的数据。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>对自定义表单的管理访问权限</p> </td> 
  </tr>  
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 复制自定义表单以创建新表单

{{step-1-to-setup}}

1. 单击&#x200B;**自定义Forms。**
1. 选择要用作新自定义表单基础的自定义表单，然后单击![复制图标](assets/copy-icon.png)。
1. 在出现的&#x200B;**自定义表单副本**&#x200B;框中，键入以下信息：

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
      <td> <p>在<b>表单类型</b>框中，选择要使用自定义表单的对象类型，然后单击要删除的任何类型旁边的X。 列表中已禁用与表单关联的类型。</p> 
      <p><img src="assets/copy-form-obj-types-040524.png"></p> 
      <p>表单必须至少与一个对象类型关联。</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**复制**。

   在原始表单中，如果计算字段引用与您添加到新表单的对象类型不兼容的字段，则会出现一条消息，提示您更改这些字段中的计算。

   同样，如果原始表单上分区界限的访问选项与您添加到新表单的对象类型不兼容，则会出现一条消息，提示您调整该选项。

1. 选择您刚刚复制的表单，然后单击![编辑图标](assets/edit-icon.png)。
1. 对表单进行任何更改，如[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)文章的以下部分所述：

   * [重用已在其他自定义表单中使用的现有字段或构件](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [添加文本字段](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
   * [添加计算字段](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
   * [添加单选按钮、复选框组和下拉列表](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
   * [添加预输入和日期字段](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-typeahead-and-date-fields)
   * [添加图像、PDF和视频](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
   * [添加Adobe XD文件](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)
   * [添加Planning连接字段](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-planning-connection-fields)

1. （可选）单击&#x200B;**保存并关闭**&#x200B;后，将表单附加到要使用表单的对象，如[将自定义表单添加到对象](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)中所述。
