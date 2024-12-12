---
product-area: projects
navigation-topic: financials
title: 管理项目支出
description: 对于项目费用和任务相关费用，创建和管理费用的过程是相同的。 在业务案例中添加到项目的任何费用将作为计划费用添加到“费用”选项卡中。 有关业务案例的更多信息，请参阅为项目创建业务案例一文。
author: Lisa
feature: Work Management
exl-id: 80c41b08-3618-4d6e-8d07-1736b2f824ea
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# 管理项目支出

对于项目费用和任务相关费用，创建和管理费用的过程是相同的。 在业务案例中添加到项目的任何费用将作为计划费用添加到“费用”选项卡中。 有关业务案例的详细信息，请参阅文章[为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

所有任务和项目中的总费用占项目的总成本。 费用的计划金额对项目的计划成本有贡献，费用的实际金额对项目的实际成本有贡献。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>
   <p>新增：标准</p>
   <p>或</p>
   <p>当前：工作或更高</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td>编辑对项目和财务数据的访问权限</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>具有Contribute或更高项目权限以及查看或管理财务的权限</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 添加费用

1. 转到要输入费用的项目。\
   如果要将费用添加到任务，请导航到任务。 
1. 单击&#x200B;**显示更多**，然后单击&#x200B;**费用**。
1. 单击&#x200B;**添加费用** 。
显示**添加费用**&#x200B;对话框。
1. 更新以下内容：

   * **描述：**&#x200B;费用的描述。

   * **费用类型：**（必需）选择最能描述该费用的类别。
   * **任务：**&#x200B;开始键入与此费用关联的任务的名称，然后在任务出现在下拉列表中时单击该名称。
   * **计划金额：**&#x200B;支出的计划预算金额。\
     这会影响项目的预算成本。

   * **实际金额：**&#x200B;费用实际成本的金额。\
     这会影响项目的实际成本。

   * **计划日期：**&#x200B;预计费用发生的日期。 您可以使用&#x200B;*mm/dd/yy*&#x200B;格式在字段中键入日期，也可以单击日历图标  ![](assets/calendar-icon.png)并动态选择日期。

   * **支付日期：**&#x200B;支付费用的日期。
   * **可记帐：**&#x200B;如果要对此费用记帐，请选择此选项。 创建开票记录时，将费用归类为可开票很重要。
   * **可偿还：**&#x200B;如果需要偿还费用，请选择此选项。 然后，您可以在偿还费用后将费用标记为已偿还。

1. 选择&#x200B;**自定义表单**&#x200B;并指定所需的任何其他信息。 您必须先创建自定义表单，然后才能将其与费用关联。 列表中仅显示活动的自定义表单。 有关创建自定义表单的信息，请参阅文章[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

1. 单击&#x200B;**保存更改**。

## 删除费用

1. 转到要删除费用的项目。
1. 单击&#x200B;**显示更多**，然后单击&#x200B;**费用**。
1. 选择要删除的费用，然后单击&#x200B;**删除** ![删除](assets/delete.png)。

1. 单击&#x200B;**是，将其删除**&#x200B;以确认删除。
