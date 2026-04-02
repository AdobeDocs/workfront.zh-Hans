---
title: 限制对自定义字段中财务数据的访问
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 创建自定义字段时，您可以定义可选设置以限制对财务数据的访问。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
source-git-commit: 5cdaccd9381b02f183b837208eaac4389b0b7a24
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 6%

---


# 限制对自定义字段中财务数据的访问

{{highlighted-preview-article-level}}

创建自定义字段时，您可以定义可选设置以限制对财务数据的访问。 这样，在访问级别中设置了特定权限的用户就可以查看数据，并且防止他们查看不应访问的财务数据。

有关创建自定义字段的信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

有关访问级别的信息，请参阅[访问级别概述](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)。 有关共享和权限的信息，请参阅[对象共享权限概述](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td>“任一”</td> 
  </tr>  
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>对自定义表单的管理访问权限</td> 
  </tr>  
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 限制对自定义字段上财务数据的访问

1. 创建新的自定义表单或打开现有表单。

   有关信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

1. 将自定义字段添加到表单或选择现有字段。

   可根据财务数据访问限制这些字段类型：

   * 单行文本
   * 段落
   * 单选下拉菜单
   * 多选下拉框
   * 复选框组
   * 单选按钮
   * 外部查找
   * 多选外部查找
   * 已计算

1. 在&#x200B;**格式**&#x200B;字段中，选择&#x200B;**货币**。

   >[!NOTE]
   >
   >对于计算字段，允许使用任何格式。 所有其他字段类型必须使用&#x200B;**货币**&#x200B;格式，否则&#x200B;**财务权限类型**&#x200B;字段将不可用。

1. （可选）仅对于计算字段，打开&#x200B;**自动权限**&#x200B;选项以允许财务权限自动来自公式中的字段。

1. 为&#x200B;**财务权限类型**&#x200B;选择一个选项。

   用户必须具有此财务权限类型，才能在表单上查看或编辑此自定义字段。

   * **不需要权限：**&#x200B;所有用户都可以看到此字段
   * **常规：**&#x200B;用户必须具有编辑或查看常规财务的权限
   * **帐单：**&#x200B;用户必须具有编辑或查看记帐费率的权限
   * **成本：**&#x200B;用户必须具有编辑或查看成本费率的权限

   对于已计算的字段：

   * 如果已打开&#x200B;**自动权限**&#x200B;字段，**财务权限类型**&#x200B;字段不可用于手动设置权限。
   * 公式中使用的字段决定了权限字段是否有效。 如果权限字段为空（并且未打开自动权限），则公式中的字段不支持财务权限。
   * 需要访问公式中的所有字段。 例如，如果在计算字段中使用了两个字段，其中一个字段应用了计费权限，而另一个字段应用了成本权限，则用户必须具有查看计费和成本费率的权限才能查看计算值。

1. 要保存更改，请单击&#x200B;**应用**&#x200B;并继续构建表单。

   或

   单击&#x200B;**保存并关闭**。

## 示例

以下两个项目与一个用户共享：

* 用户有权编辑第一个项目的所有财务选项
* 用户有权查看第二个项目的记帐费率和一般财务

用户编辑第一个项目时，自定义表单上的所有财务字段都是可编辑的。 当用户编辑第二个项目时，设置为&#x200B;**帐单**&#x200B;或&#x200B;**常规**&#x200B;的字段为仅查看字段，设置为&#x200B;**成本**&#x200B;的字段不可见。

当用户在列表或报告中查看项目时：

* 财务字段可根据权限和报表设置进行查看或编辑
* 如果用户没有权限查看财务字段，则字段为空

导出项目详细信息将显示与列表相同的财务字段值（或空白字段）。

批量编辑这两个项目时，billing和general finance字段显示为只读，cost字段显示不适用。

