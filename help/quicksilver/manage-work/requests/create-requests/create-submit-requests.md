---
product-area: requests
navigation-topic: create-requests
title: 创建和提交Adobe Workfront请求
description: 计划工作由项目和任务代表Adobe Workfront。 但是，您可能会在以下环境中工作：计划外工作（以随机请求的形式）可以随时进入。 Workfront提供了一个工作流，可通过使用请求队列来适应此类环境。
author: Alina
feature: Work Management
exl-id: 8b023a3d-326d-4d63-9e1e-8171553a9e23
source-git-commit: b40ade1f1d7a9b81c654a274c5e8c872bf74b180
workflow-type: tm+mt
source-wordcount: '2337'
ht-degree: 2%

---

# 创建和提交Adobe Workfront请求

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Linked to the UI - do not change/ remove; THIS IS NOW SPLIT IN THREE ARTICLES>> MAKE SURE THE TRANSITION TO THE OTHER TWO IS CLEAR SINCE THIS IS LINKED TO UI)</p>
<p>(NOTE:&nbsp;If they come out with templates AND drafts, consider splitting this article to keep Create in one and Working with Drafts and Requests in another??)</p>
<p>(NOTE: this article is linked from Submitting Workfront Requests from Salesforce) </p>
</div>
-->

计划工作由项目和任务代表Adobe Workfront。 但是，您可能会在以下环境中工作：计划外工作（以随机请求的形式）可以随时进入。 Workfront提供了一个工作流，可通过使用请求队列来适应此类环境。 

在请求队列中创建请求后，您可以将其分配为完成，也可以将其转换为任务或项目。\
有关将问题转换为任务或项目的详细信息，请参阅文章 [转换Adobe Workfront中的问题概述](../../../manage-work/issues/convert-issues/convert-issues.md).

您可以通过以下方式创建请求：

* 从头开始，如本文所述。
* 从草稿。 有关信息，请参阅 [从草稿创建请求](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).
* 通过复制和提交副本，从现有请求中。 有关信息，请参阅 [复制和提交请求](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## 访问要求

<!--drafted for P&P - replace table: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对问题的访问权限</p> <p>如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 使用请求队列的先决条件

作为Workfront管理员，您必须创建请求队列，并让用户可以使用这些队列，然后才能使用此功能。 具有计划员许可证并具有项目编辑访问权限和管理特定项目权限的用户也可以创建请求队列。 

有关如何创建请求队列的信息，请参阅文章 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

必须创建请求队列的以下组件：

* 处于“当前”状态的项目，作为“帮助请求队列”发布。
* 队列主题.\
   有关更多信息，请参阅文章 [创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

* 路由规则.\
   有关更多信息，请参阅文章 [创建路由规则](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

* （可选）主题组。\
   有关更多信息，请参阅文章 [创建主题组](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

* （可选）请求自定义表单。\
   有关更多信息，请参阅文章 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* （可选）请求批准流程。\
   有关更多信息，请参阅文章 [为工作项创建审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 在Workfront Web应用程序中创建请求并生成草稿

在Workfront Web应用程序中创建请求时，Workfront会先将请求另存为草稿，然后再提交。 Workfront会在您选择请求队列并开始输入其信息后立即创建草稿。

您可以继续提交请求，也可以完成尽可能多的信息，然后离开请求以便稍后完成。 Workfront会保存您在“草稿”文件夹中启动的草稿请求。

>[!IMPORTANT]
>
>处理草稿时请考虑以下事项：
>
>* 当您从第三方应用程序提交草稿请求时，Workfront不会创建草稿请求，例如将草稿发送到Workfront，或使用任何其他应用程序创建草稿请求。 从Workfront Web应用程序外部提交请求时，该请求会保存在已提交部分。
>* 如果请求队列的结构发生更改，您将无法再访问现有草稿。 例如，如果删除了队列主题或添加了主题组，则保存的草稿将不再可访问。
>


有关从现有草稿创建请求的信息，请参阅 [从草稿创建请求](../../../manage-work/requests/create-requests/create-requests-from-drafts.md). 有关删除请求草稿的信息，另请参阅 [删除请求草稿](../../../manage-work/requests/create-requests/delete-request-draft.md).

要在Workfront Web应用程序中创建请求，请执行以下操作： 

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   </MadCap:conditionalText>
   -->

1. 单击  **请求**，然后单击 **新请求** 的双曲余切值。

   >[!TIP]
   >
   >* 您可以从“请求”区域的任意部分访问“新建请求”选项。
   >* 当您无权创建问题时，“新建请求”选项将变暗。


1. （视情况而定）在 **请求类型** 字段中，并执行以下操作之一：

   * 从 **近期路径** 部分，选择最近用于打开请求队列的路径。 路径包括您最近提交到的请求队列、主题组和队列主题。 默认情况下，最后三个路径会显示。

      >[!NOTE]
      >
      >Workfront仅在您向其实际提交了请求时才会保存路径。 它不会为起草的请求创建路径。

      ![](assets/list-of-recent-paths-and-request-queues-when-entering-new-request-nwe-350x295.png)

   * 从 **请求队列** 部分，选择请求队列。
   * 输入属于先前访问路径的关键字以搜索请求队列。

      例如，如果您有一个名为“帮助台”的请求队列，其主题组名为“位置”，队列主题名为“远程”，则可以键入“remote”，并在其路径的任何元素中显示包含“remote”的所有请求队列。

      >[!TIP]
      >
      >在键入包含特殊字符的名称时，即使省略键入字符，也会显示请求队列、队列主题或主题组。

      ![](assets/request-queue-search-findings-with-highlighted-results-350x210.png)

      可用请求队列和最近路径的列表会动态更新，以仅包含结果中突出显示的关键字的路径。

      搜索结果将显示在以下区域下：

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">请求队列</td> 
        <td>名称中包含关键词的请求队列</td> 
       </tr> 
       <tr> 
        <td role="rowheader">请求路径</td> 
        <td> <p>包含关键字的路径（包括请求队列、主题组、队列主题），位于其任何元素名称中</p> </td> 
       </tr> 
      </tbody> 
     </table>
   >[!TIP]
   >
   >* 默认情况下，前200个请求队列按字母顺序显示。
   >* 请求队列的名称是已作为帮助请求队列发布的项目的名称。
   >* 配置为选定请求队列的项目描述将显示在请求队列名称的右侧。

   >   
   >有关如何将项目作为帮助请求队列发布的更多信息，请参阅文章 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 在 **新请求** 表单中，执行下列操作之一：

   * （视情况而定）从“请求类型”字段下显示的通知消息中选择一个可用的草稿。

      仅当您在未提交草稿之前保存了草稿时，才会显示此区域。

      默认情况下，将显示来自三个不同队列主题的三个最新草稿。

      ![](assets/new-drafts-after-new-request-area-was-removed-350x162.png)

   * 开始在所选队列中输入新请求。

      在开始输入新请求的信息并在“主题”字段中为请求提供名称后，“草稿”部分会自动为您保存新草稿。

1. （可选）如果请求队列包含主题组，请在第一个下拉字段中选择主题组的名称。 否则，请选择队列主题。

   >[!TIP]
   将鼠标悬停在主题组或队列主题上时，右侧会显示描述字段。 其中包含有关主题组或队列主题的其他信息。
   ![](assets/show-description-on-queue-topic-when-submitting-request-nwe-350x81.png)   >

   您的请求队列中最多可以内置10层主题组。\
   有关如何创建主题组的更多信息，请参阅文章 [创建主题组](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). 有关创建队列主题的更多信息，请参阅文章 [创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   >[!TIP]
   如果您选择了草稿或以前的路径，则主题组和队列主题已被选择。 您可以根据需要选择其他选项。

1. 根据Workfront管理员在 **新问题字段** 部分 **队列详细信息** 在项目上，您可能会在提交新请求时找到以下任何字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>主题</strong> </td> 
      <td>指定请求的名称。 这是必填字段。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>描述</strong> </td> 
      <td>为请求指定描述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>指定可能与您的请求相关的URL。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>优先级</strong> </td> 
      <td> <p>为请求指定优先级。 优先级应定义您认为此请求应解决的速度。 默认选项为： </p> 
       <ul> 
        <li>无</li> 
        <li>低 </li> 
        <li>正常</li> 
        <li>高</li> 
        <li>紧急</li> 
       </ul> <p>系统管理员可以修改优先级的名称。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>严重程度</strong> </td> 
      <td> <p>为请求指定严重性。 严重性应定义此请求对您的工作造成的影响，以防其及时得到解决。 默认选项为：</p> 
       <ul> 
        <li>轻微</li> 
        <li>导致混淆</li> 
        <li>有变通方案的问题</li> 
        <li>没有变通方案的问题</li> 
        <li>致命错误</li> 
       </ul> <p>系统管理员可以修改严重性的名称。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>主要联系人</strong> </td> 
      <td>请求的主要联系人默认为您，因为您是解决与请求相关的任何问题的指点人员。 但是，您可以将其更改为任何其他Workfront用户。</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>分配</strong> </td> 
      <td> <p><span>指定应将请求分配给的活动用户、作业角色或团队的名称。</span> </p> <p>您只能指定一个团队。</p>

   <p> 根据请求队列的设置方式，您可能只能向请求分配一两种类型的资源，而不能分配所有三种资源（例如，您可能只能向用户分配请求）。</p>

   <p>如果路由规则也与请求队列相关联，并且它自动将请求路由到不同类型的资源（例如，团队），则您的请求将分配给您在提交请求时手动指定的实体（用户）和路由规则中指定的资源（团队）。 </p>

   <p> 有关更多信息，请参阅以下文章：</p> 
      <ul> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">创建请求队列</a> </p> </li> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">创建路由规则</a> <br> </p> </li> 
      </ul> </p>

   <p><span>我们建议对您的请求队列使用路由规则，以便它们能够被自动路由到相应的资源。</span> </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>计划小时</strong> </td> 
      <td> <p>估计完成此请求需要多少小时。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>计划开始日期</strong> </td> 
      <td> <p>指定应开始处理此请求的日期。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>计划完成日期</strong> </td> 
      <td>指定希望解决此请求的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>状态</strong> </td> 
      <td>新请求的默认状态为“新”。 您的系统管理员可能已更改此状态的名称。 您还可以从此下拉菜单中将状态更改为其他内容。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文档</strong> </td> 
      <td> <p>向请求中添加文档。 </p> <p> 根据请求队列的设置方式，“文档”部分可能显示在自定义字段之前或之后。 </p> <p>您上传到Workfront的文档将按照起草的请求存储24小时。 之后，在返回编辑并提交草稿时，必须重新附加它们。 从其他驱动器链接的文档将永久保存在草稿中。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）如果Workfront管理员将自定义表单与请求队列或队列主题关联，请指定自定义表单中的字段。\
   每个Workfront实例的自定义表单都不同。 
1. （可选和视情况而定）在输入请求期间的任意时间点，单击 [!UICONTROL **放弃草稿**] 如果要删除自动创建的草稿，请执行此操作。 这将删除无法恢复的草稿。 此时将显示确认消息，确认您正在删除草稿。

1. （可选）单击 [!UICONTROL **撤消**] 确认消息中的。

1. 执行下列操作之一：

   * 单击 **提交** 如果您已准备好提交请求。 请求保存在已提交部分中。 根据请求队列的路由规则，此请求可能会路由到与指定为请求队列的项目不同的项目。 有关路由规则的信息，请参阅 [创建路由规则](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

      或

      单击 **关闭** 如果您还未准备好提交它，则可能稍后返回并完成它。 您的请求将保存在“草稿”部分，下次提交此请求队列的请求时，您将可以使用该请求。

      ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)
   提交请求时，草稿会自动删除且无法还原。

   有关处理传入请求的信息，请参阅文章 [管理工作和团队请求](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

   有关查找已提交或起草的请求的信息，另见 [查找提交的请求](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

## 从Workfront外部创建请求

在提交新请求并将其嵌入到其他应用程序时，您可以共享指向请求队列的直接链接。 从Web或其他应用程序访问此链接的用户还必须使用活动的Workfront帐户登录，才能访问此队列并向其提交请求。 有关信息，请参阅 [共享到请求队列的链接](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## 通过向Workfront发送电子邮件来创建请求

如果您的请求队列已启用通过电子邮件接收请求，则可以将请求直接通过电子邮件发送到与请求队列关联的电子邮件。

电子邮件的正文文本将作为请求描述添加。

>[!NOTE]
请求进入Workfront时，会清除HTML格式，但不会清除签名和现有的回复线程内容，并在请求描述中显示。

有关如何启用请求队列以通过电子邮件接收请求的信息，请参阅 [允许用户将问题通过电子邮件发送到请求队列项目](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## 使用Outlook客户端创建请求

您可以使用Outlook客户端提交请求。 您可以创建新请求，也可以将电子邮件转换为请求。 

有关使用Outlook客户端提交请求的信息，请参阅文章 [通过Outlook电子邮件创建Adobe Workfront请求](../../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).

## 使用Workfront移动设备应用程序创建请求

您可以在智能手机上使用移动应用程序提交请求。 您可以创建新请求，并将其提交到您有权在Web应用程序中查看的请求队列。 

有关通过移动设备应用程序提交请求的信息，请参阅 [请求](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md#requests) 章节：

* [Adobe Workfront for Android](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md)
* [Adobe Workfront for iOS](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md)

## 从其他应用程序创建请求

您可以使用任何已与Workfront集成的应用程序提交请求： 

* 您可以在Workfront与其他应用程序之间构建自定义集成，以便从其他应用程序向Workfront提交请求。\
   有关自定义Workfront集成的更多信息，请参阅文章 [Adobe Workfront集成](../../../administration-and-setup/configure-integrations/workfront-integrations-1.md).

* 如果已安装适用于Salesforce的Workfront应用程序，则可以提交来自Salesforce的请求。\
   有关使用我们的Workfront for Salesforce应用程序提交Salesforce请求的信息，请参阅文章 [从Salesforce对象提交Adobe Workfront请求](../../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

## 查找提交的请求

有关查找已提交或已起草的请求的信息，请参见 [查找提交的请求](../../../manage-work/requests/create-requests/locate-submitted-requests.md).
