---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 配置 [!DNL Adobe Workfront for Jira]
description: 您可以使用 [!DNL Adobe Workfront for Jira] 集成 [!DNL Jira] 和 [!DNL Workfront] 系统。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '2400'
ht-degree: 0%

---

# 配置 [!DNL Adobe Workfront for Jira]

您可以使用 [!DNL Adobe Workfront for Jira] 集成 [!DNL Jira] 和 [!DNL Workfront] 系统。

安装加载项后，您可以定义创建 [!DNL Jira] 在 [!DNL Workfront] 将创建工作项。 两个应用程序中的项目都会链接起来，它们的某些信息会在两个系统中自动更新。

中的所有用户 [!DNL Workfront] 和 [!DNL Jira] 可以从此集成中受益。 他们只需要获得最常工作的系统的许可证，而不需要两个系统的许可证。

此加载项适用于 [!UICONTROL 服务器] 和 [!UICONTROL 按需] (或 [!UICONTROL 云])版本 [!DNL Jira] 软件。

要获取 [!DNL Jira] 版本 [!DNL Workfront for Jira] 当前支持，请参阅 [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) 在 [!DNL Atlassian Marketplace].

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] 计划]</a>*</td> 
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

在配置之前 [!DNL Workfront for Jira]，您必须

* 安装 [!DNL Workfront for Jira]\
   有关安装的说明 [!DNL Workfront for Jira]，请参阅 [安装 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## 配置 [!DNL Workfront for Jira]

通过配置 [!DNL Workfront for Jira] 您可以：

* 定义将创建 [!DNL Jira] 项目 [!DNL Workfront] 将创建项目。
* 指定应在链接于 [!DNL Jira] 和 [!DNL Workfront].

>[!NOTE]
>
>* 在您配置 [!DNL Workfront for Jira] 在 [!DNL Jira] 环境，全部 [!DNL Jira] 用户会看到 [!DNL Workfront] 全部为右面板 [!DNL Jira] 项目。 该面板包含有关可能从 [!DNL Workfront] 或指定否 [!DNL Workfront] 项目链接到 [!DNL Jira] 项目。
>* 使用 [!DNL Jira Server] 安装时，只有与被标识为Workfront集成触发器的项目相关的问题才会显示Workfront面板。 有关为 [!DNL Workfront to Jira] 工作流，请参阅 [配置触发器，以便在 [!DNL Jira] 和 [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>




配置 [!DNL Workfront for Jira]:

1. 登录 [!DNL Jira] as a [!DNL Jira] 管理员。
1. 单击 **[!UICONTROL 设置]** 在主 [!DNL Jira] 菜单。
1. 单击 **[!UICONTROL 附加组件]**，然后单击 **[!UICONTROL 管理附加组件]**.

1. 展开 **[!DNL Workfront]** 附加组件。
1. 单击 **[!UICONTROL 配置]**.
1. 按照提示登录 [!DNL Workfront].

   >[!NOTE]
   >
   >[!UICONTROL Workfront] 连接到 [!DNL Jira] 使用OAuth 2.0，这是大多数基于Web的集成用于用户身份验证和授权的标准。

   您必须登录 [!DNL Workfront] as a [!DNL Workfront] 管理员以继续配置。

   >[!NOTE]
   >
   >* 提示您输入的域时 [!DNL Workfront] 帐户，请使用以下格式键入： *yourCompany&#39;sDomain.my.workfront.com*. 您公司的域通常是您公司的名称。
   >* 增强的身份验证在 [!DNL Workfront] 管理员为此集成启用了此功能。



1. 选择 **[!UICONTROL 触发器]** 选项卡来配置自动创建 [!DNL Jira] 项目作为新项目 [!DNL Workfront] 将创建项目。

   有关为Workfront设置触发器的更多信息，请参阅 [!DNL Jira] 工作流，请参阅 [配置触发器，以便在 [!DNL Jira] 和 [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. 选择 **[!UICONTROL 设置]** 选项卡，用于配置链接的字段之间的同步 [!DNL Jira] 和 [!DNL Workfront] 项目。

   有关设置字段同步的详细信息，请参阅 [!DNL Jira] 和 [!DNL Workfront]，请参阅 [在之间配置字段同步 [!DNL Jira] 和 [!DNL Workfront] 项目](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >在定义触发器并在两个应用程序之间同步字段后，任何 [!DNL Workfront] 能够创建任务或问题的用户可能会在 [!DNL Jira]. 如果用户所创建项目上的标准与 [!DNL Jira]，即使用户没有 [!DNL Jira] 许可证。 此外， [!DNL Jira] 用户可以立即开始工作 [!DNL Jira] 项目，且其更新显示在 [!DNL Workfront]，而没有 [!DNL Workfront] 许可证。 中的任何更新 [!DNL Workfront] 在 [!DNL Jira] 项目。

1. （可选）选择 **[!UICONTROL 活动日志]** 选项卡，以查看在集成过程中可能发生的任何错误。

   有关 [!UICONTROL 活动日志]，请参阅 [查看 [!DNL Jira] [!UICONTROL 活动日志]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## 配置触发器，以便在 [!DNL Jira] 和 [!DNL Workfront]

作为 [!DNL Jira] 系统管理员，您可以定义触发器，以在 [!DNL Jira] 在 [!DNL Workfront] 符合某些标准。

>[!NOTE]
>
>集成可能最多需要10分钟才能在 [!DNL Jira].

配置触发创建时，请考虑以下事项 [!DNL Jira] 项目 [!DNL Workfront] 项目已创建：

* 该集成是单向的：您只能触发在中创建的项目 [!DNL Workfront] ，以在 [!DNL Jira]. 您无法触发在中创建的项目 [!DNL Jira] 自动创建 [!DNL Workfront].
* 您可以拥有的触发器数量没有限制。
* 如果您在中创建的项目 [!DNL Workfront] 与多个触发器匹配，则只会在 [!DNL Jira]. 项目在中创建 [!DNL Jira] 根据第一个触发器(按照 [!DNL Jira])。 所有其他触发器都将被忽略。
* 中只有一个项目 [!DNL Workfront] 可以链接到吉拉的一个项目。 您永远无法链接一个 [!DNL Workfront] 项目至多个 [!DNL Jira] 问题或一个 [!DNL Jira] 多个问题 [!DNL Workfront] 项目。

要配置触发器以在 [!DNL Jira]:

1. 登录 [!DNL Jira] 作为系统管理员。
1. 单击 **[!UICONTROL 设置]** 在主 [!DNL Jira] 菜单。
1. 单击 **[!UICONTROL 附加组件]**，则 **[!UICONTROL 管理附加组件]**.

1. 展开 **[!DNL Workfront]** 附加组件。
1. 单击 **[!UICONTROL 配置]**.
1. 登录到 [!DNL Workfront] 作为系统管理员。

   的 **[!UICONTROL 触发器]** 选项卡。

1. 单击 **[!UICONTROL 添加触发器]** 以添加新触发器。
1. 在 **[!UICONTROL Workfront团队/用户/角色]** 字段，指定 [!DNL Workfront] 团队、用户或作业角色，然后单击以在列表中显示时将其选中。

   >[!NOTE]
   >
   >您不能有同一团队、用户或角色的多个触发器。

   当某人创建任务或问题并将其分配给其中一个实体时，系统会在[!DNL中自动创建问题 [!DNL Jira]]。

1. 在 **[!UICONTROL [!DNL Jira]项目]** 字段，开始键入 [!DNL Jira] 项目，然后单击以在列表中显示时将其选中。

   当 [!DNL Jira] 问题时，该问题会放置在您在此处指定的项目上。

1. 选择 **我[!UICONTROL ssue类型]** 下拉菜单中。

   这表示在中创建的问题类型 [!DNL Jira] 当满足此触发器的条件时，请根据 [!DNL Jira].

1. 单击&#x200B;**[!UICONTROL 保存]**。

   通过此配置，每次 [!DNL Workfront] 用户创建与指定触发器匹配的项目时，会在 [!DNL Jira].

## 在之间配置字段同步 [!DNL Jira] 和 [!DNL Workfront] 项目

作为 [!DNL Jira] 管理员，您可以定义在链接的项目上自动同步的字段 [!DNL Workfront] 和吉拉。 某些字段可以从 [!DNL Workfront] 到 [!DNL Jira] 项目，以及从Jira同步到Workfront的其他项目。

要定义在两个应用程序之间链接的项目上自动同步哪些字段，请执行以下操作：

1. 登录 [!DNL Jira] Jira管理员。
1. 单击 **[!UICONTROL 设置]** 在主 [!DNL Jira] 菜单。
1. 单击 **[!UICONTROL 附加组件]**，则 **[!UICONTROL 管理附加组件]**.

1. 展开 **[!DNL Workfront]** 附加组件。
1. 单击 **[!UICONTROL 配置]**.
1. 登录到 [!DNL Workfront] 作为Workfront管理员。
1. 单击 **[!UICONTROL 设置]** 选项卡。

1. 在 **[!UICONTROL 从吉拉同步到Workfront]** ，选择要更新的字段 [!DNL Jira] 在Workfront中更新时。

   1. 选择与字段同步的以下任意频率：

      <table style="table-layout:auto">
         <tr>
              <td>[！创建时UICONTROL]</td>
              <td>您指定的字段将在链接的Workfront和 [!DNL Jira] 项目。</td>
          </tr>
          <tr>
              <td>[!UICONTROL Always]</td>
              <td>您指定的字段将在链接的Workfront和 [!DNL Jira] 在Workfront中更新字段时显示的项目。 </td>
          </tr>
          <tr>
              <td>[!UICONTROL Never]</td>
              <td>您指定的字段永远不会在链接的 [!DNL Workfront] 和 [!DNL Jira] 项目。 中未显示任何指示 [!DNL Jira] 字段在 [!DNL Workfront]. </td>
          </tr>
      </table>

   1. 选择以同步 [!DNL Workfront] to [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL名称]</td>
         <td><p>任务或问题的名称 [!DNL Workfront] 将成为链接到的问题的名称 [!DNL Jira].</p><p>注意：在中创建新项目时 [!DNL Jira] 自动， [!DNL Workfront] 名称始终在 [!DNL Jira] 项目，无论此处是否启用了此字段。 当 [!DNL Jira] 项目手动链接到 [!DNL Workfront] 项目，名称 [!DNL Workfront] 仅更新项目 [!DNL Jira] 当您选择 <strong>始终</strong> 同步此字段。 有关手动或自动链接项目的更多信息，请参阅 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">链接项目之间 [!DNL Adobe Workfront] 和 [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL描述]</td>
         <td>任务或问题的描述 [!DNL Workfront] 将成为其链接到的问题的描述 [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">文档</td>
         <td><p>附加到任务或 [!DNL Workfront] 也附加到在吉拉链接到的问题。 的新文档版本 [!DNL Workfront] 将作为单独的文档添加到Jira，并在其后附加 <i>_v&lt;version number=""&gt;</i> 以在Workfront中指示编号版本。 </p><p>例如，如果 [!DNL Workfront] is <strong>主广告</strong>，然后在 [!DNL Workfront]，则新版本将转移到 [!DNL Jira] 作为名为的新文档 <strong>主Ad_v2</strong>.</p><p>重要的: <p>同步文档时请考虑以下事项：</p>
           <ul>
            <li><p>大于5MB的文档不同步。 如果文档由于文档过大而同步失败，则会在活动日志中记录错误。 </p><p>有关活动日志的更多信息，请参阅 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">查看Jira活动日志</a>.</p></li>
            <li><p>与来自外部服务器的任务和问题链接的文档不会传输到 [!DNL Jira] 项目。 仅上传了任务或中问题的文档 [!DNL Workfront] 转换到 [!DNL Jira].</p></li>
            <li><p>要从文档创建校样，必须在 [!DNL Workfront]. </p><p>有关生成校样的更多信息，请参阅 <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create" class="MCXref xref">为现有文档创建校样 </a>in <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">为文档创建校样</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL计划完成日期]</td>
         <td><p>任务或中问题的[!UICONTROL计划完成日期] [!DNL Workfront] 将变为链接到的问题的[!UICONTROL到期日] [!DNL Jira].</p><p>注意：确保显示 <strong>[!UICONTROL到期日期]</strong> on [!DNL Jira] 问题，以便此值进行同步。</p></td>
        </tr>
       </tbody>
      </table>

1. 在 **[!UICONTROL 同步自 [!DNL Jira] to[!DNL Workfront]]** ，选择要更新的字段 [!DNL Workfront] 在 [!DNL Jira].

   1. 选择与字段同步的以下任意频率：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Always]</td>
         <td>您指定的字段始终会在链接的 [!DNL Workfront] 和 [!DNL Jira] 更新字段时显示的项目 [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Never]</td>
         <td><p>您指定的字段永远不会在链接的 [!DNL Workfront] 和 [!DNL Jira] 项目。 中未显示任何指示 [!DNL Workfront] 字段在 [!DNL Jira]. </p><p>注意：选择从不时， [!DNL Workfront] 字段仍可从 [!DNL Jira] 在左侧 [!DNL Workfront] 面板 [!DNL Jira] 问题。 这些更新仅在 [!DNL Workfront] 项目 [!DNL Jira] 和 [!DNL Workfront] 不打开 [!DNL Jira] 项目。</p></td>
        </tr>
       </tbody>
      </table>

   1. 选择以同步 [!DNL Jira] to [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL状态]</td>
         <td>中问题的[!UICONTROL状态] [!DNL Jira] 将变为链接到的任务或问题的[!UICONTROL状态] [!DNL Workfront].<br>有关 [!DNL Workfront] 状态，请参阅 <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">创建或编辑状态</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Assignee]</td>
         <td><p>在 [!DNL Jira] 将变为链接到的任务或问题的[!UICONTROL Assignee] [!DNL Workfront].</p><p>重要信息：在 [!DNL Jira] 向没有 [!DNL Workfront] 帐户，则集成会在 [!DNL Workfront] 只有在 <strong>在中自动创建用户 [!DNL Workfront] 如果 [!DNL Jira] 用户没有 [!DNL Workfront] 帐户</strong> 设置为 <strong>[!UICONTROL Always]</strong>. 此用户不占用 [!DNL Workfront] 许可证。 可以将活动用户分配到 [!DNL Workfront]，但不能包含在更新中。 </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL附件]</td>
         <td>中问题的附件 [!DNL Jira] 也会附加到链接到的任务或问题中 [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL注释]</td>
         <td><p>对 [!DNL Jira] 问题也会发布在链接的 [!DNL Workfront] 项目。 相反，在[!UICONTROL更新]区域发布的 [!DNL Workfront] 任务或问题同步到 [!DNL Jira]链接问题的本机注释流。 </p><p>此参数设置为 <strong>[!UICONTROL Always]</strong> 默认情况下。 如果您选择 <strong>[!UICONTROL Never]</strong> 在此，您仍然可以在 [!DNL Workfront] 或 [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. 在 **[!UICONTROL 其他]** 部分，选择链接项目之间应更新的其他字段。

   1. 选择一个选项以确定您指定的字段 **[!UICONTROL 始终]** 或 **[!UICONTROL 从不]** 更新 [!DNL Jira] 或 [!DNL Workfront] 修改时。

   1. 从以下字段和更新中进行选择：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] 中右侧面板中的自定义数据 [!DNL Jira]]</td>
         <td><p>显示 [!DNL Workfront] 中某个项目的自定义数据 [!DNL Workfront] 右侧面板。</p><p>注意：自定义表单部分显示在 [!DNL Workfront] 具有 [!DNL Workfront] 系统管理员。</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] 在的右侧面板中显示优先级 [!DNL Jira]]</td>
         <td>显示 [!DNL Workfront] 中项目的优先级 [!DNL Workfront] 右侧面板。</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL在 [!DNL Workfront] 关于中到期日期更改的“更新”选项卡 [!DNL Jira]]</td>
         <td>在 [!DNL Workfront] 项目，因为[!UICONTROL到期日期]在链接的 [!DNL Jira] 项目。</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL在中自动创建用户 [!DNL Workfront] 如果 [!DNL Jira] 用户没有 [!DNL Workfront] account]</td>
         <td><p>存在以下情形：</p>
          <ul>
           <li>选择 <strong>[!UICONTROL Always]</strong> 您可以启用集成，以在每次 [!DNL Jira] 没有用户 [!DNL Workfront] 帐户对链接的 [!DNL Jira] 问题：
            <ul>
             <li>已分配给 [!DNL Jira] 问题</li>
             <li><p>将时间记录到 [!DNL Jira] 问题</p><p>此新用户不会占用 [!DNL Workfront] 许可证。 默认设置为“始终”。 用户在中以这种方式创建 [!DNL Workfront] 在其名称中添加了“[!UICONTROL Jira]”。</p></li>
            </ul></li>
           <li>选择 <strong>[!UICONTROL Never]</strong>，则会发生以下情况：
            <ul>
             <li>您看不到任何 [!DNL Jira] 分配 [!DNL Workfront] 项目。 在这种情况下，仅在 [!DNL Workfront] 在 [!DNL Workfront] 项目。</li>
             <li>登录链接的时间 [!DNL Jira] 用户在 [!DNL Workfront] 帐户不会自动转移到链接的帐户 [!DNL Workfront] 项目。 您仍可以在 [!DNL Workfront] 项目 [!DNL Jira] 问题。</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. 单击&#x200B;**[!UICONTROL 保存]**。

   现在，每当用户在任一项中的某个项目上更新此配置中指定的任何字段时 [!DNL Jira] 或 [!DNL Workfront]，则另一个应用程序中的链接项目也会更新。

## 疑难解答

### 无法在中创建项目 [!DNL Jira] 因为标记为“[!UICONTROL 找不到]&quot;

#### 问题

当 [!DNL Workfront for Jira] 应用程序， [!DNL Workfront] 禁用触发器以防止进一步并发症。 禁用这些触发器后，它们将显示为“[!UICONTROL 找不到]&quot;

#### 解决方案

找到禁用触发器的错误。 您可以在 [!DNL Workfront for Jira] &quot;[!UICONTROL 活动日志]&quot;

此行为的最常见原因是错误“[!UICONTROL 无法设置字段“duedate”。 它不在相应的屏幕上，或未知。]&quot;

此错误表示您尝试同步“[!UICONTROL 计划完成日期]从 [!DNL Workfront] to [!DNL Jira]. 为此，您必须确保 [!DNL Jira] 对象具有名为“[!UICONTROL 到期日期]&quot; 如果他们没有此字段， [!DNL Workfront] 无法同步计划的完成日期(从 [!DNL Workfront] 和禁用触发器。

要解决此错误，请尝试以下操作之一：

* 询问您的 [!DNL Jira] 管理员以更新受影响的 [!DNL Jira] 对象，以确保它们具有到期日期字段。
* 禁用的同步 [!DNL Workfront]的计划完成日期(Workfront)[!UICONTROL 设置]“”页
