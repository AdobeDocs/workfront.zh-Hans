---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: 使用Adobe Workfront MCP服务器
description: 使用Adobe Workfront MCP服务器，通过AI助手中的自然语言对话来搜索、创建、更新和管理Workfront项目。
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 4517d45ecc653d27d435a8192a612241120dd33f
workflow-type: tm+mt
source-wordcount: '1243'
ht-degree: 2%

---


# 使用Adobe Workfront MCP服务器

[!DNL Adobe Workfront] MCP服务器允许您通过询问纯英语的AI助手来查找、创建、更新和管理Workfront项目。 AI助手可决定要调用哪些Workfront操作，并为您处理与Workfront的对话。

[!DNL Claude]是当前唯一受支持的AI助手，但本文中的示例和模式适用于任何支持Workfront MCP服务器的AI助手。

本文假定您已设置连接。 有关安装的信息，请参阅[配置Adobe Workfront MCP服务器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)。 有关Workfront MCP服务器的详细信息，请参阅[Adobe Workfront MCP服务器概述](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md)。



## 通过Workfront MCP服务器可用的操作

Workfront MCP服务器涵盖了跨批准、规划和工作流的操作。

<!-- NEEDS DETAIL: Confirm the full inventory of actions exposed through the Workfront MCP server. The five core actions below are confirmed from Hamilton's walkthrough. The approvals, planning, and workflow sections need to be filled in from Jeff's engineering channel post, hands-on access, and the deck Oznur published in the MCP external channel. -->

>[!IMPORTANT]
>
>人工智能助手使用您的Workfront帐户和权限在Workfront中执行操作。 您和您的AI助手提供商将负责AI助手代表您执行的操作。 在让AI助手继续操作之前，请确认AI助手将要执行的操作。


## 负责AI助理操作

将AI助手连接到Workfront时，AI助手将使用您的Workfront帐户和权限在Workfront中执行操作。 AI助手的操作与您直接在Workfront界面中执行的操作具有相同的效果。

您和您的AI助手提供商负责AI助手在Workfront中执行的操作。 Adobe不负责更改AI助手对Workfront数据所做的更改。

在让AI助手继续请求之前，请确认您了解它要执行的操作，尤其是更改或删除数据的操作。

### 核心操作

Workfront MCP服务器包括以下核心操作：

| 操作 | 作用 |
|---|---|
| 创建 | 在Workfront中创建新项目。 |
| 搜索 | 查找和检索Workfront中的项目。 |
| 更新 | 更改Workfront中的现有项目。 |
| 删除 | 从Workfront中删除项目。 |
| 解析字段名称 | 查找正确的Workfront字段名称，以便AI助手可以根据您的数据构建准确的请求。 |

<!-- NEEDS DETAIL: Confirm which Workfront object types are supported across the core actions (projects, tasks, issues, portfolios, programs, custom forms, planning records, approvals, etc.). -->

### 审批操作

<!-- NEEDS DETAIL: List the approval-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request a marketer might make. -->

### 规划操作

<!-- NEEDS DETAIL: List the planning-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

### 工作流操作

<!-- NEEDS DETAIL: List the workflow-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

## 要问的内容的示例

连接后，在AI助手中键入自然语言请求。 AI助手确定要调用的Workfront操作并返回结果。

<!-- NEEDS DETAIL: Example prompts in this section are adapted from the Workflow Optimization Agent (WOA) examples doc on another branch. Validate each example against a working Claude + Workfront MCP server setup before publication, since WOA and the MCP server may expose different action inventories. -->

### 查找并查看您的工作

要求AI助手搜索Workfront以查找与您所查找的内容匹配的项目。 例如：

* *显示品牌营销团队的所有活动项目。*
* *获取分配给Joan Harris的所有任务。*
* *在“技术”类别下显示“网站重新设计”项目中的所有问题。*

### 创建新项目

请求AI助手创建项目、任务或其他Workfront项。 例如：

* *从3月10日至4月30日创建一个名为“Q2 Innovation Sandbox”的空白项目。 将我设置为所有者。*
* *将名为“登陆页面QA”的新任务添加到项目中，并计划从4月22日至4月26日执行。*
* *创建新的营销活动记录，名为“2026年夏季促销”。*

### 更新现有项

请求AI助手更改Workfront中已存在的项目。 例如：

* *更新“设计审阅”任务，使其在4月18日完成，并将其分配给创意团队。*
* *对于“Lucent AI Launch - NA”项目，请将完成日期推迟到4月中旬，并将预算增加到15万美元。*
* *将“夏季促销活动”记录中的预算字段更新为$75,000。*

### 删除项目

请求AI助手删除Workfront项目。 例如：

* *删除名为“Q1测试营销活动”的项目。*
* *从项目中删除“打印资产生产”任务。*
* *删除名为“旧促销活动”的促销活动记录。*

>[!WARNING]
>
>通过AI助手删除Workfront中的项目，与在Workfront界面中删除这些项目相同。 在继续操作之前，请确认AI助手将要删除的内容。

### 使用审批

请求AI助手管理文档和资产批准。 例如：

* *将Sarah Chen和Miguel Alvarez添加为当前文档的批准者。*
* *向资源“Spring Campaign视频”的批准者发送提醒，后者尚未回复。*
* *将“营销启动”审批模板应用于资产“春季促销活动视频”。*

<!-- NEEDS DETAIL: Add approvals-specific context from the WOA examples doc, including: content approvals must be enabled for the organization, the AI assistant cannot approve or reject on behalf of humans (except via the Workfront AI Reviewer), and best experience is with the Unified Approvals experience. -->

### 使用计划记录

要求人工智能助理管理规划记录。 例如：

* *为品牌营销团队创建一个名为“Q2营销计划”的新计划记录。*
* *将名为“社交媒体审核”的新任务添加到计划记录中。*
* *更新“社交媒体审核”任务，使其在4月18日完成，并将其分配给创意团队。*

### 使用工作流

请求AI助手管理工作流。 例如：

* *将“Q2创新沙盒”项目路由到创新审核委员会。*
* *将“夏季促销活动”记录更新为“准备启动”状态。*
* *批准“夏季营销活动”记录。*


### 在对话中链结请求

您可以在单个对话中链结请求。 AI助手会保留上下文，以便每个请求都可以基于前一个请求进行构建。 例如：

1. 要求AI助手查找一组项目： *查找我的过期任务。*
1. 在AI助手返回列表后，要求其对结果执行操作： *将所有结果更新到下个星期五。*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## 注意事项

在使用Workfront MCP服务器时，请牢记以下注意事项。

### AI助理可以使用对话中较早出现的信息

人工智能助理有时会重复使用对话中早期的数据，而不是请求Workfront提供最新信息。 如果自上次查看AI助手以来Workfront中的某些内容发生了更改，您可能会看到过时的信息。

要强制AI助手获取新数据，请明确询问该变量。 例如：

* *从Workfront获取最新数据。 不使用缓存的结果。*

### Workfront MCP服务器会自动更新

当Adobe发布新版本的Workfront MCP服务器时，您的AI助手会自动使用新版本。 您无需重新连接或更改任何内容。

## 数据和安全性

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI assistant. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI assistant provider, what happens to it after the conversation ends, and any differences between AI assistants (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### 哪些数据离开Workfront

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI assistant (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### AI助手提供商如何处理您的Workfront数据

<!-- NEEDS DETAIL: For each supported AI assistant, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### AI助理之间的区别

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI assistant handles Workfront data once additional AI assistants are supported. -->

## 日常使用故障诊断

有关设置和身份验证问题的详细信息，请参阅[配置Adobe Workfront MCP服务器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)中的[设置和身份验证疑难解答](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication)。

| 问题 | 可能的原因 | 修复 |
|---|---|---|
| AI助手正在向您提供过时的信息。 | AI助手正在重用对话中早期的数据。 | 请求AI助手从Workfront获取新数据。 |
| AI助手从错误的Workfront项目返回数据。 | AI助手根据模糊的措辞挑选了错误的项目。 | 使用更具体的名称、ID或过滤器再次询问。 |
| 更新或删除操作在Workfront中未生效。 | AI助手尚未调用操作，或您的权限不允许执行此操作。 | 通过AI助手确认操作已运行，然后检查您的Workfront权限。 |

<!-- NEEDS DETAIL: Add additional day-to-day troubleshooting scenarios discovered during hands-on testing. -->

## 常见问题

### 我可以通过人工智能助手处理哪些Workfront项目？

您在Workfront中通过访问级别和对象权限有权访问的任何项目。

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### 我的Workfront数据是发送到AI助手提供商还是由他们存储？

有关详细信息，请参阅本文中的[数据和安全性](#data-and-security)。

### 新版本的Workfront MCP服务器发布后会发生什么情况？

MCP服务器会自动更新。 您无需重新连接或更改任何内容。

### 要使用Workfront MCP服务器，我是否需要知道Workfront API？

不可以。 AI助手会将您的自然语言请求翻译为正确的Workfront操作。 如果您已经熟悉Workfront API，那么您会觉得熟悉API的操作，但这不是必需的。
