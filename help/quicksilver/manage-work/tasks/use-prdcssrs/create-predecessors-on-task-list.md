---
product-area: projects
navigation-topic: use-predecessors
title: 在任务列表上创建前置任务关系
description: 您可以使用前置任务（或仅前置任务）来链接依赖其他任务来开始或完成的任务。 例如，在发出邀请（前任任务）之前，您不希望托管交易方（从属任务）。
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 420ba180dd0bfd53514c58f77ca9897ba9797320
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# 在任务列表上创建前置任务关系

您可以使用前置任务（或仅前置任务）来链接依赖其他任务来开始或完成的任务。 例如，在发出邀请（前任任务）之前，您不希望托管交易方（从属任务）。

本文将向您展示如何在任务列表中创建前置任务。

您可以在Adobe Workfront的以下区域查看以前的任务：

* 在“前置任务”列的任务列表中。
* 在甘特图中
* 在从属任务的“前置任务”部分

有关更多信息，请参阅 [任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>编辑对任务和项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务和项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建前置任务

1. 转到项目。
1. 单击 **任务** 中。
1. 确保当前视图显示 **前置** 列。

   如果视图未显示“前置项”列，请更改为显示该视图的视图，或将该列添加到您的视图。

1. 选择要指定为从属任务的任务。
1. 在 **前置任务** 列。
1. 键入要指定为所选任务的前置任务的任务编号，然后按 **输入**.

   当前任务标记为完成时，前置任务图标将变为绿色。 这表示相关任务已准备就绪。

   有关“前置项”列中可用的关系类型的详细信息，请参阅 [任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) in [任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 查看前置任务详细信息

您可以从任务列表中快速查看有关前置任务的详细信息。

1. 在任务列表中，将鼠标悬停在 **前置任务** 列。

   此时将显示一个包含前置任务详细信息的框。

   ![前置任务详细信息](assets/predecessor-details-in-task-list.png)

   将显示以下详细信息：

   **前置名称：** 引用的前置代理的名称。 包括前置任务的任务编号。 单击任务名称以将其打开。 在上例中，前身是生产/执行/交付。

   **项目名称：** 前置项所在项目的名称。 如果前置项目属于与任务相同的项目，则该项目将被标识为当前项目；如果前置项目属于其他项目，则该项目将被标识为跨项目。 在上例中，项目名称为数字资产生产（集成） — 项目。 有关跨项目前置项的更多信息，请参阅 [创建跨项目前置项](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   您可以展开项目详细信息，以查看项目的计划开始和结束日期、条件、状态、完成百分比和所有者。 对于跨项目，您可以单击 **请参阅项目** 以打开项目。

   **ID:** 前置任务所在项目的参考编号。

   **计划开始时间：** 上一任务的计划起始日期。

   **计划结束：** 前置任务的计划完成日期。

   **前置任务数：** 引用的前置文件的前置文件数。 在上例中，被引用的前身有1个前身。

   **后继者数量：** 被引用的前任的后继任务（或从属任务）数。 在上例中，被引用的前身具有1个后继者。
