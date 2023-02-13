---
product-area: projects
navigation-topic: financials
title: 管理项目费用
description: 项目和任务相关费用的创建和管理费用的过程是相同的。 在“业务案例”中添加到项目的任何费用都将作为计划费用添加到“费用”标签中。 有关业务案例的更多信息，请参阅为项目创建业务案例一文。
author: Alina
feature: Work Management
exl-id: 80c41b08-3618-4d6e-8d07-1736b2f824ea
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 1%

---

# 管理项目费用

项目和任务相关费用的创建和管理费用的过程是相同的。 在“业务案例”中添加到项目的任何费用都将作为计划费用添加到“费用”标签中。 有关“业务案例”的详细信息，请参阅 [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

所有任务和项目的费用总额将计入项目的总成本。 费用的计划金额会计入项目的计划成本，而费用的实际金额会计入项目的实际成本。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目和财务数据的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限，并具有管理财务的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 添加费用

1. 转到要输入费用的项目。\
   如果要向任务添加费用，请改为定位到任务。 
1. 单击 **显示****更多**，然后单击 **费用。**
1. 单击 **添加费用。**
此 
**添加费用** 对话框。
1. 更新以下内容：

   * **描述：** 费用的描述。

   * **费用类型：** （必需）选择最能描述费用的类别。
   * **任务：** 开始键入此费用关联的任务名称，然后在下拉列表中显示时单击该名称。
   * **计划金额：** 费用的计划预算金额。\
      这会影响项目的预算成本。

   * **实际金额：** 费用实际成本的金额。\
      这会影响项目的实际成本。

   * **计划日期：** 开支的预期发生日期。 您可以使用 *mm/dd/yy* 格式，或者单击日历图标  ![](assets/calendar-icon.png) 并动态选择日期。

   * **付款日期：** 支付费用的日期。
   * **计费：** 如果要开单此费用，请选择此选项。 在创建计费记录时，将费用分类为可计费项很重要。
   * **可报销：** 如果需要报销费用，请选择此选项。 然后，在报销费用后，您可以将费用标记为已报销。

1. 选择 **自定义表单** 并指定所需的任何其他信息。 必须先创建自定义表单，然后才能将其与费用关联。 列表中仅显示活动的自定义表单。 有关创建自定义表单的信息，请参阅文章 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 单击 **保存更改。**

## 删除费用

1. 转到要删除费用的项目。
1. 单击&#x200B;**显示****更多**，然后单击 **费用。**
1. 选择要删除的费用，然后单击 **删除** ![删除](assets/delete.png).

1. 单击 **是，删除它** 以确认删除。 
