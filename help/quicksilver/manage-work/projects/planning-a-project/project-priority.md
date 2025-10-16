---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 了解和更新项目优先级
description: 有几种方法可以将优先级用于项目，并且它们不会相互通信。 我们建议您为符合自己需求的项目选择其中一个优先级，并在对项目的重要性进行分类时参考该优先级。
author: Alina
feature: Work Management
exl-id: b1e0b6c5-f2a7-455b-836b-6c0ead85e3ad
source-git-commit: 00e693fc8b35a59f6ed212bc30da7f85cc78c845
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 1%

---

# 了解并更新项目优先级

有几种方法可以将优先级用于项目，并且它们不会相互通信。 我们建议您为符合自己需求的项目选择其中一个优先级，并在对项目的重要性进行分类时参考该优先级。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p> 
   <p>规划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Adobe Workfront中的项目优先级类型

以下是可用于在Adobe Workfront中对项目进行排名的优先级类型：

* **项目优先级字段**：您可以手动为项目分配优先级。 本文介绍了如何手动为项目分配优先级。

  有关详细信息，请参阅本文中的[有关项目优先级的注意事项](#considerations-about-project-priority)部分。

* **Portfolio优化程序中的项目优先级**（如果项目与项目组合关联）：

  有关Portfolio Optimizer中项目优先级的更多信息，请参阅文章[在Portfolio Optimizer中排定项目优先级](../../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md)。

* **资源规划者中项目的优先级**：您可以手动设置资源规划者中项目的优先级，以指示哪些项目应首先接收资源。

  有关在资源规划程序中排列项目优先顺序的更多信息，请参阅文章[资源规划程序导航概述](../../../resource-mgmt/resource-planning/resource-planner-navigation.md)中的“项目规划优先级”部分。

## 有关项目优先级的注意事项 {#considerations-about-project-priority}

您可以将优先级与Workfront中的项目关联。 指明项目的优先级会告知系统中的每个人，该项目有多重要。

为您的项目选择优先级时，请考虑以下事项：

* 您的Workfront管理员定义Workfront中可用的优先级。 创建项目后，即可将它们与优先级字段中的项目相关联。

  有关在Workfront中创建优先级的详细信息，请参阅文章[创建和自定义优先级](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md)。

* 当您更新项目的“优先级”字段时，此优先级未转移到Portfolio优化程序或资源规划者。 项目的“优先级”字段只是一个手动标记，您可以将该标记放置到项目上，以向其他用户指示其重要性。
* 项目的优先级值主要用于报告目的。

  例如，在项目筛选器中使用此字段时，您可以搜索优先级值为紧急的所有项目。
* 任务和问题还具有优先级，但任务、问题和项目优先级相互独立工作，不会自动影响彼此的优先级。 您可以在低优先级项目中有一个高优先级问题或一个中优先级任务。
* 您可以在Workfront的以下区域中更新项目的优先级：

   * 在&#x200B;**编辑项目**&#x200B;对话框中。
   * 在项目的&#x200B;**项目详细信息**&#x200B;选项卡中。
   * 在项目列表或报表中。

## 更新项目优先级字段

1. 转到要更新其优先级的项目。
1. 单击左侧面板中的&#x200B;**项目详细信息**。
1. 单击项目详细信息区域右上角的&#x200B;**编辑**&#x200B;图标![编辑图标](assets/qs-edit-icon.png)，然后单击&#x200B;**概述**。

1. 在&#x200B;**优先级**&#x200B;字段中，从以下选项中选择：

   * 无
   * 低
   * 正常

     这是默认优先级。

   * 高
   * 紧急

   ![项目的优先级列表](assets/project-priority-picker-list.png)

1. 单击&#x200B;**保存更改**。

   您必须与其他用户沟通，并了解每个优先级别对项目意味着什么。
