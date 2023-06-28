---
product-area: projects
navigation-topic: manage-issues
title: 创建问题
description: 在处理项目时，您可能会发现发生了意外事件。 您可以将这些意外事件记录为特定项目或任务的问题。 具有适当访问权限的用户可以在项目或任务进展到完成时查看和监控问题的状态，而无需冗长的电子邮件链或状态会议。 与任务（属于计划事件）不同，问题表示Adobe Workfront中的计划外工作项。
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: 716b5a151585aa314cd9db67237d2ed085e817c1
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 0%

---

# 创建问题

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

在处理项目时，您可能会发现发生了意外事件。 您可以将这些意外事件记录为特定项目或任务的问题。 具有适当访问权限的用户可以在项目或任务进展到完成时查看和监控问题的状态，而无需冗长的电子邮件链或状态会议。 与任务（属于计划事件）不同，问题表示Adobe Workfront中的计划外工作项。

您还可以将问题作为请求添加到项目中。 有关信息，请参阅 [创建和提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>在Workfront中，问题和请求可互换使用。 您可以记录项目和任务中的问题，以指示需要解决的意外工作。 您还可以提交在指定为请求队列的项目中记录为问题的请求。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

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
   <td> <p>查看或更高版本以向项目或任务添加问题</p> <p>使用请求队列请求或更高版本将问题添加为请求。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑问题的访问权限</p> <p>查看或更高权限的项目和任务</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关访问访问级别中问题的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予对问题的访问权限</a>. 有关Workfront管理员如何更改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>Contribute或更高权限，能够向任务或创建问题的项目添加问题</p> <p> 有关向问题授予权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题 </a></p> <p>有关请求其他权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

<!--
(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## 创建问题时的限制

如果您拥有正确的访问权限，则可以在项目或任务上创建问题。 但是，在下列情况下，您可能无法创建问题：

* 您的Workfront管理员或组管理员必须启用向项目偏好设置区域中处于“完成”或“终止”状态的项目添加问题。 有关设置项目首选项的信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* 您无法将问题添加到未决批准中的项目。

## 准备新问题表单

您的组织应已制定明确定义的流程，以便记录问题的时间和方式。 配置此流程时，第一步是创建提交问题所需的表单。 无论您是允许将问题直接添加到任务和项目，还是有已提交问题的请求队列，您都可以定义哪些Workfront字段，以及在用户提交新问题且必须完成时可以使用哪些自定义字段。 “新建问题”表单可包含重要信息，这些信息将有助于快速解决问题。

项目新问题的字段在项目的“队列详细信息”部分中定义，将记录问题。 有关配置项目的队列详细信息部分的信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

有关通过将问题提交到请求队列来创建问题的信息，请参阅 [通过输入新请求创建问题](#create-issues-by-entering-a-new-request) 章节。

## 使用“新建问题”按钮在任务或项目上创建问题

在项目中定义新问题表单的字段后，您可以开始创建问题。

要在任务或项目上创建问题，请执行以下操作：

1. 转到要创建问题的项目。
1. （可选）如果要记录任务的问题，请转到 **任务** 区域，然后单击任务的名称。
1. 单击 **问题** 部分。

   ![](assets/qs-issues-icon-highlighted-on-project-350x216.png)

1. 单击 **新建问题**.

   ![](assets/qs-issue-list-on-project-with-new-issue-button-highlighted-350x270.png)

1. （视情况而定）如果项目创建者在项目上创建了“队列主题”或“主题组”，则它们将被添加到新问题表单中。 指定 **主题组** 或 **队列主题** 您的新问题。 他们应具有根据您的环境自定义的名称。\
   有关创建主题组的详细信息，请参见 [创建主题组](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). 有关创建队列主题的详细信息，请参见 [创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   <!--update the screen shot above for preview and highlight in yellow-->

   * 如果项目上只设置了一个队列主题，则会自动显示该主题。
   * 如果主题组下没有队列主题或主题组，则主题组下拉列表中将没有任何内容。

1. （视情况而定）如果项目创建者允许 **问题类型** 要显示在新问题表单上的字段，请从以下选项中选择问题类型：

   * 错误报告
   * 更改顺序
   * 问题
   * 请求\
     根据Workfront管理员配置项目首选项的方式，问题类型的名称可能有所不同。

1. 指定中可用的任何字段 **新建问题** 表单。 有关在输入新问题时定义字段的更多信息，请参阅 [编辑问题](../../../manage-work/issues/manage-issues/edit-issues.md).
1. （视情况而定）如果队列主题与自定义表单关联，则该自定义表单将显示在 **新建问题** 表单。\
   或\
   如果项目通过队列详细信息区域与问题自定义表单相关联，则该表单会显示在 **新建问题** 表单，位于默认Workfront字段下。

   有关信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 单击 **保存新问题。**

问题可分配给多个用户、工作角色或团队。 有关分配和管理请求的更多信息，请参阅 [管理工作和团队请求](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## 为任务或项目创建内联问题

>[!IMPORTANT]
>
>项目所有者必须启用 **允许用户添加内联问题** 在为项目定义问题设置时，您可以先将内联问题添加到项目或任务。 有关在项目上配置问题设置的信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).
>

如果要快速添加多个问题，可以通过将问题添加到问题列表，为任务或内联项目创建问题。

>[!NOTE]
>
>当您内联添加问题时，Workfront不会将“新问题”表单应用于新问题。 如果您希望用户在输入问题时提供某些信息，我们不建议添加内联问题。 这可能会对问题报告产生负面影响，并且稍后还会对分配给问题的用户获得解决问题所需的所有信息的能力产生负面影响。

要创建内联问题，请执行以下操作：

1. 转到要创建问题的项目。
1. （可选）如果要记录任务的问题，请转到 **任务** 部分，然后单击任务的名称。
1. 单击 **问题** 部分。
1. 单击 **添加更多问题**.

   在问题部分的问题列表中创建新行。

   >[!TIP]
   >
   >如果在“编辑项目”框中取消选中“允许用户添加问题内联”设置，则此选项将灰显。 有关信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. 开始在名称字段中键入问题的名称，然后继续内联添加有关问题的更多信息。

   >[!TIP]
   >
   >可用于编辑内联的字段由您应用于问题列表的视图提供。 您可能无法内联编辑以下类型的字段：
   >   
   >* 属于其他对象的字段
   >* 您无权编辑的字段
   >* 计算字段，以及Workfront自动更新的字段

1. 单击Enter以完成内联编辑，然后将问题添加到项目或任务。

## 通过输入新请求创建问题 {#create-issues-by-entering-a-new-request}

您可以将项目指定为接收问题的容器。 此类项目在Workfront中称为“请求队列”。 您可以通过主菜单中的请求区域访问请求队列。

>[!TIP]
>
>术语“问题”和“请求”在Workfront中可以互换。

有关如何将项目设置为请求队列以接收问题的更多信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). 有关提交请求的信息，请参见 [创建和提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md).
