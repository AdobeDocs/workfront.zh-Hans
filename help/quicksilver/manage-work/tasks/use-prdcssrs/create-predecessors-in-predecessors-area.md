---
product-area: projects
navigation-topic: use-predecessors
title: 使用前置任务区域创建前置任务关系
description: 您可以使用前置任务（或只是前置任务）来链接依赖其他任务启动或完成的任务。
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 使用前置任务区域创建前置任务关系

<!-- Audited: 5/2025 -->

您可以使用前置任务（或只是前置任务）来链接依赖其他任务启动或完成的任务。 例如，在发送邀请（前置任务）之前，您不希望主持某方（依赖任务）。

本文介绍如何使用任务中的“前置任务”选项卡设置前置任务。

有关在任务列表中设置前置任务的信息，请参阅[在任务列表中创建前置任务关系](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md)。

您可以在Adobe Workfront的以下区域中查看任务的前置任务：

* 在相关任务的“前置任务”部分
* 在甘特图中
* 在“前置任务”列的任务列表中

有关前置任务的信息，请参阅[前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>新增：标准 </p>
   <p>或 </p>
   <p>当前：计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务和项目的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 为任务创建前置任务

1. 导航到要指定为从属任务的任务。

1. 在左侧面板中，单击&#x200B;**前置任务**。

1. 在&#x200B;**前置任务**&#x200B;部分中，单击&#x200B;**+添加前置任务**。 将打开&#x200B;**添加前置任务**&#x200B;对话框。

1. （可选）要添加跨项目前置任务，请将&#x200B;**父项目**&#x200B;字段中的项目名称替换为其他项目。

   有关信息，请参阅[创建跨项目前置任务](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md)。

1. 在&#x200B;**任务**&#x200B;字段中，键入要指定为前置任务的一个或多个任务的名称，然后在它们出现在下拉列表时将其选定。

1. 选择&#x200B;**依赖关系类型**。

   有关信息，请参阅[任务依赖关系类型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)。

1. 输入&#x200B;**延迟**&#x200B;金额。

   有关信息，请参阅{&#x200B;0}滞后类型概述[&#128279;](../../../manage-work/tasks/use-prdcssrs/lag-types.md)。

   ![添加前置任务对话框](assets/add-predecessor-dialog-box.png)

1. 如果要强制两个任务之间的前置任务关系，请选中&#x200B;**强制**&#x200B;复选框。

   有关信息，请参阅[强制执行前置任务](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md)。

1. 单击&#x200B;**保存**。
