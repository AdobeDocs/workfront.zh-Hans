---
product-area: projects
navigation-topic: manage-issues
title: 创建问题
description: 在处理项目时，您可能会发现出现意外事件。 您可以将这些意外事件记录为特定项目或任务的问题。 具有相应访问权限的用户可以在项目或任务完成过程中查看和监控问题的状态，从而无需冗长的电子邮件链或状态会议。 与计划事件任务不同，问题代表Adobe Workfront中的计划外工作项。
author: Alina
feature: Work Management
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 0%

---

# 创建问题

在处理项目时，您可能会发现出现意外事件。 您可以将这些意外事件记录为特定项目或任务的问题。 具有相应访问权限的用户可以在项目或任务完成过程中查看和监控问题的状态，从而无需冗长的电子邮件链或状态会议。 与计划事件任务不同，问题代表Adobe Workfront中的计划外工作项。

您还可以将问题作为请求添加到项目中。 有关信息，请参阅 [创建和提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>问题和请求在Workfront中可互换使用。 您可以记录项目和任务中的问题，以指明需要解决的未预见工作。 您还可以提交被记录为指定为请求队列的项目问题的请求。

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
   <td> <p>查看或更高版本以向项目或任务添加问题</p> <p>使用请求队列，请求或更高版本将问题添加为请求。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对问题的访问权限</p> <p>查看或更高权限访问项目和任务</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关访问访问级别中问题的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予对问题的访问权限</a>. 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>具有向创建问题的任务或项目添加问题的权限的参与者或更高权限</p> <p> 有关授予问题权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题 </a></p> <p>有关请求其他权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## 创建问题时的限制

当您拥有正确的访问权限和权限时，您可以在项目或任务中创建问题。 但是，在以下情况下，您可能无法创建问题：

* 您的Workfront管理员或组管理员必须允许向项目首选项区域中处于完全或无效状态的项目添加问题。 有关设置项目首选项的信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* 您无法向处于“待批准”状态的项目添加问题。

## 准备新问题表单

贵组织应制定一个明确的流程，用于记录问题的时间和方式。 配置此过程时，第一步是创建提交问题所需的表单。 无论您是允许将问题直接添加到任务和项目中，还是如果您有提交问题的请求队列，您都可以定义哪些Workfront字段以及用户在提交新问题时可以使用的自定义字段，并且这些字段必须填写。 “新问题”窗体可以包含有助于快速解决问题的重要信息。

项目中新问题的字段在将记录问题的项目的“队列详细信息”部分中定义。 有关配置项目的“队列详细信息”部分的信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

有关通过将问题提交到请求队列来创建问题的信息，请参阅 [通过输入新请求创建问题](#create-issues-by-entering-a-new-request) 章节。

## 使用“新建问题”按钮创建任务或项目的问题

在项目中定义了新问题表单的字段后，即可开始创建问题。

要在任务或项目上创建问题，请执行以下操作：

1. 转到要创建问题的项目。
1. （可选）如果要记录任务的问题，请转到 **任务** ，然后单击任务的名称。
1. 单击 **问题** 中。

   ![](assets/qs-issues-icon-highlighted-on-project-350x216.png)

1. 单击 **新问题**.

   ![](assets/qs-issue-list-on-project-with-new-issue-button-highlighted-350x270.png)

1. （视情况而定）如果项目创建者在项目中创建了队列主题或主题组，则这些主题或主题组会添加到新的问题表单中。 指定 **主题组** 或 **队列主题** 新期刊中的。 这些用户名应根据您的环境进行自定义。\
   有关创建主题组的更多信息，请参阅 [创建主题组](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). 有关创建队列主题的更多信息，请参阅 [创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * 如果项目上只设置了一个队列主题，则会自动显示该主题。
   * 如果主题组下没有任何队列主题或主题组，则“主题组”下拉列表中将不提供任何内容。

1. （视情况而定）如果项目创建者允许 **问题类型** “New Issue（新建问题）”窗体中显示的字段，请从以下选项中选择问题类型：

   * 错误报告
   * 更改顺序
   * 问题
   * 请求\
      根据Workfront管理员配置项目首选项的方式，问题类型的名称可能会因您而异。

1. 指定 **新问题** 表单。 有关在输入新问题时定义字段的详细信息，请参阅 [编辑问题](../../../manage-work/issues/manage-issues/edit-issues.md).
1. （视情况而定）如果队列主题与自定义表单关联，则该自定义表单将显示在 **新问题** 表单。\
   或\
   如果项目通过“队列详细信息”区域与问题自定义表单关联，则该表单会显示在 **新问题** 表单中，选择“默认Workfront”字段。

   有关信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 单击 **保存新问题。**

问题可以分配给多个用户、作业角色或团队。 有关分配和管理请求的更多信息，请参阅 [管理工作和团队请求](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## 在内联任务或项目上创建问题

>[!IMPORTANT]
>
>项目所有者必须启用 **允许用户在内联中添加问题** 在为项目定义问题设置时，您可以先在项目或任务中添加内联问题。 有关在项目中配置问题设置的信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

如果要快速添加多个问题，可以通过将任务或项目添加到问题列表，为内联任务或项目创建问题。

>[!NOTE]
>
>在内联添加问题时，Workfront不会将“新问题”表单应用于新问题。 如果您希望用户在输入问题时提供特定信息，我们不建议在内联添加问题。 这可能会对问题报告以及以后分配给问题的用户是否能够拥有解决问题所需的所有信息产生负面影响。

要在内联创建问题，请执行以下操作：

1. 转到要创建问题的项目。
1. （可选）如果要记录任务的问题，请转到 **任务** ，然后单击任务的名称。
1. 单击 **问题** 中。
1. 单击 **添加更多问题**.

   将在“问题”部分的问题列表中创建一个新行。

   >[!TIP]
   >
   >如果在“编辑项目”框中取消选择“允许用户添加问题”内联设置，则此选项将灰显。 有关信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. 开始在“名称”字段中键入问题的名称，然后继续在内联中添加有关该问题的更多信息。

   >[!TIP]
   >
   >可用于编辑内联的字段由您应用到问题列表的视图提供。 您可能无法在内联编辑以下类型的字段：
   >   
   >* 属于其他对象的字段
   >* 您无权编辑的字段
   >* 属于计算且由Workfront自动更新的字段


1. 单击Enter以完成内联编辑，并将问题添加到项目或任务中。

## 通过输入新请求创建问题 {#create-issues-by-entering-a-new-request}

您可以指定项目作为接收问题的接收器。 在Workfront中，这些类型的项目称为请求队列。 您可以通过主菜单的请求区域访问请求队列。

>[!TIP]
>
>术语“issue”和“request”在Workfront中可互换。

有关如何将项目设置为请求队列以接收问题的更多信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). 有关提交请求的信息，请参阅 [创建和提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md).
