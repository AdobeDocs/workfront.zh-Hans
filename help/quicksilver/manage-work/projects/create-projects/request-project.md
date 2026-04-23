---
product-area: projects
navigation-topic: create-projects
title: Request a project
description: 您可以在开始处理项目之前请求批准该项目。 我们建议为新项目构建业务案例，以便您概述希望通过完成项目而实现的一些要点，并向您的管理团队展示您的人工和费用预算。 填写业务案例并提交项目审批完成项目的正式请求。 提交业务案例以供审批后，项目的状态变为“已请求”。
author: Alina
feature: Work Management
exl-id: 6557a7a5-3d5e-476d-b834-007c9e120397
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 5%

---

# 请求项目

<!--Audited: 10/2025-->

You can request for a project to be approved before you start working on it.

When you create a blank project, the status of the project is Idea.

If you need a formal request for the project to be approved, we recommend building a Business Case for a new project so that you can outline some of the key points you want to achieve by completing it, as well as to present to your management your labor and expense budget.

Filling out the Business Case and submitting the project for approval completes the formal request for the project. After submitting the business case for approval the status of the project becomes Requested.

You can request a project when you add a new project in the following areas of Adobe Workfront:

* In the Projects area
* In the Projects area of a Portfolio
* 在项目群的项目区域中
* 在项目组的组区域中，当您是组管理员时。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront许可证</p> </td> 
   <td> <p>标准</p>
   <p>规划</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>Edit access to Projects</p>
   <p>如果您从项目组合或项目群请求项目，则必须拥有对项目组合和项目群的“编辑”访问权限</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>在创建项目请求时，您会自动接收项目的管理权限 </p> 
   <p>如果您从项目组合或项目群请求项目，您必须具有项目组合和项目群的管理权限。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront license*</p> </td> 
   <td> <p>New: Standard </p>
   Or
   <p>Current: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project request you automatically receive Manage permissions to the project </p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Request a project

1. 执行下列操作之一：

   * Click the **Main Menu** icon![Main Menu lines](assets/lines-main-menu.png) in the upper-left corner, click **Projects**, then expand **New Project**.
   * Go to a portfolio, then expand **New Project**.
   * Go to a program, then expand **New Project**.
   * If you are a group administrator, you can also create a project in the Projects section of a group you manage. For more information, see [Create and modify a group&#39;s projects](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. 单击&#x200B;**请求项目**。

   ![新项目下拉列表](assets/new-project-dropdown-nwe-350x358.png)

1. 执行下列操作之一：

   * Follow the same steps as for creating a project while defining a Business Case. （推荐）

     For information, see [Create a Business Case for a project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

   * Create a project from scratch or using a template and change the status to **Requested**.

     For information, see [Create a project](../../../manage-work/projects/create-projects/create-project.md) or [Create a project using a template](../../../manage-work/projects/create-projects/create-project-from-template.md).

   The project you request has a status of **Requested** and it displays on the **Requested Projects** tab of a Portfolio, if you associated it with a Portfolio.

   A portfolio manager can now review it and either approve it or reject it, in which case the status of the project changes to either **Approved** or **Rejected**.
