---
product-area: projects
navigation-topic: use-predecessors
title: 使用前置任务区域创建前置任务关系
description: 您可以使用前置任务（或只是前置任务）来链接依赖其他任务启动或完成的任务。 例如，在发出邀请（前置任务）之前，您不希望主持某方（依赖任务）。
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: d5f4e83badd4d011816551f06b056ffe886d3b17
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# 使用前置任务区域创建前置任务关系

您可以使用前置任务（或只是前置任务）来链接依赖其他任务启动或完成的任务。 例如，在发出邀请（前置任务）之前，您不希望主持某方（依赖任务）。

本文介绍如何使用任务中的“前置任务”选项卡设置前置任务。

有关在任务列表中设置前置任务的信息，请参阅 [在任务列表上创建前置任务关系](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

您可以在Adobe Workfront的以下区域中查看任务的前置任务：

* 在相关任务的“前置任务”部分
* 在甘特图中
* 在“前置任务”列的任务列表中

有关前置任务的信息，请参阅 [前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务和项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 为任务创建前置任务

1. 转至要指定为从属任务的任务，然后单击 **前置任务** 在左侧面板中。

   您可能需要单击 **显示更多**，则 **前置任务**.

1. 单击 **+添加前置任务**.
1. （可选）要添加跨项目前置任务，请在左侧导航中替换项目的名称， **父项目** 字段中，然后键入要作为前置任务的一个或多个任务的名称。

   有关添加跨项目前置任务的信息，请参阅 [创建跨项目前置任务](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. 键入要指定为前置任务的一个或多个任务的名称。

   ![](assets/add-predecessor-box-nwe-350x465.png)

1. 选择 **依赖关系类型**.

   有关任务相关性类型的信息，请参阅 [任务相关性类型概览](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. 指定 **滞后时间** 以天为单位的金额。

   有关Lag类型的信息，请参阅&#x200B; [滞后类型概述](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

1. 选择 **强制** 如果要强制两个任务之间的前置任务关系，请执行以下操作。

   有关实施前置任务的信息，请参阅 [强制前置任务](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. 单击&#x200B;**保存**。
