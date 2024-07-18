---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Slack模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动使用Slack的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: ba5bad6a-3cb3-4024-82f7-d38ee9a8e0b5
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1744'
ht-degree: 0%

---

# [!DNL Slack]模块

在[!DNL Adobe Workfront Fusion]方案中，您可以自动使用[!DNL Slack]的工作流，并将其连接到多个第三方应用程序和服务。

如果需要有关创建方案的说明，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中创建方案。

有关模块的信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模块。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td>
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 先决条件

要使用[!DNL Slack]模块，您必须具有[!DNL Slack]帐户。

## [!DNL Slack]模块及其字段

配置[!DNL Slack]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL Slack]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)

* [消息](#messages)
* [文件](#files)
* [渠道](#channels)
* [反应](#reactions)
* [星级](#stars)
* [已保存的项目](#saved-items)
* [固定](#pins)
* [用户](#users)
* [提醒](#reminders)
* [活动](#events)
* [帐户信息](#profile)
* [其他](#other)

### 消息

+++**[!UICONTROL 观看公共渠道消息]**

在将新消息添加到公共渠道时，此触发器模块将启动场景。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Slack]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Channel] </td> 
   <td> <p>选择要监视新消息的公共渠道。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>设置在一个执行周期内将返回的最大邮件数[!DNL Workfront Fusion]。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL 观看私人频道留言]**

此触发器模块在将新消息添加到专用渠道（组）后启动场景。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Slack]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Channel] </td> 
   <td> <p>选择要监视新消息的专用渠道。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>设置在一个执行周期内将返回的最大邮件数[!DNL Workfront Fusion]。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

<!--

+++ **[!UICONTROL Watch Direct Messages]**

This trigger module starts the scenario when a new message is added to a direct message.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel] </td> 
   <td> <p>Select the direct message conversation you want to watch for new messages.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Set the maximum number of messages [!DNL Workfront Fusion] will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Watch Multiparty Direct Messages]**

This trigger module starts the scenario when a new message is added to a multiparty direct message channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel] </td> 
   <td> <p>Select the direct message conversation you want to watch for new messages.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Set the maximum number of messages [!DNL Workfront Fusion] will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Search for Message]**

This search module returns messages matching a search query.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td> <p>Enter the query that you want to search by. </p> <p>For information on creating formulas from the mapping panel, see <a href="../../workfront-fusion/functions/map-using-functions.md" class="MCXref xref">Map items using functions in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Set the maximum number of messages [!DNL Workfront Fusion] will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

-->

+++ **[!UICONTROL 获取私人频道消息]**

此操作模块从所选渠道检索消息的详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Slack]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL渠道ID]</p> </td> 
   <td> <p>输入（映射）渠道ID。</p> <p>注意：可以使用[！UICONTROL List Channels]模块检索渠道ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL消息ID（时间戳）]</p> </td> 
   <td> <p> 输入或映射要检索相关信息的消息的消息时间戳。</p> <p>注意：可以使用其他模块（例如[！UICONTROL Watch Public Channel]模块）检索时间戳。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 获取公共频道消息]**

此操作模块从指定的公共渠道返回具有给定ID的消息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Slack]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL渠道ID]</p> </td> 
   <td> <p>输入或映射渠道ID。</p> <p>注意：可以使用[！UICONTROL List Channels]模块检索渠道ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL消息ID（时间戳）]</td> 
   <td> <p> 输入或映射要检索相关信息的消息的消息时间戳。</p> <p>注意：可以使用其他模块（例如[！UICONTROL Watch Public Channel]模块）检索时间戳。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

<!--

+++ **[!UICONTROL List replies]**

This action module retrieves a thread of messages posted to a conversation.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that contains the message that you want to retrieve replies for, then select the channel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parent message ID (Time stamp)]</td> 
   <td> <p> Enter or map the message time stamp of the message you want to retrieve replies for.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Public Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of replies you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

-->

+++ **[!UICONTROL 创建消息]**

此操作模块将创建新消息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Slack]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL输入渠道ID或名称]</p> </td> 
   <td> <p>选择您希望如何选择要创建消息的渠道。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>在<strong>[！UICONTROL渠道ID或名称]</strong>字段中，输入或映射要发布消息的渠道的渠道ID或名称。</p> <p>注意：可以使用[！UICONTROL List Channels]模块检索渠道ID。</p> </li> 
     <li> <p><strong>[！UICONTROL从列表中选择]</strong> </p> <p>选择渠道类型，然后选择渠道。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Text]</p> </td> 
   <td> <p>输入要创建的消息的文本内容。</p> <p>注意：有关文本格式化的详细信息，请参阅[!DNL Slack]文档中的<a href="https://api.slack.com/reference/surfaces/formatting">设置应用程序表面文本的格式</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL块]</td> 
   <td>块是可重用组件，可用于自定义和组织消息。 有关块的详细信息，请参阅[!DNL Slack]文档中的<a href="https://api.slack.com/block-kit">块套件</a>。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL线程消息ID（时间戳）]</td> 
   <td>如果新消息是回复，请输入要回复的消息的时间戳。 不要输入已经是回复的消息的时间戳。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL回复广播]</td> 
   <td> <p>如果同时满足以下两个条件，请选择<strong>[！UICONTROL是]</strong>：</p> 
    <ul> 
     <li> <p>新消息是对另一消息的回复</p> </li> 
     <li> <p>您希望频道中的所有人都能够看到新消息</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL链接名称]</p> </td> 
   <td> <p>启用此选项以允许名称和渠道使用<code>@username</code>或<code>#channel</code>格式。 </p> <p>有关详细信息，请参阅[!DNL Slack]文档中的<a href="https://api.slack.com/docs/formatting">设置应用程序表面文本格式</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL解析消息文本]</p> </td> 
   <td> <p>启用此选项以允许自动分析。 </p> <p>有关详细信息，请参阅[!DNL Slack]文档中的<a href="https://api.slack.com/docs/formatting">设置应用程序表面文本格式</a>。</p> <p>注意：如果您在原始消息中使用了[！UICONTROL链接名称]或[！UICONTROL解析消息文本]选项，则您还应在运行[！UICONTROL更新消息]模块时指定这些选项。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL使用Markdown]</p> </td> 
   <td> <p>启用此选项以允许[!DNL Slack]在文本中使用Markdown。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL主要展开基于文本的内容]</p> </td> 
   <td> <p>启用此选项以允许展开主要基于文本的内容。 </p> <p>有关[!DNL Slack]中展开的详细信息，请参阅[!DNL Slack]文档中的<a href="https://api.slack.com/reference/messaging/link-unfurling">消息中的展开链接</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL展开媒体内容]</p> </td> 
   <td> <p>启用此选项以允许展开媒体内容。 </p> <p>有关[!DNL Slack]中展开的详细信息，请参阅[!DNL Slack]文档中的<a href="https://api.slack.com/reference/messaging/link-unfurling">消息中的展开链接</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 更新消息]**

此操作模块允许您编辑现有消息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Slack]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL输入渠道ID或名称]</p> </td> 
   <td> <p>选择您希望如何选择要发送的消息。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>在<strong>[！UICONTROL渠道ID或名称]</strong>字段中，输入或映射包含该消息的渠道ID，然后输入该消息的<strong>[！UICONTROL时间戳（消息ID）]</strong>。.</p> <p>注意：可以使用[！UICONTROL List Channels]模块检索渠道ID。</p> </li> 
     <li> <p><strong>[！UICONTROL从列表中选择]</strong> </p> <p>选择渠道类型，然后选择渠道，最后选择消息。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Text]</p> </td> 
   <td> <p>输入要更新的消息的新文本内容。</p> <p>有关详细信息，请参阅[!DNL Slack]文档中的<a href="https://api.slack.com/docs/formatting">设置应用程序表面文本格式</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL块]</td> 
   <td>块是可重用组件，可用于自定义和组织消息。 有关块的详细信息，请参阅[!DNL Slack]文档中的<a href="https://api.slack.com/block-kit">块套件</a>。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL链接名称]</p> </td> 
   <td> <p>启用此选项以允许名称和渠道使用<code>@username</code>或<code>#channel</code>格式。 </p> <p>有关详细信息，请参阅[!DNL Slack]文档中的<a href="https://api.slack.com/docs/formatting">设置应用程序表面文本格式</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL解析消息文本]</p> </td> 
   <td> <p>启用此选项以允许自动分析。 </p> <p> 有关详细信息，请参阅[!DNL Slack]文档中的<a href="https://api.slack.com/docs/formatting">设置应用程序表面文本格式</a>。</p> <p>注意：如果您在原始消息中使用了[！UICONTROL链接名称]或[！UICONTROL解析消息文本]选项，则您还应在运行更新消息模块时指定这些选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 删除邮件]**

此操作模块删除指定的消息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Slack]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL渠道ID]</p> </td> 
   <td> <p>输入或映射渠道ID。</p> <p>注意：可以使用[！UICONTROL List Channels]模块检索渠道ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL消息ID]</td> 
   <td> <p> 输入或映射要删除的消息的时间戳。</p> <p>注意：可使用其他模块（如Watch Private Channel模块）检索时间戳。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

<!--

### Files 

+++ **[!UICONTROL Watch Files]**

This trigger module starts a scenario when a new file is added.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Select the type of file that you want the module to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td> <p>Select the type of channel you want to watch for files, then select the channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Enter or map the maximum number of files you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL List Files]**

This action module returns a list of files based on the specified filter.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type] </td> 
   <td> <p>Select the type(s) of files you want to retrieve.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel type]</p> </td> 
   <td> <p>Select the type of channel representing the channel that you want to list files from, then select the channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Created by]</td> 
   <td> <p>Select a user to return only files created by that user.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date from]</td> 
   <td>Enter the earliest date that you want to return files from. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date to]</td> 
   <td>Enter the latest date that you want to return files from. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Enter or map the maximum number of files you want the module to return during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Get a File]**

This action module returns details about the specified file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td> <p>Enter or map the ID of the file that you want to retrieve. </p> <p>Note: The file ID can be retrieved using another module, such as the [!DNL Watch Files] Module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Download a File]**

This action module downloads a file from a URL. It must follow the [!UICONTROL Slack] >[!UICONTROL Get a File] module in a scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL private download]</td> 
   <td> <p>Map the <b>[!UICONTROL URL Private download]</b> value from the [!DNL Slack] >[!UICONTROL Get a File] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Upload a File]**

This action module creates or uploads a file to [!DNL Slack]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channels]</td> 
   <td> <p>For each channel you want to upload the file to, click <b>[!UICONTROL Add item]</b>, then select the channel type and channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>Enter a title for the file you want to upload</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Thread ID (timestamp)]</td> 
   <td> <p>If you are uploading the file as a reply, enter or map the time stamp of the message you want to reply to.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Initial Comment]</td> 
   <td> <p>Enter or map the text of the message that introduces the file.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Create a Text File]**

This action module creates a text file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channels]</td> 
   <td> <p>For each channel you want to upload the file to, click <b>[!UICONTROL Add item]</b>, then select the channel type and channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>Enter a title for the file you want to upload</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Thread ID (timestamp)]</td> 
   <td> <p>If you are uploading the file as a reply, enter or map the time stamp of the message you want to reply to.</p> <p>Note: The time stamp can be retrieved using another module, such as the[!UICONTROL  Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Initial Comment]</td> 
   <td> <p>Enter or map the text of the message that introduces the file.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Delete a File]**

This action module returns deletes the specified file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td> <p>Enter or map the ID of the file that you want to delete. </p> <p>Note: The file ID can be retrieved using another module, such as the [!DNL Watch Files] Module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

-->

### 渠道

+++ **[!UICONTROL 列出频道]**

此搜索模块返回工作区中所有渠道的列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Slack]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL排除已存档的]</p> </td> 
   <td> <p>选择[！UICONTROL是]可在结果中排除存档的渠道。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL类型] </td> 
   <td> <p>选择要检索的渠道类型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>设置在一个执行周期内返回的最大通道数[!DNL Workfront Fusion]。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 获取频道]**

此操作模块返回有关工作区渠道的信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Slack]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL渠道ID]</p> </td> 
   <td> <p>输入或映射要检索相关信息的渠道ID。</p> <p>注意：可以使用[！UICONTROL List Channels]模块检索渠道ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 列出渠道中的成员]**

此搜索模块返回选定渠道中的用户列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Slack]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL渠道类型]</td> 
   <td>选择包含要列出的成员列表的渠道类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Public] / [！UICONTROL Private Channel]</td> 
   <td>选择要为其列出成员的渠道。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>设置在一个执行周期内[!DNL Workfront Fusion]返回的最大成员数。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

<!--

+++ **[!UICONTROL Set the Topic of a Channel]**

This action module changes the topic of a channel

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to change the topic for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM Channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to change the topic for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Topic]</td> 
   <td>Enter or map the new topic of the channel. This field does not support formatting or links.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Set the Purpose of a Channel]**

This action module changes the purpose of a channel

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to change the purpose for.</td> 
  </tr> 
  <tr> 
>[!MORELIKETHIS]
>
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM Channel] / User</td> 

   <td>Select the channel or user that you want to change the purpose for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Purpose]</td> 
   <td>Enter or map the new purpose of the channel. This field does not support formatting or links.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Join a Channel]**

This action module joins the user to a channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel ID]</p> </td> 
   <td> <p>Enter or map the ID of the channel that you want to join.</p> <p>Note: The Channel ID can be retrieved using the [!UICONTROL List Channels] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Leave a Channel]**

This action module removes the user from a channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel ID]</p> </td> 
   <td> <p>Enter or map the ID of the channel that you want to leave.</p> <p>Note: The Channel ID can be retrieved using the [!UICONTROL List Channels] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Create a Channel]**

This action module creates a new channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
   <td> <p>Enter or map a name for the new channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Is private]</td> 
   <td>Enable this option to set the new channel as private.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Archive a Channel]**

This action module archives a  channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel ID]</p> </td> 
   <td> <p>Enter or map the ID of the channel that you want to archive.</p> <p>Note: The Channel ID can be retrieved using the [!UICONTROL List Channels] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Unarchive a Channel]**

This action module unarchives a channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel ID]</p> </td> 
   <td> <p>Enter or map the ID of the channel that you want to unarchive.</p> <p>Note: The Channel ID can be retrieved using the [!UICONTROL List Channels] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Reactions

+++ **[!UICONTROL List reactions]**

This action module returns reactions that a user made.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL User]</p> </td> 
   <td> <p>Select the user that made the reactions that you want to list.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of reactions you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Add a reaction]**

This action module adds a reaction to an item.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to add a reaction to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to add a reaction to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Enter or map the time stamp of the message you want to add a reaction to.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reaction (emoji) name]</td> 
   <td>Enter or map the name of the emoji that you want to use for a reaction. Example: <code>thumbsup</code>. </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Remove a reaction]**

This action module adds a reaction to an item.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to remove a reaction from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to add a reaction from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Enter or map the time stamp of the message you want to add a reaction to.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reaction (emoji) name]</td> 
   <td>Enter or map the name of the emoji that you want to remove from the message. Example: <code>thumbsup</code>. </td> 
  </tr> 
 </tbody> 
</table>

+++

### Stars 

+++ **[!UICONTROL Add a star]**

This action module makes a channel a starred channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to add a star to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL IM] / [!UICONTROL Multiple IM channel]</td> 
   <td>Select the channel or user that you want to add a star to.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Remove a star]**

This action module removed the star from a starred channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to add a star to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL IM] / [!UICONTROL Multiple IM channel]</td> 
   <td>Select the channel or user that you want to add a star to.</td> 
  </tr> 
 </tbody> 
</table>

+++

### Saved Items

+++ **[!UICONTROL Save an Item]**

This action module adds an item to saved items.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID (Time stamp)]</td> 
   <td> <p> Enter or map the time stamp of the message you want to save.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td> <p>Enter or map the file that you want to save.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Remove Saved Item]**

This action module adds an item to saved items.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID (Time stamp)]</td> 
   <td> <p> Enter or map the time stamp of the message you want to remove from saved items.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td> <p>Enter or map the file you want to remove from saved items.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Pins

+++ **[!UICONTROL Pin an Item]**

This action module pins an item, such as a file or file comment, to a channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to pin an item to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to pin an item to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Enter or map the time stamp of the message you want to pin.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Unpin an Item]**

This action module unpins an item from a channel. You can unpin files, file comments, channel messages, or group messages.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to unpin an item from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to unpin an item from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Enter or map the time stamp of the message you want to unpin.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Users 

+++ **[!UICONTROL Watch Users]**

This trigger module starts the scenario when a new user is added to the [!DNL Slack] workspace.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Set the maximum number of users [!DNL Workfront Fusion] will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Search for User]**

This action module retrieves details about a single user, by using their email address.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Email] </p> </td> 
   <td> <p>Enter or map the email address of the user you want to retrieve details about.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL List Users]**

This action module returns a list of all users in a workspace.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Limit]</p> </td> 
   <td> <p>Enter or map the maximum number of users you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Get a User]**

This action module retrieves details about a member of a workspace.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL User ID]</p> </td> 
   <td> <p>Enter or map the User ID of the user you want to retrieve details for.</p> <p>Note: The User ID can be retrieved using another module, such as the [!DNL List Users] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Invite Users]**

This action module invites 1-30 users to a public or private channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want invite users to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to invite users to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Users]</td> 
   <td> <p>Select the users that you want to add to the channel.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Kick a User]**

This action module removes a user from a channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want remove a user from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private channel]</td> 
   <td>Select the channel that you want to remove a user from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Users]</td> 
   <td> <p>Select the user that you want to remove from the channel.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Reminders

+++ **[!UICONTROL List Reminders]**

This action module returns a list of all reminders created by or given to the currently authenticated user.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Limit]</p> </td> 
   <td> <p>Enter or map the maximum number of reminders you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Get a Reminder]**

This action module retrieves details about a specific reminder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Reminder ID]</p> </td> 
   <td> <p>Enter or map the Reminder ID of the reminder you want to retrieve details for.</p> <p>Note: The Reminder ID can be retrieved using another module, such as the [!UICONTROL List Reminders] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Create a Reminder]**

This action module creates a reminder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td>Enter or map the content of the reminder</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Time]</td> 
   <td> <p>Enter or map the date and time when this reminder should happen. Enter one of the following: </p> 
    <ul> 
     <li> <p>The Unix timestamp (up to five years from now)</p> </li> 
     <li> <p>The number of seconds until the reminder (if within 24 hours) </p> </li> 
     <li> <p>A natural language description (Examples: "in 15 minutes" or "every Thursday")</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL User] </p> </td> 
   <td> <p>Select the user that receives the reminder.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Complete a Reminder]**

This action module completes a specific reminder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Reminder ID]</p> </td> 
   <td> <p>Enter or map the Reminder ID of the reminder you want to complete.</p> <p>Note: The Reminder ID can be retrieved using another module, such as the [!UICONTROL List Reminders] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Delete a Reminder]**

This action module deletes a specific reminder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Reminder ID]</p> </td> 
   <td> <p>Enter or map the Reminder ID of the reminder you want to delete.</p> <p>Note: The Reminder ID can be retrieved using another module, such as the [!UICONTROL List Reminders] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Events

+++ **[!UICONTROL New Event]**

This instant trigger starts a scenario when a new message or other event is created.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Webhook]</p> </td> 
   <td> <p>Select the webhook you want to use.</p> <p>Or</p> <p>Create a new webhook.</p> 
    <ol> 
     <li value="1"> <p>Click <b>[!UICONTROL Add]</b>.</p> </li> 
     <li value="2"> <p>Select the event type.</p> </li> 
     <li value="3"> <p>Select or add a connection. For instructions about connecting your [!DNL Slack] account to [!UICONTROL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!UICONTROL Adobe Workfront Fusion] - Basic instructions</a></p> </li> 
     <li value="4"> <p>If prompted, select the channel that you want to watch.</p> </li> 
     <li value="5"> <p>Click <b>[!UICONTROL Save]</b> to save the webhook and return to the module.</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Profile

+++ **[!UICONTROL Set a status]**

This action module updates a user's current status.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Status text]</p> </td> 
   <td> <p>Enter or map the status text. Consider the following:</p> 
    <ul> 
     <li> <p>You can enter up to 100 characters.</p> </li> 
     <li> <p>You can use markup or other formatting, such as user mentions.</p> </li> 
     <li> <p>You can include emojis in the status text by using the format <code>:emojiname:</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status Emoji]</td> 
   <td> <p>Enter or map the emoji that you want to use to represent your status. Use the format <code>:emojiname:</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status expiration]</td> 
   <td>Enter or map the date and time you want the status to expire. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
 </tbody> 
</table>

+++

-->

### 其他

+++ **[!UICONTROL 进行API调用]**

此操作模块允许您对[!DNL Slack] API进行经过身份验证的自定义调用。 这样，您可以创建其他[!DNL Slack]模块无法实现的数据流自动化。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Slack]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>输入相对于<code>https://slack.com/api/</code>的路径。 示例： <code>/users/identity</code>。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP请求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[！UICONTROL Workfront Fusion]会为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：  <p>在JSON中使用条件语句（如<code>if</code>）时，请将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL基本URL]</td> 
   <td>选择要用于API调用的基本URL。</td> 
  </tr> 
 </tbody> 
</table>

+++

## 术语

在配置[!DNL Slack]模块时，以下术语可能很有用：

* **DM**： [!UICONTROL 直接消息]
* **即时消息**： [!UICONTROL 即时消息]
* **专用频道**：以前为[!UICONTROL 组]
* **直接消息**：以前为[!UICONTROL IM]
* **频道**： API文档中的[!UICONTROL 对话]，[!DNL Slack]应用程序中的[!UICONTROL 频道]。