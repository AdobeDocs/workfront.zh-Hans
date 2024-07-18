---
product-area: projects;user-management
keywords: 附加，应用
navigation-topic: work-with-custom-forms
title: 向对象添加自定义表单
description: 您可以将现有的自定义表单添加到下面列出的任何对象中。 自定义表单包含自定义字段，您可以在其中存储有关对象的信息。
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 1%

---

# 向对象添加自定义表单

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

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
* 账单记录

您只能将自定义表单添加到为其创建表单的对象类型。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中所述的操作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
<tr> 
  <td role="rowheader">Adobe Workfront许可证</td> 
  <td> <p>新文档：参与者或更高版本 </p>
 <p>或</p> 
<p>当前：请求或更高版本 </p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑您对其管理自定义表单的对象的访问权限</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理要为其附加自定义表单的对象的权限。</p> <p>查看自定义表单或更高权限，具有附加到自定义数据</b>对象（项目、任务和问题）的<b>权限。 有关详细信息，请参阅<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">共享自定义表单</a>。</p> <p>重要信息：如果您没有对自定义Forms具有管理访问权限的计划许可证，则您必须具有至少查看自定义表单的特定权限，如<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">共享自定义表单</a>中所述。 即使表单在系统范围内可见，也必须向您授予这些权限。 </p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

您的Workfront管理员或具有自定义表单的计划许可证和管理访问权限的用户必须在您的环境中创建自定义表单，然后才能将它们添加到对象中。 有关详细信息，请参阅[使用表单设计器设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 向对象添加自定义表单

您可以通过两种方式将自定义表单添加到对象：

* [通过编辑对象向对象添加自定义表单](#add-a-custom-form-to-an-object-by-editing-the-object)
* [从详细信息区域将自定义表单添加到对象](#add-a-custom-form-to-an-object-from-the-details-area)

### 通过编辑对象向对象添加自定义表单 {#add-a-custom-form-to-an-object-by-editing-the-object}

1. 转到要添加自定义表单的对象。
1. 单击&#x200B;**更多**&#x200B;菜单![](assets/more-icon.png)，然后单击&#x200B;**编辑** ![](assets/edit-icon.png)。
1. 单击&#x200B;**自定义Forms** > **添加Forms**，然后从下拉菜单中选择最多10个表单。

1. （可选）更新自定义表单上可编辑字段中的信息。

   您必须更新所添加表单上的所有必填字段。

1. 单击&#x200B;**保存**。

### 从详细信息区域将自定义表单添加到对象 {#add-a-custom-form-to-an-object-from-the-details-area}

1. 转到要添加自定义表单的对象。
1. 单击左侧面板中的&#x200B;**`<Object type>`详细信息**&#x200B;部分。 例如，单击&#x200B;**项目详细信息**&#x200B;以将自定义表单添加到项目，或单击&#x200B;**问题详细信息**&#x200B;以将自定义表单添加到问题。
1. 单击右上角的&#x200B;**添加自定义表单**&#x200B;字段，然后从显示的列表中选择最多10个自定义表单。

   如果表单包含任何必填字段（用红色星号标记），则此时无需填写这些字段。

   所选表单会自动附加到对象。

1. （可选）更新表单自定义字段中的信息，然后单击&#x200B;**保存更改**。

## 对象中的多个自定义表单

您最多可以在给定对象上添加10个自定义表单，从而使字段对某些用户可用，而对其他用户不可用，或使您更好地满足多个项目的表单要求。

**示例：**&#x200B;如果某个现有项目已经有一个自定义表单，而另一个自定义表单上存在此项目需要更多自定义字段，则可以向该项目添加第二个具有附加字段的表单，而不是向现有自定义表单添加字段。

## 将自定义表单批量添加到多个对象

通过在列表中选择自定义表单，您可以将自定义表单添加到多个对象。

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>对于项目以外的所有对象，将自定义表单添加到对象的操作都是相同的。
>
>有关将自定义表单批量添加到项目的信息，请参阅文章[编辑项目](../../manage-work/projects/manage-projects/edit-projects.md)。


1. 导航到对象列表。
1. 在列表中选择多个对象。

1. 单击&#x200B;**更多**&#x200B;菜单![](assets/more-icon.png)，然后单击&#x200B;**编辑**&#x200B;图标![](assets/edit-icon.png)。

   或

   单击列表顶部的&#x200B;**编辑**&#x200B;图标![](assets/edit-icon.png)。
1. 单击左侧面板中的&#x200B;**自定义Forms**。
1. 在&#x200B;**进行选择**&#x200B;下拉菜单中，选择要与所有选定对象关联的表单。

   >[!NOTE]
   >
   >如果在下拉菜单中找不到该表单，则意味着至少一个对象已经与该表单相关联。 在将表单添加到其余对象之前，先确定是哪个对象，并将其从选定对象中排除。


1. 单击&#x200B;**保存更改**。

   如果表单包含任何必填字段（用红色星号标记），则此时无需填写这些字段。
