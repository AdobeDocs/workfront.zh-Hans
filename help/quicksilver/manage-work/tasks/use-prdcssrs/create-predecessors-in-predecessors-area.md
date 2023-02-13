---
product-area: projects
navigation-topic: use-predecessors
title: 使用“前置任务”(Precessivers)区域创建前置任务关系
description: 您可以使用前置任务（或仅前置任务）来链接依赖其他任务来开始或完成的任务。 例如，在发出邀请（前任任务）之前，您不希望托管交易方（从属任务）。
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# 使用“前置任务”(Precessivers)区域创建前置任务关系

您可以使用前置任务（或仅前置任务）来链接依赖其他任务来开始或完成的任务。 例如，在发出邀请（前任任务）之前，您不希望托管交易方（从属任务）。

本文将介绍如何使用任务中的“前置任务”选项卡来设置前置任务。

有关在任务列表中设置前置任务的信息，请参阅 [在任务列表上创建前置任务关系](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

您可以在Adobe Workfront的以下区域查看以前的任务：

* 在从属任务的“前置任务”部分中
* 在甘特图中
* 在“前置任务”列的任务列表中

有关前置任务的信息，请参阅 [任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>编辑对任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务和项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 为任务创建前置任务

1. 转到要指定为从属任务的任务，然后单击 **前置任务** 中。

   您可能需要单击 **显示更多**，则 **前置任务**.

1. 单击 **+添加前驱**.
1. （可选）要添加跨项目前置项，请在 **父项目** 字段，然后键入作为前置任务的任务名称。

   有关添加跨项目前置项的信息，请参阅 [创建跨项目前置项](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. 键入要指定为前置任务的任务名称。

   ![](assets/add-predecessor-box-nwe-350x465.png)

1. 选择 **依赖关系类型**.

   有关任务依赖关系类型的信息，请参阅 [任务依赖关系类型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. 指定 **滞后** 金额（以天为单位）。

   有关滞后类型的信息，请参&#x200B;阅 [滞后类型概述](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

1. 选择 **强制** 如果要执行两个任务之间的前置任务关系。

   有关强制前置任务的信息，请参阅 [强制前置任务](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. 单击&#x200B;**保存**。
