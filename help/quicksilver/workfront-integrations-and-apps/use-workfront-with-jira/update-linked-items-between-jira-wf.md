---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: 更新链接项目之间 [!DNL Jira] 和 [!DNL Adobe Workfront]
description: 链接时 [!DNL Jira] 问题 [!DNL Adobe Workfront] 任务或问题时，您的用户可以更新一个应用程序中的项目，并且该项目的对应项也会为在第二个应用程序中工作的用户进行更新。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '1703'
ht-degree: 0%

---

# 更新链接项目之间 [!DNL Jira] 和 [!DNL Adobe Workfront]

链接时 [!DNL Jira] 问题 [!DNL Adobe Workfront] 任务或问题时，您的用户可以更新一个应用程序中的项目，并且该项目的对应项也会为在第二个应用程序中工作的用户进行更新。

有关在 [!DNL Workfront] 和 [!DNL Jira]，请参阅 [在Adobe Workfront和Jira之间链接项目](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

在设置 [!DNL Workfront] 表示 [!DNL Jira]，作为 [!DNL Jira] 系统管理员，您可以配置一个应用程序中的某些字段，以便与另一个应用程序中链接项目中的字段同步。

有关在链接的字段之间同步字段的更多信息 [!DNL Jira] 和 [!DNL Workfront] 项目，请参阅 [配置 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] 计划</a>*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] 许可证概述</a>*</td> 
   <td> <p>[!UICONTROL计划]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 访问</td> 
   <td> <p>系统管理员访问权限</p> <p>重要信息：我们建议您在 [!DNL Jira] 和 [!DNL Workfront] 专门用于此集成，而不是使用可能附加到用户的现有集成。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。 有关 [!DNL Workfront] 管理员，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 先决条件

在您关联项目之前 [!DNL Workfront] 和 [!DNL Jira]，您必须

* 安装 [!DNL Workfront for Jira].

   有关安装的说明 [!DNL Workfront for Jira]，请参阅 [安装 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* 配置 [!DNL Workfront for Jira].

   有关配置的说明 [!DNL Workfront for Jira]，请参阅 [配置 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* 链接项目之间 [!DNL Workfront] 和 [!DNL Jira].

   有关说明，请参阅 [链接项目之间 [!DNL Adobe Workfront] 和 [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## 更新中的链接项目 [!DNL Workfront]

如果您主要在 [!DNL Workfront]，您可以在 [!DNL Workfront] 和同行 [!DNL Jira] 也会更新。 此更新通过 [!DNL Workfront] 表示 [!DNL Jira] 不要求你 [!DNL Jira] 许可证。

只要 [!DNL Workfront] 管理员已配置 [!DNL Workfront for Jira] 要同步链接项目之间的字段，请在 [!DNL Workfront] 链接的 [!DNL Jira] 问题。 有关更新 [!DNL Workfront]，请参阅 [编辑问题](../../manage-work/issues/manage-issues/edit-issues.md) 和 [编辑任务](../../manage-work/tasks/manage-tasks/edit-tasks.md).

下表显示了 [!DNL Workfront] 字段与同步 [!DNL Jira] 链接项目上的字段：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>已更新 [!DNL Workfront] 字段</strong> </th> 
   <th><strong>已同步 [!DNL Jira] 字段/更新</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL问题或任务名称]</td> 
   <td> <p>[!UICONTROL问题名称]</p> <p>有关名称更改的评论将添加到 <strong>[!DNL Workfront]</strong> 选项卡 [!DNL Jira] 问题。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL问题或任务描述]</td> 
   <td> <p> [!UICONTROL问题描述]</p> <p>有关更新描述的注释将添加到 <strong>[!DNL Workfront]</strong> 选项卡 [!DNL Jira] 问题。<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL已上传文档]</p> <p>注意：链接到的文档 [!DNL Workfront] 来自外部服务器的项目不会传输到 [!DNL Jira] 问题。 仅上传到 [!DNL Workfront] 项目也会更新为链接的 [!DNL Jira] 问题。 </p> </td> 
   <td> <p>[!UICONTROL附件]</p> <p>有关已上传附件的评论会添加到 <strong>[!DNL Workfront]</strong> 选项卡 [!DNL Jira] 问题。<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计划完成日期]</td> 
   <td> <p>[!UICONTROL到期日期]</p> <p>有关[!UICONTROL到期日期]已更改的注释将添加到 [!DNL Workfront] 选项卡 [!DNL Jira] 问题。 </p> <p>注意：必须启用 <strong>[!UICONTROL到期日期]</strong> , [!DNL Jira] 无法在[!UICONTROL Jira]中查看此字段更新的问题。 </p> </td> 
  </tr> 
  <tr> 
   <td>自定义Forms和自定义字段</td> 
   <td> <p> 在 [!DNL Workfront] 右侧面板 [!DNL Jira] 问题。 <br>面板中仅显示具有实际值的自定义字段。<br></p> <p>注意：自定义表单部分会显示 [!DNL Workfront] 管理员。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL问题或任务优先级]</td> 
   <td>在 [!DNL Workfront] 右侧面板 [!DNL Jira] 问题。 <br>它不会更新问题 <strong>[!UICONTROL优先级]</strong> 字段 [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日志时间] </td> 
   <td> <p>有关已记录时间的评论将添加在 <strong>[!DNL Workfront]</strong> 选项卡 [!DNL Jira] 问题。 这包括记录时间的用户的名称，以及记录时间的用户（如果时间不同）的名称。 未在 <strong>[!UICONTROL工作日志]</strong> 选项卡 [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL注释]</td> 
   <td> <p>该评论会添加到 <strong>[!DNL Workfront]</strong> 选项卡 [!DNL Jira] 问题。 它不会添加到 <strong>[!UICONTROL注释]</strong> 选项卡 [!DNL Jira] 问题</p> <p>注意：手动链接两个现有项目时，添加到 [!DNL Workfront] 将项目链接到之前的项目 [!DNL Jira] 不同步到 [!DNL Jira] 问题。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 更新中的链接项目 [!DNL Jira]

如果您主要在 [!DNL Jira]，您可以在 [!DNL Jira] 和同行 [!DNL Workfront] 也会更新。 您不必拥有 [!DNL Workfront] 许可证 [!DNL Workfront] 链接到 [!DNL Jira] 接收您在中进行的更新时出现问题 [!DNL Jira].

以 [!DNL Workfront] 管理员已配置 [!DNL Workfront] 表示 [!DNL Jira] 要同步链接项目之间的字段，请在中更新某些字段 [!DNL Jira] 链接的 [!DNL Workfront] 项目。

下表显示了 [!DNL Jira] 字段与同步 [!DNL Workfront] 链接项目上的字段：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>已更新 [!DNL Jira] 字段</strong> </th> 
   <th><strong>已同步 [!DNL Workfront] 字段/更新</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL问题状态]</td> 
   <td> <p> [!UICONTROL问题或任务状态]</p> <p>中的问题状态 [!DNL Jira] 在Workfront中同步以下状态或与以下状态等同的状态：</p> 
    <ul> 
     <li> <p>[!UICONTROL新建]（[!UICONTROL新建]）</p> </li> 
     <li> <p>[!UICONTROL正在进行]([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Closed]/[!UICONTROL Complete]([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>注意：的 [!DNL Jira] 状态与第一个同步 [!DNL Workfront] 状态等于适当状态。</p> <p>有关中项目状态的更多信息 [!DNL Workfront]，请参阅 <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">创建或编辑状态</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL问题被分派人]</td> 
   <td> <p> [!UICONTROL问题或任务被分派人]</p> <p>重要信息：在 [!DNL Jira] 向没有 [!DNL Workfront] 帐户，则集成会在 [!DNL Workfront] 仅当选项“[!UICONTROL自动在 [!DNL Workfront] 如果 [!DNL Jira] 用户没有 [!DNL Workfront] account]”设置为[!UICONTROL Always]。 此用户不占用 [!DNL Workfront] 许可证。 可以将活动用户分配到 [!DNL Workfront]，但不能包含在更新中。 有关配置自动创建的 [!DNL Workfront] 用户 [!DNL Jira]，请参阅 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">配置 [!DNL Workfront for Jira]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL问题附件]</td> 
   <td> [!UICONTROL问题或任务文档]<br>有关在 [!DNL Jira] 已添加到的[!UICONTROL Updates]选项卡 [!DNL Workfront] 问题或任务。  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL到期日期]</td> 
   <td> <p> 关于[!UICONTROL到期日]在 [!DNL Jira] 已添加到的[!UICONTROL Updates]选项卡 [!DNL Workfront] 问题或任务。 </p> <p>注意：在 [!DNL Workfront] 问题或任务。 </p> </td> 
  </tr> 
  <tr> 
   <td> 在 [!DNL Workfront] 右侧面板或[!UICONTROL More]菜单中的 [!DNL Jira] 问题<br></td> 
   <td> <p>小时<br>除了将Jira中记录的小时数添加到链接的 [!DNL Workfront] 项目时，有关日志记录时间的注释会添加到的[!UICONTROL更新]选项卡中 [!DNL Workfront] 项目。</p> <p>有关链接的日志记录时间的更多信息 [!DNL Jira] 问题，包括更新 [!DNL Jira] 正在登录时间的用户 [!DNL Workfront]，请参阅 <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">链接的日志时间 [!DNL Jira] 和 [!DNL Workfront] 项目</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> 注释 <br><br></td> 
   <td> <p>注释会添加到的[!UICONTROL Updates]选项卡中 [!DNL Workfront] 问题或任务(如果 <strong>[!UICONTROL注释]</strong> 在[!UICONTROL设置]选项卡的[!UICONTROL从JIRA同步到WORKFRONT]部分中设置为 <strong>[!UICONTROL Always]</strong>.</p> <p>有关在中配置Workfront设置的信息 [!DNL Jira]，请参阅 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">配置 [!DNL Workfront for Jira]</a>.</p> <p>有关对链接项目进行注释的信息 [!DNL Jira] 问题，请参阅 <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">来自链接的评论 [!DNL Jira] 问题</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 从链接的日志时间 [!DNL Jira] 问题

您记录 [!DNL Jira] 项目 [!DNL Jira] 也会转给链接的 [!DNL Workfront] 项目，不考虑 [!DNL Jira] 你记录时间。\
当您在Jira中登录时， [!DNL Workfront] 面板，则时间仅在 [!DNL Workfront].\
您在 [!DNL Workfront] 不影响 [!DNL Jira].

>[!NOTE]
>
>如果时间被添加到 [!DNL Jira] 链接到的项目 [!DNL Workfront] 任务， [!UICONTROL 小时类型] 在 [!DNL Workfront] is [!UICONTROL 任务时间]. 如果时间被添加到 [!DNL Jira] 链接到的项目 [!DNL Workfront] 问题， [!UICONTROL 小时类型] 在 [!DNL Workfront] is [!UICONTROL 问题时间].

评论会添加到 **[!DNL Workfront]** 选项卡 [!DNL Jira] 和 **[!UICONTROL 更新]** 选项卡 [!DNL Workfront] 记录记录时间。\
时间也会显示在 **[!UICONTROL 小时]** 选项卡 [!DNL Workfront] 项目。

* [链接的日志时间 [!DNL Jira] 和 [!DNL Workfront] 项目](#log-time-for-linked-jira-and-workfront-items)
* [记录时间 [!DNL Jira] 至 [!DNL Workfront] 项目](#log-time-from-jira-to-a-workfront-item)

### 链接的日志时间 [!DNL Jira] 和 [!DNL Workfront] 项目

您可以从 [!DNL Jira] 链接到的问题 [!DNL Workfront] 项目，并且时间都记录在 [!DNL Jira] 问题以及 [!DNL Workfront] 项目。

>[!IMPORTANT]
>
>如果用户在 [!DNL Jira] 中不存在 [!DNL Workfront]，则集成会在Workfront中创建新的活动用户(如果 **[!UICONTROL 在中自动创建用户 [!DNL Workfront]&#x200B;如果 [!DNL Jira] 用户没有&#x200B;*[!DNL Workfront]&#x200B;帐户]**设置为**[!UICONTROL &#x200B;始终&#x200B;]**. 此用户不占用 [!DNL Workfront] 许可证。 您可以将活动用户分配到 [!DNL Workfront]，但是您不能在更新中包含它们。 有关配置自动创建的信息 [!DNL Workfront] 用户 [!DNL Jira]，请参阅 [配置 [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

在 [!DNL Jira] 把两个都录下来 [!DNL Jira] 和 [!DNL Workfront]:

1. 登录 [!DNL Jira].
1. 转到 [!DNL Jira] 链接到 [!DNL Workfront] 项目。
1. 展开 **[!UICONTROL 更多]** 菜单，单击 **[!UICONTROL 日志工作]**.

1. 在 **[!UICONTROL 逗留时间]** 字段，指定处理此问题所花费的时间。 您必须使用以下时间段指定时间：

   * [!UICONTROL 周] (w)
   * [!UICONTROL 天] (d)
   * [!UICONTROL 小时] (h)

1. 继续向时间条目添加信息，包括 **[!UICONTROL 工作描述]**，然后单击 **[!UICONTROL 日志]**.\
   时间会添加到 **[!UICONTROL 工作日志]** 选项卡 [!DNL Jira] 项目，以及 [!DNL Workfront] 链接到该项目的项目。\
   时间条目的工作描述将记录为中小时条目的注释 [!DNL Workfront].

### 记录时间 [!DNL Jira] 至 [!DNL Workfront] 项目

您只需将时间记录到链接的 [!DNL Workfront] 项目 [!DNL Jira] 此时未将问题记录到 [!DNL Jira] 问题。

1. 登录 [!DNL Jira].
1. 导航到 [!DNL Jira] 链接到 [!DNL Workfront] 项目。

   详细信息 [!DNL Workfront] 项目应显示在 [!DNL Workfront] 问题的右侧面板。

1. 单击 **[!UICONTROL 日志时间]** 图标。

1. 指定 **[!UICONTROL 小时]** 和 **[!UICONTROL 分钟]** 要记录问题。

1. 单击 **[!UICONTROL 日志时间]**.

   时间会添加到 [!DNL Workfront] 项目。

   此时间不会添加到 [!UICONTROL 工作日志] 选项卡 [!DNL Jira] 问题。

## 来自链接的评论 [!DNL Jira] 问题 {#comment-from-a-linked-jira-issue}

当您对 [!DNL Jira] 项目 [!DNL Workfront] 右侧面板 [!DNL Jira]，则也会在 [!UICONTROL 更新] 选项卡。

要从中评论 [!DNL Jira] 至 [!DNL Workfront] 项目：

1. 登录 [!DNL Jira].
1. 导航到 [!DNL Jira] 链接到 [!DNL Workfront] 项目。

   详细信息 [!DNL Workfront] 项目应显示在 [!DNL Workfront] 问题的右侧面板。

1. 单击 **[!UICONTROL 评论]** 图标 [!DNL Workfront] 面板或 **[!UICONTROL 评论]** 选项卡。

1. 开始键入评论，然后单击 **[!UICONTROL 发送]**.

   该评论将添加到以下内容：

   * 的 **[!DNL Workfront]** 选项卡 [!DNL Jira] 问题。
   * 的 **[!UICONTROL 评论]** 选项卡 [!DNL Jira] 问题。
   * 的 **[!UICONTROL 更新]** 选项卡。
