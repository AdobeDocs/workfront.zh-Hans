---
product-area: projects
navigation-topic: manage-issues
title: 创建问题
description: 在处理项目时，您可能会发现出现意外事件。 您可以将这些意外事件记录为特定项目或任务的问题。 具有适当访问权限的用户可以在项目或任务进展到完成时查看和监控问题的状态，而无需冗长的电子邮件链或状态会议。 与属于已计划事件的任务不同，问题表示Adobe Workfront中的未计划工作项。
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '1540'
ht-degree: 0%

---

# 创建问题

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> 

<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span> 

-->

在处理项目时，您可能会发现出现意外事件。 您可以将这些意外事件记录为特定项目或任务的问题。 具有适当访问权限的用户可以在项目或任务进展到完成时查看和监控问题的状态，而无需冗长的电子邮件链或状态会议。 与属于已计划事件的任务不同，问题表示Adobe Workfront中的未计划工作项。

您还可以将问题作为请求添加到项目中。 有关信息，请参阅[创建并提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md)。

>[!TIP]
>
>在Workfront中，问题和请求可互换使用。 您可以同时记录项目和任务中的问题以指示需要解决的意外工作。 您还可以提交在指定为请求队列的项目中记录为问题的请求。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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
   <td> <p>查看或更高版本以向项目或任务添加问题</p> <p>使用请求队列请求或更高版本将问题添加为请求。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对问题的访问权限</p> <p>查看或更高权限的项目和任务</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关访问访问级别中问题的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予对问题的访问权限</a>。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>Contribute或更高权限，能够将“问题”添加到您创建问题的任务或项目</p> <p> 有关向问题授予权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题</a></p> <p>有关请求其他权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

+++

<!--
(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## 创建问题时的限制

当您拥有正确的访问权限时，您可以创建项目或任务的问题。 但是，在下列情况下，您可能无法创建问题：

* 您的Workfront管理员或组管理员必须启用添加问题，才能在项目偏好设置区域中向处于“完成”或“终止”状态的项目添加问题。 有关设置项目首选项的信息，请参阅[配置系统范围项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。
* 您无法将问题添加到未决批准中的项目。

## 准备新问题表单

您的组织应具有明确定义的流程，以便记录问题的时间和方式。 配置此流程时，第一步是创建提交问题所需的表单。 无论您允许将问题直接添加到任务和项目，还是允许将问题提交到的请求队列，您都可以定义哪些Workfront字段，以及在用户提交新问题且必须完成时可以使用哪些自定义字段。 新问题表单可包含有助于快速解决问题的重要信息。

项目新问题的字段在项目的“队列详细信息”部分中定义，将记录问题。 有关配置项目“队列详细信息”部分的信息，请参阅[创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

有关通过将问题提交到请求队列来创建问题的信息，请参阅本文中的[通过输入新请求来创建问题](#create-issues-by-entering-a-new-request)部分。

## 使用“新建问题”按钮创建任务或项目的问题

在项目中定义新问题表单的字段后，您可以开始创建问题。

<!-- OLD UI: redesigned on Oct 26, 2023:

Creating issues differs depending on which environment you choose to create the issue. 

### Create issues on a task or project using the New Issue button in the Production environment

To create an issue on a task or a project:

1. Go to a project where you want to create the issue. 
1. (Optional) If you want to log the issue for a task, go to the **Tasks** area, then click the name of a task. 
1. Click the **Issues** section.

   
1. Click **New Issue**.

  

1. (Conditional) If the project creator created Queue Topics or Topic Groups on the project they are added to the new issue form. Specify the **Topic Group** or the **Queue Topic** of your new issue. Topic Groups and Queue Topics have names customized to your environment.  
   For more information about creating Topic Groups, see [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). For more information about creating Queue Topics, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![New issue screen](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * If there is only one Queue Topic set on the project, it is displayed automatically.
   * If the Topic Group does not have any Queue Topics or Topic Groups under it, nothing is available in the Topic Group drop-down.

1. (Conditional) If the project creator allowed for the **Request Type** field to display on the New Issue form, select the type of your issue from the following options:

   * Bug Report
   * Change Order
   * Issue
   * Request  
     Depending on how your Workfront administrator has configured your Project Preferences, the names of the issue types might be different for you. 

   >[!TIP]
   >
   >The Request Types must be enabled in the Queue Details and as well as when creating the Queue Topic to display as a selection in the New Issue form. For information, see the following articles: 
   >* [Create a Request Queue](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Create Queue Topics](../../requests/create-and-manage-request-queues/create-queue-topics.md)


1. Add a name for the new issue in the **Issue Name** field. 
1. Continue specifying the fields available in the **New Issue** form. For more information about the fields available as you enter a new issue, see [Edit issues](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Not all the issue-related fields are available in the New Issue form. The project creator enables the fields available when creating an issue when they define the Queue Details area of the project. For more information, see [Create a Requests Queue](../../requests/create-and-manage-request-queues/create-request-queue.md). 


1. (Conditional) If the Queue Topics are associated with a custom form, that custom form will display in the **New Issue** form.  
   Or  
   If the project is associated with an issue custom form through the Queue Details area, the form displays in the **New Issue** form, after the default Workfront fields.

   For information, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Click **Save New Issue.**

Issues can be assigned to multiple users, job roles or to a team. For more information about assigning and managing requests, see [Manage work and team requests](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

<!--When this is coming to Production, remove the "Production" section above and replace it with the following content:
-->

要在任务或项目中创建问题，请执行以下操作：

1. 转到要创建问题的项目。
1. （可选）如果要记录任务的问题，请转到&#x200B;**任务**&#x200B;区域，然后单击任务名称。
1. 单击&#x200B;**问题**&#x200B;部分。

   此时将显示项目问题列表

1. 单击问题列表顶部的&#x200B;**新建问题**。
新问题框随即显示。

   ![新问题框](assets/new-issue-box-matches-new-request-ui.png)

1. （视情况而定）如果项目创建者在项目中创建了“队列主题”或“主题组”，则它们将被添加到新问题表单中。 指定新问题的&#x200B;**主题组**&#x200B;或&#x200B;**队列主题**。 “主题组”和“队列主题”的名称已根据您的环境定制。\
   有关创建主题组的详细信息，请参阅[创建主题组](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)。 有关创建队列主题的详细信息，请参阅[创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)。

   * 如果项目上只设置了一个队列主题，则会自动显示该主题。
   * 如果“主题组”下面没有任何“队列主题”或“主题组”，则“主题组”下拉列表中没有任何内容。

1. 在&#x200B;**主题**&#x200B;字段中添加问题名称，然后添加&#x200B;**描述**。

1. （视情况而定）如果项目创建者允许在“新问题”表单中显示&#x200B;**请求类型**&#x200B;字段，请从以下选项中选择问题类型：

   * 错误报告
   * 更改顺序
   * 问题
   * 请求\
     根据Workfront管理员配置项目首选项的方式，问题类型的名称可能有所不同。

   >[!TIP]
   >
   >必须在“队列详细信息”中以及创建队列主题时启用请求类型，以在“新建问题”表单中显示为选项。 有关信息，请参阅以下文章：
   >* [创建请求队列](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [创建队列主题](../../requests/create-and-manage-request-queues/create-queue-topics.md)

1. 继续指定&#x200B;**新问题**&#x200B;表单中可用的字段。 有关输入新问题时可用字段的更多信息，请参阅[编辑问题](../../../manage-work/issues/manage-issues/edit-issues.md)。

   >[!IMPORTANT]
   >
   >新问题表单中并非所有与问题相关的字段都可用。 项目创建者在定义项目的队列详细信息区域时，会启用创建问题时可用的字段。 有关详细信息，请参阅[创建请求队列](../../requests/create-and-manage-request-queues/create-request-queue.md)。


1. （视情况而定）如果队列主题与自定义表单关联，则该自定义表单将显示在&#x200B;**新问题**&#x200B;表单中。\
   或\
   如果项目通过“队列详细信息”区域与问题自定义表单相关联，则该表单在默认Workfront字段之后显示在&#x200B;**新建问题**&#x200B;表单中。

   有关信息，请参阅[创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

1. 单击&#x200B;**提交**。

   问题可分配给多个用户、工作角色或团队。 有关分配和管理请求的更多信息，请参阅[管理工作和团队请求](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md)。


## 在任务或项目中内联创建问题

>[!IMPORTANT]
>
>在为项目定义问题设置时，项目所有者必须启用&#x200B;**允许用户添加内联问题**，然后才能将内联问题添加到项目或任务中。 有关配置项目的问题设置的信息，请参阅[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)。
>

如果要快速添加多个问题，可以通过将任务或项目添加到问题列表，为任务或内联项目创建问题。

>[!NOTE]
>
>当您内联添加问题时，Workfront不会将新问题表单应用到新问题。 如果您希望用户在输入问题时提供某些信息，我们不建议内联添加问题。 这可能会对问题报告产生负面影响，并且稍后还会影响分配给问题的用户获得解决问题所需的所有信息的能力。

要创建内联问题，请执行以下操作：

1. 转到要创建问题的项目。
1. （可选）如果要记录任务的问题，请转到&#x200B;**任务**&#x200B;部分，然后单击任务名称。
1. 单击左侧面板中的&#x200B;**问题**&#x200B;部分。
1. 单击问题列表底部的&#x200B;**添加更多问题**。

   在“问题”部分的问题列表中创建新行。

   >[!TIP]
   >
   >如果在编辑项目框中取消选中允许用户添加问题内联设置，则此选项将灰显。 有关信息，请参阅[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)。

   ![添加更多问题按钮](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. 在名称字段中开始键入问题的名称，然后继续内联添加有关问题的更多信息。

   >[!TIP]
   >
   >您应用于问题列表的视图会提供可用于编辑内联的字段。 您可能无法内联编辑以下类型的字段：
   >   
   >* 属于其他对象的字段
   >* 您无权编辑的字段
   >* 计算字段，以及Workfront自动更新的字段

1. 单击Enter完成内联编辑，然后将问题添加到项目或任务。

## 通过输入新请求创建问题 {#create-issues-by-entering-a-new-request}

您可以将项目指定为接收问题的容器。 在Workfront中，此类项目称为请求队列。 您可以通过主菜单中的请求区域访问请求队列。

>[!TIP]
>
>术语“问题”和“请求”在Workfront中可以互换。

有关如何将项目设置为请求队列以接收问题的更多信息，请参阅[创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。 有关提交请求的信息，请参阅[创建并提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md)。
