---
product-area: projects;user-management
keywords: 附加，应用
navigation-topic: work-with-custom-forms
title: 将自定义表单添加到对象
description: 您可以将现有的自定义表单添加到下面列出的任何对象中。 自定义表单包含自定义字段，您可以在其中存储有关对象的信息。
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 23257f11b0795aa1f1e422923f6d596017c58126
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 1%

---

# 将自定义表单添加到对象

<span class="preview">此页面上高亮显示的信息是指尚未公开发布的功能。 它仅在“预览”环境中可用。</span>

您可以将现有的自定义表单添加到下面列出的任何对象中。 自定义表单包含自定义字段，您可以在其中存储有关对象的信息。

* 项目（包括业务案例）
* 任务
* 问题
* 公司
* 项目组合
* 项目群
* 文档
* 用户
* 迭代
* 费用
* 开票记录

您只能将自定义表单添加到为其创建表单的对象类型。

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
   <td> <p>编辑您对其管理自定义表单的对象的访问权限</p> <p><b>注释</b></p>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理要为其附加自定义表单的对象的权限。</p> <p>查看自定义表单或更高权限，并具有以下权限： <b>附加到自定义数据</b> 对象（项目、任务和问题）。 有关更多信息，请参阅 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">共享自定义表单</a>.</p> <p>重要信息：如果您没有对自定义Forms具有管理访问权限的计划许可证，则您必须至少具有查看自定义表单的特定权限，如中所述 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">共享自定义表单</a>. 即使表单在系统范围内可见，也必须向您授予这些权限。 </p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

您的Workfront管理员或具有自定义表单的计划许可证和管理访问权限的用户必须在您的环境中创建自定义表单，然后才能将其添加到对象中。 有关更多信息，请参阅 [创建或编辑自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 将自定义表单添加到对象

您可以通过两种方式将自定义表单添加到对象：

* [通过编辑对象向对象添加自定义表单](#add-a-custom-form-to-an-object-by-editing-the-object)
* [将自定义表单从详细信息区域添加到对象](#add-a-custom-form-to-an-object-from-the-details-area)

### 通过编辑对象向对象添加自定义表单 {#add-a-custom-form-to-an-object-by-editing-the-object}

1. 转到要添加自定义表单的对象。
1. 单击 **更多** 菜单 ![](assets/more-icon.png)，然后单击 **编辑** ![](assets/edit-icon.png).
1. 单击 **自定义Forms** > **添加Forms**，然后从下拉菜单中选择最多10个表单。

1. （可选）更新自定义表单上可编辑字段中的信息。

   您必须更新所添加表单上的所有必填字段。

1. 单击&#x200B;**保存**。

### 将自定义表单从详细信息区域添加到对象 {#add-a-custom-form-to-an-object-from-the-details-area}

1. 转到要添加自定义表单的对象。
1. 单击 **`<Object type>`详细信息** 区域。 例如，单击 **项目详细信息** 将自定义表单添加到项目或 **问题详细信息** 向问题添加自定义表单。
1. 单击 **添加自定义表单** 字段，然后从显示的列表中选择最多10个自定义表单。

   如果表单包含任何必填字段（用红色星号标记），则此时无需填写这些字段。

   所选表单会自动附加到对象。

1. （可选）更新表单自定义字段中的信息，然后单击 **保存更改**.

## 对象上的多个自定义表单

在一个给定的对象中最多可以添加10个自定义表单，这样可以使某些字段对其他人可用，而对其他人不可用，或者允许您更好地满足多个项目的表单要求。

**示例：** 如果现有项目已经有一个自定义表单，并且需要更多自定义字段（这些字段存在于另一个自定义表单中），您可以向项目中添加另一个具有附加字段的表单，而不是将字段添加到现有自定义表单（如果仅此一个项目需要这些字段）。

## 将自定义表单批量添加到多个对象

通过在列表中选择自定义表单，可以将它们添加到多个对象中。

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
><span class="preview">有关在“预览”环境中将自定义表单批量添加到项目的信息，请参阅文章 [编辑项目](../../manage-work/projects/manage-projects/edit-projects.md)</span>.

—>

1. 导航到对象列表。
1. 在列表中选择多个对象。

1. 单击 **更多** 菜单 ![](assets/more-icon.png)，然后单击 **编辑** 图标  ![](assets/edit-icon.png)，或者只需单击 **编辑** 图标 ![](assets/edit-icon.png).
1. 单击 **自定义Forms** （在左侧面板中）。
1. 选择要与以下位置中的所有选定对象关联的表单： **进行选择** 下拉菜单。
   >[!NOTE]
   >
   >如果在下拉菜单中找不到该表单，则意味着至少一个对象已经与该表单相关联。 在将表单添加到其余对象之前，先确定是哪个对象，并将其从选定对象中排除。

1. 单击 **保存更改**.

   如果表单包含任何必填字段（用红色星号标记），则此时无需填写这些字段。
