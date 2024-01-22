---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: 更新链接项，介于 [!DNL Jira] 和 [!DNL Adobe Workfront]
description: 当您链接时 [!DNL Jira] 问题至 [!DNL Adobe Workfront] 任务或问题，您的用户可以更新一个应用程序中的项目，该项目的对等项也会针对在第二个应用程序中工作的用户进行更新。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: e01f5eaf3133fa1bdaedf4dad56e9a8175b70667
workflow-type: tm+mt
source-wordcount: '1570'
ht-degree: 0%

---

# 更新链接项，介于 [!DNL Jira] 和 [!DNL Adobe Workfront]

当您链接时 [!DNL Jira] 问题至 [!DNL Adobe Workfront] 任务或问题，您的用户可以更新一个应用程序中的项目，该项目的对等项也会针对在第二个应用程序中工作的用户进行更新。

有关链接项目之间的详细信息 [!DNL Workfront] 和 [!DNL Jira]，请参见 [Adobe Workfront和Jira之间的链接项目](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

在您设置时 [!DNL Workfront] 对象 [!DNL Jira]， as a [!DNL Jira] 系统管理员可以配置一个应用程序中的某些字段，使其与另一个应用程序中链接项中的字段同步。

有关在链接字段之间同步的详细信息 [!DNL Jira] 和 [!DNL Workfront] 项，请参阅 [配置 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

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
   <td> <p>系统管理员访问权限</p> <p>重要信息：我们建议您在中创建单独的系统管理员帐户 [!DNL Jira] 和 [!DNL Workfront] 以专门用于此集成，而不使用可能附加到用户的现有集成。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是 [!DNL Workfront] 管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 先决条件

在链接项目之前，请执行以下操作 [!DNL Workfront] 和 [!DNL Jira]，您必须：

* 安装 [!DNL Workfront for Jira].

  有关安装的说明 [!DNL Workfront for Jira]，请参见 [安装 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* 配置 [!DNL Workfront for Jira].

  有关配置的说明 [!DNL Workfront for Jira]，请参见 [配置 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* 链接项目介于 [!DNL Workfront] 和 [!DNL Jira].

  有关说明，请参阅 [链接项目介于 [!DNL Adobe Workfront] 和 [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## 更新中的链接项 [!DNL Workfront]

如果您主要在 [!DNL Workfront]，您可以在以下位置更新您的工作项： [!DNL Workfront] 和他们的同事 [!DNL Jira] 也会更新。 此更新通过集成进行 [!DNL Workfront] 对象 [!DNL Jira] 这不需要你有一个 [!DNL Jira] 许可证。

只要您的 [!DNL Workfront] 管理员已配置 [!DNL Workfront for Jira] 要同步链接项之间的字段，请执行某些更新字段 [!DNL Workfront] 还更新了链接的 [!DNL Jira] 问题。 有关更新中的项目的详细信息 [!DNL Workfront]，请参见 [编辑问题](../../manage-work/issues/manage-issues/edit-issues.md) 和 [编辑任务](../../manage-work/tasks/manage-tasks/edit-tasks.md).

以下列表显示了 [!DNL Workfront] 字段与同步 [!DNL Jira] 链接项中的字段：

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
   <td>[！UICONTROL问题或任务名称]</td> 
   <td> <p>[！UICONTROL问题名称]</p> <p>有关名称变更的注释将添加到 <strong>[!DNL Workfront]</strong> 选项卡 [!DNL Jira] 问题。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL问题或任务描述]</td> 
   <td> <p> [！UICONTROL问题说明]</p> <p>有关已更新描述的注释将添加到 <strong>[!DNL Workfront]</strong> 选项卡 [!DNL Jira] 问题。<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [！UICONTROL上载的文档]</p> <p>注意：链接到的文档 [!DNL Workfront] 来自外部服务器的项目未传输到 [!DNL Jira] 问题。 仅直接上传到的文档 [!DNL Workfront] 项目也会更新到链接的 [!DNL Jira] 问题。 </p> </td> 
   <td> <p>[！UICONTROL附件]</p> <p>有关已上载附件的注释将添加到 <strong>[!DNL Workfront]</strong> 选项卡 [!DNL Jira] 问题。<br></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划完成日期]</td> 
   <td> <p>[！UICONTROL到期日期]</p> <p>有关已更改的[！UICONTROL截止日期]的注释已添加到 [!DNL Workfront] 选项卡 [!DNL Jira] 问题。 </p> <p>注意：必须启用 <strong>[！UICONTROL到期日期]</strong> 您的 [!DNL Jira] 无法看到此字段在[！UICONTROL Jira]中更新的问题。 </p> </td> 
  </tr> 
  <tr> 
   <td>自定义Forms和自定义字段</td> 
   <td> <p> 显示在 [!DNL Workfront] 右侧面板 [!DNL Jira] 问题。 <br>面板中仅显示具有实际值的自定义字段。<br></p> <p>注意：自定义表单部分显示时具有 [!DNL Workfront] 管理员。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL问题或任务优先级]</td> 
   <td>显示在 [!DNL Workfront] 右侧面板 [!DNL Jira] 问题。 <br>它不会更新问题 <strong>[！UICONTROL优先级]</strong> 中的字段 [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日志时间] </td> 
   <td> <p>有关记录时间的注释将添加到 <strong>[!DNL Workfront]</strong> 选项卡 [!DNL Jira] 问题。 这包括记录时间的用户的名称，以及在时间不同时为其记录时间的用户的名称。 没有时间登录 <strong>[！UICONTROL工作日志]</strong> tab in [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Comments]</td> 
   <td> <p>该注释将添加到 <strong>[!DNL Workfront]</strong> 选项卡 [!DNL Jira] 问题。 它不会添加到 <strong>[！UICONTROL Comments]</strong> 选项卡 [!DNL Jira] 问题</p> <p>注意：手动链接两个现有项目时，添加到中的注释 [!DNL Workfront] 项目之前，将其链接到 [!DNL Jira] 不要同步到 [!DNL Jira] 问题。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 更新中的链接项 [!DNL Jira]

如果您主要在 [!DNL Jira]，您可以在以下位置更新您的工作项： [!DNL Jira] 和他们的同事 [!DNL Workfront] 也会更新。 您不必拥有 [!DNL Workfront] 的许可证 [!DNL Workfront] 链接到您的 [!DNL Jira] 接收您在中进行的更新的问题 [!DNL Jira].

前提是 [!DNL Workfront] 管理员已配置 [!DNL Workfront] 对象 [!DNL Jira] 要同步链接项之间的字段，请更新某些字段 [!DNL Jira] 还更新了链接的 [!DNL Workfront] 项目。

以下列表显示了 [!DNL Jira] 字段与同步 [!DNL Workfront] 链接项中的字段：

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
   <td>[！UICONTROL问题状态]</td> 
   <td> <p> [！UICONTROL问题或任务状态]</p> <p>中的问题状态 [!DNL Jira] 在Workfront中同步以下状态，或同步与以下状态相同的状态：</p> 
    <ul> 
     <li> <p>[！UICONTROL New] ([！UICONTROL NEW])</p> </li> 
     <li> <p>[！UICONTROL正在进行中] ([！UICONTROL INP])</p> </li> 
     <li> <p>[！UICONTROL已关闭]/[！UICONTROL完成] ([！UICONTROL CLS]/[！UICONTROL CPL])</p> </li> 
    </ul> <p>注意： [!DNL Jira] 状态与第一个同步 [!DNL Workfront] 与相应状态对应的状态。</p> <p>有关中项目状态的详细信息 [!DNL Workfront]，请参见 <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">创建或编辑状态</a>.</p> </td> 
  </tr>
  <tr> 
   <td>[！UICONTROL问题附件]</td> 
   <td> [！UICONTROL问题或任务文档]<br>有关在中上传新文档的注释 [!DNL Jira] 已添加到[！UICONTROL更新]选项卡的 [!DNL Workfront] 问题或任务。  </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL到期日期]</td> 
   <td> <p> 有关中的[！UICONTROL截止日期]更改的注释 [!DNL Jira] 已添加到[！UICONTROL更新]选项卡的 [!DNL Workfront] 问题或任务。 </p> <p>注意：此日期不会发生任何更改 [!DNL Workfront] 问题或任务。 </p> </td> 
  </tr> 
  <tr> 
   <td> 将时间记录在 [!DNL Workfront] 从右侧面板或[！UICONTROL更多]菜单访问 [!DNL Jira] 问题<br></td> 
   <td> <p>小时<br>除了将在Jira中记录的小时数添加到链接以外 [!DNL Workfront] 项，有关日志记录时间的注释将添加到的[！UICONTROL更新]选项卡中 [!DNL Workfront] 项目。</p> <p>有关链接的日志记录时间的详细信息 [!DNL Jira] 问题，包括更新 [!DNL Jira] 登录时间的用户 [!DNL Workfront]，请参见 <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">链接的日志记录时间 [!DNL Jira] 和 [!DNL Workfront] 个项目</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> 评论 <br><br></td> 
   <td> <p>注释将添加到的[！UICONTROL Updates]选项卡中 [!DNL Workfront] 问题或任务，如果 <strong>[！UICONTROL Comments]</strong> 在[！UICONTROL Setup]选项卡的[！UICONTROL从JIRA同步到WORKFRONT]部分中，设置为 <strong>[！UICONTROL Always]</strong>.</p> <p>有关在中配置Workfront设置的信息 [!DNL Jira]，请参见 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">配置 [!DNL Workfront for Jira]</a>.</p> <p>有关对链接中的项目添加注释的信息 [!DNL Jira] 问题，请参阅 <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">来自链接的评论 [!DNL Jira] 问题</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 记录链接的时间 [!DNL Jira] 问题

您录制的时间 [!DNL Jira] 中的项目 [!DNL Jira] 还将传输到链接的 [!DNL Workfront] 项，无论在何处 [!DNL Jira] 您记录时间。\
当您在 [!DNL Workfront] 时，时间仅记录在 [!DNL Workfront].\
您录制的时间 [!DNL Workfront] 不影响中链接问题的时间 [!DNL Jira].

>[!NOTE]
>
>如果将时间添加到 [!DNL Jira] 链接到的项目 [!DNL Workfront] 任务， [!UICONTROL 小时类型] 表示时间 [!DNL Workfront] 是 [!UICONTROL 任务时间]. 如果将时间添加到 [!DNL Jira] 链接到的项目 [!DNL Workfront] 问题， [!UICONTROL 小时类型] 表示时间 [!DNL Workfront] 是 [!UICONTROL 问题时间].

注释将添加到 **[!DNL Workfront]** tab in [!DNL Jira] 和 **[!UICONTROL 更新]** 中项目的选项卡 [!DNL Workfront] 记录记录时间。\
时间还显示在 **[!UICONTROL 小时]** 选项卡 [!DNL Workfront] 项目。

* [链接的日志记录时间 [!DNL Jira] 和 [!DNL Workfront] 个项目](#log-time-for-linked-jira-and-workfront-items)
* [记录开始时间 [!DNL Jira] 到 [!DNL Workfront] 项目](#log-time-from-jira-to-a-workfront-item)

### 链接的日志记录时间 [!DNL Jira] 和 [!DNL Workfront] 个项目

您可以从以下位置记录时间： [!DNL Jira] 链接到的问题 [!DNL Workfront] ，并且时间记录在 [!DNL Jira] 问题以及 [!DNL Workfront] 项目。

>[!IMPORTANT]
>
>如果用户登录时间 [!DNL Jira] 不存在于 [!DNL Workfront]，则集成会在Workfront中创建一个新的活动用户，如果 **[!UICONTROL 在中自动创建用户 [!DNL Workfront]如&#x200B;果 [!DNL Jira] 用户没有&#x200B;*[!DNL Workfront]帐&#x200B;户]**设置为**[!UICONTROL &#x200B;始终&#x200B;]**. 此用户未占用 [!DNL Workfront] 许可证。 您可以将活动用户分配到中的工作项 [!DNL Workfront]，但不能将它们包含在更新中。 有关配置自动创建的信息 [!DNL Workfront] 用户来自 [!DNL Jira]，请参见 [配置 [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

记录项目在中的时间 [!DNL Jira] 并将它记录在 [!DNL Jira] 和 [!DNL Workfront]：

1. 登录 [!DNL Jira].
1. 转到 [!DNL Jira] 链接到的问题 [!DNL Workfront] 项目。
1. 展开 **[!UICONTROL 更多]** 菜单并单击 **[!UICONTROL 记录工作]**.

1. 在 **[!UICONTROL 逗留时间]** 字段，指定处理此问题所花费的时间。 您必须使用以下时间段指定时间：

   * [!UICONTROL 周] (w)
   * [!UICONTROL 天] (d)
   * [!UICONTROL 小时] (h)

1. 继续向时间条目添加信息，包括 **[!UICONTROL 工作描述]**，然后单击 **[!UICONTROL 日志]**.\
   时间将添加到 **[!UICONTROL 工作日志]** 选项卡 [!DNL Jira] 项目，以及 [!DNL Workfront] 链接到它的项目。\
   时间条目的工作描述将记录为中小时条目的注释 [!DNL Workfront].

### 记录开始时间 [!DNL Jira] 到 [!DNL Workfront] 项目

您可以只将时间记录到链接的 [!DNL Workfront] 项来自 [!DNL Jira] 未将此时间录制到的问题 [!DNL Jira] 问题。

1. 登录 [!DNL Jira].
1. 导航到 [!DNL Jira] 链接到的问题 [!DNL Workfront] 项目。

   此产品的 [!DNL Workfront] 项目应显示在以下位置： [!DNL Workfront] 问题的右侧面板。

1. 单击 **[!UICONTROL 记录时间]** 图标。

1. 指定金额 **[!UICONTROL 小时]** 和 **[!UICONTROL 分钟]** 您希望记录此问题。

1. 单击 **[!UICONTROL 记录时间]**.

   时间将添加到 [!DNL Workfront] 项目。

   此时间未添加到 [!UICONTROL 工作日志] 选项卡 [!DNL Jira] 问题。

## 来自链接的评论 [!DNL Jira] 问题 {#comment-from-a-linked-jira-issue}

当您对 [!DNL Jira] 项来自 [!DNL Workfront] 右侧面板位于 [!DNL Jira]，则该注释也会添加到 [!UICONTROL 更新] Workfront中链接项目的选项卡。

评论来源： [!DNL Jira] 到 [!DNL Workfront] 项目：

1. 登录 [!DNL Jira].
1. 导航到 [!DNL Jira] 链接到的问题 [!DNL Workfront] 项目。

   此产品的 [!DNL Workfront] 项目应显示在以下位置： [!DNL Workfront] 问题的右侧面板。

1. 单击 **[!UICONTROL 评论]** 图标 [!DNL Workfront] 面板或 **[!UICONTROL 评论]** 选项卡。

1. 开始键入评论，然后单击 **[!UICONTROL 发送]**.

   该注释将添加到以下内容：

   * 此 **[!DNL Workfront]** 选项卡 [!DNL Jira] 问题。
   * 此 **[!UICONTROL 评论]** 选项卡 [!DNL Jira] 问题。
   * 此 **[!UICONTROL 更新]** Workfront中链接项目的选项卡。
