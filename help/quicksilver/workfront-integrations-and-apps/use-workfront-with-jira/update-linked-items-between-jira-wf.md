---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: 更新 [!DNL Jira] 和 [!DNL Adobe Workfront]之间的链接项
description: 当您将 [!DNL Jira] 问题链接到 [!DNL Adobe Workfront] 任务或问题时，您的用户可以更新一个应用程序中的项目，该项目的对应项也会更新第二个应用程序中工作的用户。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: 99924f690c53584c090d19fff90d23d84ec306d4
workflow-type: tm+mt
source-wordcount: '1576'
ht-degree: 0%

---

# 更新[!DNL Jira]和[!DNL Adobe Workfront]之间的链接项

当您将[!DNL Jira]问题链接到[!DNL Adobe Workfront]个任务或问题时，您的用户可以在一个应用程序中更新项目，该项目的对应项也会针对在第二个应用程序中工作的用户进行更新。

有关在[!DNL Workfront]和[!DNL Jira]之间链接项目的详细信息，请参阅[在Adobe Workfront和Jira之间链接项目](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md)。

在为[!DNL Jira]设置[!DNL Workfront]时，作为[!DNL Jira]系统管理员，您可以配置一个应用程序中的某些字段，使其与另一个应用程序中链接项中的字段同步。

有关在链接的[!DNL Jira]和[!DNL Workfront]项之间同步字段的更多信息，请参阅[配置 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td><p>新建：任何</p>
       <p>或</p>
       <p>当前： [！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td><p>新文档： [！UICONTROL Standard]</p>
       <p>或</p>
       <p>当前： [！UICONTROL计划]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 访问</td> 
   <td> <p>系统管理员访问权限</p> <p>重要提示：建议您在[!DNL Jira]和[!DNL Workfront]中创建单独的系统管理员帐户以专门用于此集成，而不是使用可能附加到用户的现有帐户。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是[!DNL Workfront]管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 先决条件

在链接[!DNL Workfront]和[!DNL Jira]之间的项目之前，您必须：

* 安装[!DNL Workfront for Jira]。

  有关安装[!DNL Workfront for Jira]的说明，请参阅[安装 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)。

* 配置[!DNL Workfront for Jira]。

  有关配置[!DNL Workfront for Jira]的说明，请参阅[配置 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)。

* [!DNL Workfront]和[!DNL Jira]之间的链接项。

  有关说明，请参阅[链接介于 [!DNL Adobe Workfront] 和 [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md)之间的项目。

## 更新[!DNL Workfront]中的链接项

如果您主要在[!DNL Workfront]中工作，则可以在[!DNL Workfront]中更新工作项，而在[!DNL Jira]中的对应工作项也会更新。 此更新是通过[!DNL Jira]的[!DNL Workfront]集成进行的，它不需要您拥有[!DNL Jira]许可证。

只要[!DNL Workfront]管理员已将[!DNL Workfront for Jira]配置为同步链接项之间的字段，则您在[!DNL Workfront]中更新的某些字段也会更新链接的[!DNL Jira]问题。 有关更新[!DNL Workfront]中项目的详细信息，请参阅[编辑问题](../../manage-work/issues/manage-issues/edit-issues.md)和[编辑任务](../../manage-work/tasks/manage-tasks/edit-tasks.md)。

以下列表显示了与链接项中的[!DNL Jira]字段同步的[!DNL Workfront]字段：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>已更新[!DNL Workfront]字段</strong> </th> 
   <th><strong>已同步[!DNL Jira]字段/更新</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL问题或任务名称]</td> 
   <td> <p>[！UICONTROL问题名称]</p> <p>有关名称更改的注释已添加到[!DNL Jira]问题的<strong>[!DNL Workfront]</strong>选项卡中。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL问题或任务描述]</td> 
   <td> <p> [！UICONTROL问题说明]</p> <p>有关已更新描述的注释已添加到[!DNL Jira]问题的<strong>[!DNL Workfront]</strong>选项卡中。<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [！UICONTROL上载的文档]</p> <p>注意：链接到来自外部服务器的[!DNL Workfront]项的文档未传输到[!DNL Jira]问题。 只有直接上传到[!DNL Workfront]项的文档也会更新为链接的[!DNL Jira]问题。 </p> </td> 
   <td> <p>[！UICONTROL附件]</p> <p>有关已上载附件的注释已添加到[!DNL Jira]问题的<strong>[!DNL Workfront]</strong>选项卡中。<br></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划完成日期]</td> 
   <td> <p>[！UICONTROL到期日期]</p> <p>已更改的[！UICONTROL截止日期]的注释已添加到[!DNL Jira]问题的[!DNL Workfront]选项卡中。 </p> <p>注意：必须为您的[!DNL Jira]问题启用<strong>[！UICONTROL到期日期]</strong>，才能在[！UICONTROL Jira]中看到此字段的更新。 </p> </td> 
  </tr> 
  <tr> 
   <td>自定义Forms和自定义字段</td> 
   <td> <p> 显示在[!DNL Jira]问题的[!DNL Workfront]右侧面板中。 <br>面板中仅显示具有实际值的自定义字段。<br></p> <p>注意：自定义表单分区以[!DNL Workfront]管理员的访问级别显示。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL问题或任务优先级]</td> 
   <td>显示在[!DNL Jira]问题的[!DNL Workfront]右侧面板中。 <br>它不更新[!DNL Jira]中的问题<strong>[！UICONTROL优先级]</strong>字段。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日志时间] </td> 
   <td> <p>有关记录时间的注释已添加到[!DNL Jira]问题的<strong>[!DNL Workfront]</strong>选项卡中。 这包括记录时间的用户的名称，以及在时间不同时为其记录时间的用户的名称。 [!DNL Jira]中的<strong>[！UICONTROL工作日志]</strong>选项卡中未记录任何时间。<br></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Comments]</td> 
   <td> <p>该评论已添加到[!DNL Jira]问题的<strong>[!DNL Workfront]</strong>选项卡。 它未添加到[!DNL Jira]问题的<strong>[！UICONTROL评论]</strong>选项卡中</p> <p>注意：当您手动链接两个现有项时，在将其链接到[!DNL Jira]之前添加到[!DNL Workfront]项的注释不会同步到[!DNL Jira]问题。 </p> <p>Jira注释与Workfront同步。</td> 
  </tr> 
 </tbody> 
</table>

## 更新[!DNL Jira]中的链接项

如果您主要在[!DNL Jira]中工作，则可以在[!DNL Jira]中更新工作项，而在[!DNL Workfront]中的对应工作项也会更新。 对于链接到[!DNL Jira]问题的[!DNL Workfront]项目，您不必拥有[!DNL Workfront]许可证即可接收您在[!DNL Jira]中进行的更新。

在您的[!DNL Workfront]管理员已为[!DNL Jira]配置[!DNL Workfront]以同步链接项之间的字段的情况下，您在[!DNL Jira]中更新的某些字段也会更新链接的[!DNL Workfront]项。

以下列表显示了与链接项中的[!DNL Workfront]字段同步的[!DNL Jira]字段：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>已更新[!DNL Jira]字段</strong> </th> 
   <th><strong>已同步[!DNL Workfront]字段/更新</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL问题状态]</td> 
   <td> <p> [！UICONTROL问题或任务状态]</p> <p>[!DNL Jira]中的问题状态与Workfront中的以下状态或等于以下状态的状态同步：</p> 
    <ul> 
     <li> <p>[！UICONTROL New] ([！UICONTROL NEW])</p> </li> 
     <li> <p>[！UICONTROL正在进行中] ([！UICONTROL INP])</p> </li> 
     <li> <p>[！UICONTROL已关闭]/[！UICONTROL完成] ([！UICONTROL CLS]/[！UICONTROL CPL])</p> </li> 
    </ul> <p>注意： [!DNL Jira]状态与对应于相应状态的前[!DNL Workfront]状态同步。</p> <p>有关[!DNL Workfront]中项目状态的详细信息，请参阅<a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">创建或编辑状态</a>。</p> </td> 
  </tr>
  <tr> 
   <td>[！UICONTROL问题附件]</td> 
   <td> [！UICONTROL问题或任务文档]<br>有关在[!DNL Jira]中上传新文档的注释已添加到[!DNL Workfront]问题或任务的[！UICONTROL更新]选项卡中。  </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL到期日期]</td> 
   <td> <p> 有关[!DNL Jira]中[！UICONTROL截止日期]更改的注释已添加到[!DNL Workfront]问题或任务的[！UICONTROL更新]选项卡中。 </p> <p>注意：[!DNL Workfront]问题或任务未更改日期。 </p> </td> 
  </tr> 
  <tr> 
   <td> 在[!DNL Workfront]右侧面板中或从[!DNL Jira]问题上的[！UICONTROL更多]菜单记录时间<br></td> 
   <td> <p>小时数<br>除了将在Jira中记录的小时数添加到链接的[!DNL Workfront]项目之外，还向[!DNL Workfront]项目的[！UICONTROL更新]选项卡添加了有关记录时间的注释。</p> <p>有关在链接的[!DNL Jira]问题上记录时间的详细信息，包括更新在[!DNL Workfront]中记录时间的[!DNL Jira]用户，请参阅链接的[!DNL Jira]和[!DNL Workfront]项的<a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">记录时间</a>。</p> </td> 
  </tr> 
  <tr> 
   <td> 评论 <br><br></td> 
   <td> <p>如果[！UICONTROL Setup]选项卡的[！UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT]部分中的<strong>[！UICONTROL Comments]</strong>设置是<strong>[！UICONTROL Always]</strong>，则评论会添加到[!DNL Workfront]问题或任务的[！UICONTROL Updates]选项卡中。</p> <p>有关在[!DNL Jira]中配置Workfront设置的信息，请参阅<a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">配置[!DNL Workfront for Jira]</a>。</p> <p>有关对链接[!DNL Jira]问题中的项进行评论的信息，请参阅链接[!DNL Jira]问题</a>中的<a href="#comment-from-a-linked-jira-issue" class="MCXref xref">评论。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 记录链接[!DNL Jira]问题的时间

您在[!DNL Jira]中为[!DNL Jira]项记录的时间也将传输到链接的[!DNL Workfront]项，无论您在[!DNL Jira]中的哪个位置记录该时间。\
当您在[!DNL Workfront]面板中以Jira记录时间时，时间仅记录在[!DNL Workfront]中。\
您在[!DNL Workfront]中记录的时间不会影响[!DNL Jira]中链接问题的时间。

>[!NOTE]
>
>如果将时间添加到链接到[!DNL Workfront]任务的[!DNL Jira]项中，则[!DNL Workfront]中时间的[!UICONTROL 小时类型]为[!UICONTROL 任务时间]。 如果将时间添加到链接到[!DNL Workfront]问题的[!DNL Jira]项中，则[!DNL Workfront]中时间的[!UICONTROL 小时类型]为[!UICONTROL 问题时间]。

已将评论添加到[!DNL Jira]中的&#x200B;**[!DNL Workfront]**&#x200B;选项卡和[!DNL Workfront]中项目的&#x200B;**[!UICONTROL 更新]**&#x200B;选项卡以记录日志记录时间。\
时间还显示在[!DNL Workfront]项的&#x200B;**[!UICONTROL 小时]**&#x200B;选项卡中。

* [为链接的 [!DNL Jira] 和 [!DNL Workfront] 项记录时间](#log-time-for-linked-jira-and-workfront-items)
* [将时间从 [!DNL Jira] 记录到 [!DNL Workfront] 项](#log-time-from-jira-to-a-workfront-item)

### 已链接[!DNL Jira]和[!DNL Workfront]项的日志记录时间

您可以记录链接到[!DNL Workfront]项的[!DNL Jira]问题的时间，该时间记录在[!DNL Jira]问题和[!DNL Workfront]项中。

>[!IMPORTANT]
>
>如果在[!DNL Jira]中记录时间的用户在[!DNL Workfront]中不存在，则集成会在Workfront中创建一个新的活动用户(如果&#x200B;**[!UICONTROL 在[!DNL Workfront]中自动创建用户(&#x200B;如果[!DNL Jira]用户没有&#x200B;*[!DNL Workfront]帐&#x200B;户]**)设置为**[!UICONTROL &#x200B;始终&#x200B;]**)。 此用户未占用[!DNL Workfront]许可证。 您可以将活动用户分配给[!DNL Workfront]中的工作项，但不能将其包含在更新中。 有关配置从[!DNL Jira]自动创建[!DNL Workfront]用户的信息，请参阅[配置 [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)。

要在[!DNL Jira]中记录项目的时间，并在[!DNL Jira]和[!DNL Workfront]中记录该时间，请执行以下操作：

1. 登录[!DNL Jira]。
1. 转到链接到[!DNL Workfront]项目的[!DNL Jira]问题。
1. 展开&#x200B;**[!UICONTROL 更多]**&#x200B;菜单并单击&#x200B;**[!UICONTROL 记录工作]**。

1. 在&#x200B;**[!UICONTROL 逗留时间]**&#x200B;字段中，指定处理此问题所花费的时间。 您必须使用以下时间段指定时间：

   * [!UICONTROL 周] (w)
   * [!UICONTROL 天] (d)
   * [!UICONTROL 小时] （小时）

1. 继续向时间条目添加信息，包括&#x200B;**[!UICONTROL 工作描述]**，然后单击&#x200B;**[!UICONTROL 日志]**。\
   时间已添加到[!DNL Jira]项的&#x200B;**[!UICONTROL 工作日志]**&#x200B;选项卡，以及链接到它的[!DNL Workfront]项。\
   时间条目的工作描述记录为[!DNL Workfront]中小时条目的注释。

### 将时间从[!DNL Jira]记录到[!DNL Workfront]项

您可以只将时间记录到[!DNL Jira]问题中链接的[!DNL Workfront]项，而无需将时间记录到[!DNL Jira]问题。

1. 登录[!DNL Jira]。
1. 导航到链接到[!DNL Workfront]项目的[!DNL Jira]问题。

   [!DNL Workfront]项目的详细信息应显示在问题的[!DNL Workfront]右侧面板中。

1. 单击&#x200B;**[!UICONTROL 记录时间]**&#x200B;图标。

1. 指定您想为问题记录的&#x200B;**[!UICONTROL 小时]**&#x200B;和&#x200B;**[!UICONTROL 分钟]**&#x200B;的量。

1. 单击&#x200B;**[!UICONTROL 记录时间]**。

   时间已添加到[!DNL Workfront]项。

   此时间未添加到[!DNL Jira]问题的[!UICONTROL 工作日志]选项卡。

## 来自链接[!DNL Jira]问题的评论 {#comment-from-a-linked-jira-issue}

当您在[!DNL Jira]中对[!DNL Workfront]右侧面板中的[!DNL Jira]项进行评论时，该评论也会添加到Workfront中链接项的[!UICONTROL 更新]选项卡中。

要评论从[!DNL Jira]到[!DNL Workfront]项，请执行以下操作：

1. 登录[!DNL Jira]。
1. 导航到链接到[!DNL Workfront]项目的[!DNL Jira]问题。

   [!DNL Workfront]项目的详细信息应显示在问题的[!DNL Workfront]右侧面板中。

1. 单击[!DNL Workfront]面板或&#x200B;**[!UICONTROL 评论]**&#x200B;选项卡上的&#x200B;**[!UICONTROL 评论]**&#x200B;图标。

1. 开始键入评论，然后单击&#x200B;**[!UICONTROL 发送]**。

   该注释将添加到以下内容：

   * [!DNL Jira]问题的&#x200B;**[!DNL Workfront]**&#x200B;选项卡。
   * [!DNL Jira]问题的&#x200B;**[!UICONTROL 评论]**&#x200B;选项卡。
   * Workfront中链接项的&#x200B;**[!UICONTROL 更新]**&#x200B;选项卡。
