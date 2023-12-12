---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 配置 [!DNL Adobe Workfront for Jira]
description: 您可以使用 [!DNL Adobe Workfront for Jira] 集成 [!DNL Jira] 和 [!DNL Workfront] 系统。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: 6d2494f1ccb2f9b222a953ed8bae922bd0f26389
workflow-type: tm+mt
source-wordcount: '2420'
ht-degree: 0%

---

# 配置 [!DNL Adobe Workfront for Jira]

您可以使用 [!DNL Adobe Workfront for Jira] 集成 [!DNL Jira] 和 [!DNL Workfront] 系统。

安装加载项后，您可以定义用于创建 [!DNL Jira] 出现以下情况时自动问题 [!DNL Workfront] 将创建工作项。 两个应用程序中的项目会相互链接，并且其中的一些信息会在两个系统中自动更新。

中的所有用户 [!DNL Workfront] 和 [!DNL Jira] 将受益于此集成。 他们只需要许可证就可以使用他们最常使用的系统，而不需要许可证就可以同时使用两个系统。

此加载项同时适用于 [!UICONTROL 服务器] 和 [!UICONTROL 按需] (或 [!UICONTROL 云])个版本 [!DNL Jira] 软件。

对于 [!DNL Jira] 版本 [!DNL Workfront for Jira] 当前支持，请参阅 [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) 在 [!DNL Atlassian Marketplace].

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL [!DNL Adobe Workfront] 计划]*</td> 
   <td><p>新建：任何</p>
       <p>或</p>
       <p>当前： [！UICONTROL Pro]或更高版本</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td><p>新文档： [！UICONTROL Standard] </p>
       <p>或</p> 
       <p>当前： [！UICONTROL计划] </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 访问</td> 
   <td> <p>系统管理员访问权限</p> <p>重要信息：我们建议您在中创建单独的系统管理员帐户 [!DNL Jira] 和 [!DNL Workfront] 以专门用于此集成，而不使用可能附加到用户的现有集成。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须是 [!DNL Workfront] 管理员。 有关的信息 [!DNL Workfront] 管理员，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理权限</a>.</p> <p>注意：如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 先决条件

在配置之前 [!DNL Workfront for Jira]，您必须：

* 安装 [!DNL Workfront for Jira].
有关安装的说明 [!DNL Workfront for Jira]，请参见 [安装 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## 配置 [!DNL Workfront for Jira]

通过配置 [!DNL Workfront for Jira]，您可以：

* 定义将创建的触发器 [!DNL Jira] 项目时间 [!DNL Workfront] 将创建项目。
* 指定哪些字段应在链接到的项目之间同步 [!DNL Jira] 和 [!DNL Workfront].

>[!NOTE]
>
>* 配置之后 [!DNL Workfront for Jira] 在您的 [!DNL Jira] 环境，全部 [!DNL Jira] 用户看到 [!DNL Workfront] 全部右面板 [!DNL Jira] 个项目。 面板包含有关可能链接到的项的信息 [!DNL Workfront] 或指定 [!DNL Workfront] 项链接到 [!DNL Jira] 个项目。
>* 使用时 [!DNL Jira Server] 安装时，只有与标识为Workfront集成触发器的项目关联的问题才会显示Workfront面板。 有关设置触发器的详细信息 [!DNL Workfront to Jira] 工作流，请参见 [配置触发器以自动链接以下项之间的项： [!DNL Jira] 和 [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

配置 [!DNL Workfront for Jira]：

1. 登录 [!DNL Jira] as a [!DNL Jira] 管理员。
1. 单击 **[!UICONTROL 设置]** 在主页中 [!DNL Jira] 菜单。
1. 单击 **[!UICONTROL 加载项]**，然后单击 **[!UICONTROL 管理加载项]**.

1. 展开 **[!DNL Workfront]** 加载项。
1. 单击 **[!UICONTROL 配置]**.
1. 按照提示登录 [!DNL Workfront].

   >[!NOTE]
   >
   >用户必须具有有效的 `apiKey` 在 [!UICONTROL Workfront] 创建成功的连接。

   您必须登录到 [!DNL Workfront] as a [!DNL Workfront] 管理员以继续配置。

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] 连接到 [!DNL Jira] 使用OAuth 2.0，大多数基于Web的集成使用这一标准对用户进行身份验证和授权。
   >* 当提示您输入域时， [!DNL Workfront] 帐户，使用以下格式键入它： *yourCompany&#39;sDomain.my.workfront.com*. 您公司的域通常是您公司的名称。
   >* 增强身份验证在 [!DNL Workfront] 管理员会为此集成启用它。

1. 在Jira中，选择 **[!UICONTROL 触发器]** 选项卡以配置自动创建 [!DNL Jira] 项作为新 [!DNL Workfront] 将创建项目。

   有关为Workfront设置触发器的更多信息，请 [!DNL Jira] 工作流，请参见 [配置触发器以自动链接以下项之间的项： [!DNL Jira] 和 [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. 选择 **[!UICONTROL 设置]** 选项卡，以配置链接之间的字段同步 [!DNL Jira] 和 [!DNL Workfront] 个项目。

   有关设置以下对象之间的字段同步的详细信息 [!DNL Jira] 和 [!DNL Workfront]，请参见 [配置字段同步，介于 [!DNL Jira] 和 [!DNL Workfront] 项目](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >定义触发器和两个应用程序之间的字段同步后， [!DNL Workfront] 可以创建任务或问题的用户可能会触发在中创建项目 [!DNL Jira]. 如果所创建项目的条件与中的触发器匹配，则用户可以创建项目 [!DNL Jira]，即使用户没有 [!DNL Jira] 许可证。 此外，任何 [!DNL Jira] 用户可以立即开始使用 [!DNL Jira] 项，并且其更新在中可见 [!DNL Workfront]，但没有一个 [!DNL Workfront] 许可证。 中的任何更新 [!DNL Workfront] 也可在 [!DNL Jira] 个项目。

1. （可选）选择 **[!UICONTROL 活动日志]** 选项卡，以查看集成期间可能发生的任何错误。

   欲知关于 [!UICONTROL 活动日志]，请参见 [查看 [!DNL Jira] [!UICONTROL 活动日志]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## 配置触发器以自动链接以下项之间的项： [!DNL Jira] 和 [!DNL Workfront]

作为 [!DNL Jira] 系统管理员定义的触发器可自动在中创建问题 [!DNL Jira] 当项目位于 [!DNL Workfront] 符合特定标准。

>[!NOTE]
>
>集成最多可能需要10分钟才能在中创建新问题 [!DNL Jira].

配置触发创建时，请考虑以下事项 [!DNL Jira] 项作为 [!DNL Workfront] 将创建以下项目：

* 集成是单向的：您只能触发在中创建的项目 [!DNL Workfront] 将在中自动创建 [!DNL Jira]. 您无法触发在中创建的项目 [!DNL Jira] 将在中自动创建 [!DNL Workfront].
* 您可以触发的触发器数量没有限制。
* 如果您在中创建的项目 [!DNL Workfront] 与多个触发器匹配，在中只创建一个项目 [!DNL Jira]. 项目创建于 [!DNL Jira] 根据第一个触发器(按照它们在 [!DNL Jira])。 所有其他触发器将被忽略。
* 中只有一个项目 [!DNL Workfront] 可以链接到Jira中的一个项目。 您永远无法链接一个 [!DNL Workfront] 项目到多个 [!DNL Jira] 问题，或一个 [!DNL Jira] 问题到多个 [!DNL Workfront] 个项目。

配置触发器以在中自动创建项目 [!DNL Jira]：

1. 登录 [!DNL Jira] 作为系统管理员。
1. 单击 **[!UICONTROL 设置]** 在主页中 [!DNL Jira] 菜单。
1. 单击 **[!UICONTROL 加载项]**，则 **[!UICONTROL 管理加载项]**.
1. 展开 **[!DNL Workfront]** 加载项。
1. 单击 **[!UICONTROL 配置]**.
1. 登录 [!DNL Workfront] 作为系统管理员。

   此 **[!UICONTROL 触发器]** 在Jira中，默认情况下会选中选项卡。

1. 单击 **[!UICONTROL 添加触发器]** 以添加新触发器。
1. 在 **[!UICONTROL Workfront团队/用户/角色]** 字段，指定 [!DNL Workfront] 团队、用户或工作角色，然后单击以将其在列表中显示时选定。

   >[!NOTE]
   >
   >同一团队、用户或角色不能有多个触发器。

   当有人创建任务或问题并将其分配给其中一个实体时，问题会在[！DNL]中自动创建 [!DNL Jira]]。

1. 在 **[!UICONTROL [!DNL Jira]项目]** 字段，开始键入 [!DNL Jira] 项目，然后单击以在列表中显示该项目时将其选中。

   当 [!DNL Jira] 创建的问题，并放置到您在此处选择的项目上。

1. 选择 **I[!UICONTROL 问题类型]** 从下拉菜单中。

   这表示在中创建的问题类型 [!DNL Jira] 当满足此触发器的条件时，根据您在中的特定项目设置 [!DNL Jira].

1. 单击&#x200B;**[!UICONTROL 保存]**。

   使用此配置，每次 [!DNL Workfront] 用户创建与指定触发器匹配的项目，在中创建新问题 [!DNL Jira].

## 配置字段同步，介于 [!DNL Jira] 和 [!DNL Workfront] 项目

作为 [!DNL Jira] 管理员，您可以定义哪些字段应当对链接到的项自动同步 [!DNL Workfront] 和吉拉。 某些字段可以从 [!DNL Workfront] 到 [!DNL Jira] 项目和其他项目从Jira同步到Workfront。

要定义应在两个应用程序之间链接的项目上自动同步的字段，请执行以下操作：

1. 登录 [!DNL Jira] 作为Jira管理员。
1. 单击 **[!UICONTROL 设置]** 在主页中 [!DNL Jira] 菜单。
1. 单击 **[!UICONTROL 加载项]**，则 **[!UICONTROL 管理加载项]**.
1. 展开 **[!DNL Workfront]** 加载项。
1. 单击 **[!UICONTROL 配置]**.
1. 登录 [!DNL Workfront] Workfront管理员。
1. 在Jira中，单击 **[!UICONTROL 设置]** 选项卡。
1. 在 **[!UICONTROL 从Workfront同步到Jira]** 部分，选择要更新的字段 [!DNL Jira] 在Workfront中更新它们时。

   1. 选择以下任何与字段同步的频率：

      <table style="table-layout:auto">
         <tr>
              <td>[！UICONTROL On Creation]</td>
              <td>您指定的字段将在链接的Workfront与之间同步 [!DNL Jira] 在Workfront中创建项目时的项目。</td>
          </tr>
          <tr>
              <td>[！UICONTROL Always]</td>
              <td>您指定的字段将在链接的Workfront与之间同步 [!DNL Jira] 在Workfront中更新字段时的项目。 </td>
          </tr>
          <tr>
              <td>[！UICONTROL从不]</td>
              <td>您指定的字段在链接之间从不同步 [!DNL Workfront] 和 [!DNL Jira] 个项目。 中没有任何提示 [!DNL Jira] 该字段更新于 [!DNL Workfront]. </td>
          </tr>
      </table>

   1. 选择以下任一选项以同步以下项的字段： [!DNL Workfront] 到 [!DNL Jira]：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[！UICONTROL名称]</td>
         <td><p>中任务或问题的名称 [!DNL Workfront] 将成为它所链接到的问题的名称 [!DNL Jira].</p><p>注意：在中创建新项目时 [!DNL Jira] 自动 [!DNL Workfront] 名称始终在 [!DNL Jira] 项，无论是否在此处启用此字段。 当 [!DNL Jira] 项目被手动链接到 [!DNL Workfront] 项目，此项目的名称 [!DNL Workfront] 仅项目更新 [!DNL Jira] 当您选择时 <strong>始终</strong> 同步此字段。 有关手动或自动链接项目的详细信息，请参阅 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">链接项目介于 [!DNL Adobe Workfront] 和 [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL描述]</td>
         <td>中任务或问题的描述 [!DNL Workfront] 成为它所链接到的问题的描述 [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">文档</td>
         <td><p>附加到中任务或问题的文档 [!DNL Workfront] 也附在Jira中与它有关的问题上。 新文档版本 [!DNL Workfront] 作为单独的文件添加到Jira并附加 <i>_v&lt;version number=""&gt;</i> 指示Workfront中的编号版本。 </p><p>例如，如果文档的名称 [!DNL Workfront] 是 <strong>主广告</strong>，然后在中添加一个新版本 [!DNL Workfront]，则会将新版本传输到 [!DNL Jira] 作为名称为的新文档 <strong>主Ad_v2</strong>.</p><p>重要提示： <p>同步文档时，请考虑以下事项：</p>
           <ul>
            <li><p>大于5MB的文档不会同步。 如果文档同步因文档太大而失败，则活动日志中会记录一个错误。 </p><p>有关活动日志的详细信息，请参阅 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">查看Jira活动日志</a>.</p></li>
            <li><p>链接到来自外部服务器的任务和问题的文档不会传输到 [!DNL Jira] 个项目。 仅直接在任务或问题中上传的文档 [!DNL Workfront] 已转移到中的链接问题 [!DNL Jira].</p></li>
            <li><p>要从文档创建验证，您必须在中生成验证 [!DNL Workfront]. </p><p>有关生成校样的更多信息，请参阅 <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">为现有文档创建验证 </a>在 <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">为文档创建验证</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL计划完成日期]</td>
         <td><p>中的任务或问题的[！UICONTROL规划完成日期] [!DNL Workfront] 将成为它所链接到的问题的[！UICONTROL截止日期] [!DNL Jira].</p><p>注意：确保显示 <strong>[！UICONTROL到期日期]</strong> 日期 [!DNL Jira] 问题，此值需要同步。</p></td>
        </tr>
       </tbody>
      </table>

1. 在 **[!UICONTROL 同步自 [!DNL Jira] 到[!DNL Workfront]]** 部分，选择要更新的字段 [!DNL Workfront] 当它们在中更新时 [!DNL Jira].

   1. 选择以下任何与字段同步的频率：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[！UICONTROL Always]</td>
         <td>您指定的字段始终在链接的字段之间同步 [!DNL Workfront] 和 [!DNL Jira] 项更新字段时 [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL从不]</td>
         <td><p>您指定的字段在链接之间从不同步 [!DNL Workfront] 和 [!DNL Jira] 个项目。 中没有任何提示 [!DNL Workfront] 该字段更新于 [!DNL Jira]. </p><p>注意：如果选择“从不”， [!DNL Workfront] 字段仍然可以从手动更新 [!DNL Jira] 在左侧 [!DNL Workfront] 面板 [!DNL Jira] 问题。 这些更新仅显示在 [!DNL Workfront] 中的项目 [!DNL Jira] 和 [!DNL Workfront] 并且不在 [!DNL Jira] 个项目。</p></td>
        </tr>
       </tbody>
      </table>

   1. 选择以同步以下任意字段，从 [!DNL Jira] 到 [!DNL Workfront]：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[！UICONTROL状态]</td>
         <td>中问题的[！UICONTROL状态] [!DNL Jira] 将成为它所链接到的任务或问题的[！UICONTROL状态] [!DNL Workfront].<br>有关详情 [!DNL Workfront] 状态，请参见 <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">创建或编辑状态</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL被分派人]</td>
         <td><p>中问题的[！UICONTROL被分派人] [!DNL Jira] 成为与其链接的任务或问题的[！UICONTROL被分配人] [!DNL Workfront].</p><p>重要提示：在中分配项目时 [!DNL Jira] 发送给没有 [!DNL Workfront] 帐户，则集成将在中创建一个新的活动用户 [!DNL Workfront] 仅当 <strong>在中自动创建用户 [!DNL Workfront] 如果 [!DNL Jira] 用户没有 [!DNL Workfront] 帐户</strong> 设置为 <strong>[！UICONTROL Always]</strong>. 此用户未占用 [!DNL Workfront] 许可证。 可将活动用户分配到中的工作项 [!DNL Workfront]，但不能包含在更新中。 </p></td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL附件]</td>
         <td>中的问题附件 [!DNL Jira] 也会附加到与其链接的任务或问题 [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL Comments]</td>
         <td><p>评论 [!DNL Jira] 问题也会发布在链接上 [!DNL Workfront] [！UICONTROL更新]区域中的项。 相反，在[！UICONTROL更新]区域张贴的注释用于 [!DNL Workfront] 任务或问题同步到 [!DNL Jira]的链接问题的本机注释流。 </p><p>此参数设置为 <strong>[！UICONTROL Always]</strong> 默认情况下。 如果您选择 <strong>[！UICONTROL从不]</strong> 在此，您仍然可以在以下任一位置对链接的项目手动发布评论： [!DNL Workfront] 或 [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. 在 **[!UICONTROL 其他]** 部分，选择应在链接项之间更新的其他字段。

   1. 选择一个选项以确定您指定的字段是否 **[!UICONTROL 始终]** 或 **[!UICONTROL 从不]** 更新位置 [!DNL Jira] 或 [!DNL Workfront] 修改它们时。

   1. 从以下字段和更新中进行选择：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[！UICONTROL副本 [!DNL Workfront] 中的右侧面板中的自定义数据 [!DNL Jira]]</td>
         <td><p>显示 [!DNL Workfront] 中项目的自定义数据 [!DNL Workfront] 右侧面板。</p><p>注意：自定义表单部分显示在 [!DNL Workfront] 右侧面板，其访问级别为 [!DNL Workfront] 系统管理员。</p></td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL副本 [!DNL Workfront] 中的右侧面板中的优先级 [!DNL Jira]]</td>
         <td>显示 [!DNL Workfront] 中项目的优先级 [!DNL Workfront] 右侧面板。</td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL在 [!DNL Workfront] 有关到期日期更改的“更新”选项卡 [!DNL Jira]]</td>
         <td>在的[！UICONTROL Update]选项卡中添加注释 [!DNL Workfront] [！UICONTROL到期日期]在链接中更改时的项 [!DNL Jira] 项目。</td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL在中自动创建用户 [!DNL Workfront] 如果 [!DNL Jira] 用户没有 [!DNL Workfront] 帐户]</td>
         <td><p>存在以下情况：</p>
          <ul>
           <li>当您选择时 <strong>[！UICONTROL Always]</strong>Workfront ，则可启用该集成，以便在每次 [!DNL Jira] 用户没有 [!DNL Workfront] 帐户对链接执行以下操作 [!DNL Jira] 问题：
            <ul>
             <li>已分配给 [!DNL Jira] 问题</li>
             <li><p>将时间记录到 [!DNL Jira] 问题</p><p>此新用户未占用 [!DNL Workfront] 许可证。 默认设置为“始终”。 在中通过这种方式创建的用户 [!DNL Workfront] 已将“[！UICONTROL Jira]”添加到其名称中。</p></li>
            </ul></li>
           <li>当您选择时 <strong>[！UICONTROL从不]</strong>，会发生以下情况：
            <ul>
             <li>您看不到任何 [!DNL Jira] 分配： [!DNL Workfront] 个项目。 在这种情况下，仅分配在 [!DNL Workfront] 显示在 [!DNL Workfront] 个项目。</li>
             <li>登录到链接的时间 [!DNL Jira] 由没有 [!DNL Workfront] 帐户不会自动转移到链接的 [!DNL Workfront] 项目。 您仍然可以在 [!DNL Workfront] 项 [!DNL Jira] 问题。</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. 单击&#x200B;**[!UICONTROL 保存]**。

   现在，每次用户更新此配置中指定的任何字段时， [!DNL Jira] 或 [!DNL Workfront]，则其他应用程序中的链接项目也会更新。

## 故障排除

### 无法在中创建项目 [!DNL Jira] 因为触发器字段标记为“[!UICONTROL 找不到]&quot;

#### 问题

当出现错误时 [!DNL Workfront for Jira] 应用程序， [!DNL Workfront] 禁用触发器以防止出现进一步的复杂情况。 禁用这些触发器后，它们显示为“[!UICONTROL 找不到]“

#### 解决方案

找到禁用触发器的错误。 您可以在 [!DNL Workfront for Jira] [!UICONTROL 活动日志].

导致此行为的最常见原因是错误“[!UICONTROL 无法设置字段“duedate”。 不在相应的屏幕上，或未知。]&quot;

此错误表示您正在尝试同步&#39;&#39;[!UICONTROL 计划完成日期]”从 [!DNL Workfront] 到 [!DNL Jira]. 为此，您必须确保 [!DNL Jira] 对象具有名为“”的字段[!UICONTROL 到期日期]“ 如果他们没有这个领域， [!DNL Workfront] 无法从同步计划完成日期 [!DNL Workfront] 并禁用您的触发器。

要解决此错误，请尝试以下操作之一：

* 询问您的 [!DNL Jira] 管理员更新受影响的 [!DNL Jira] 对象以确保它们具有到期日期字段。
* 禁用同步 [!DNL Workfront]的Workfront中的计划完成日期 [!UICONTROL 设置] 页面。
