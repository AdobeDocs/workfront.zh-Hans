---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: 使用Adobe Workfront MCP服务器
description: 使用Adobe Workfront MCP服务器可通过人工智能代理平台中的自然语言对话，搜索、创建、更新和管理Workfront项目。
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 152486b7850e01f3de23f22bbe3729c5cd3d3aa2
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 0%

---


# 使用Adobe Workfront MCP服务器

[!DNL Adobe Workfront] MCP服务器允许您通过询问纯英文的AI代理平台来查找、创建、更新和管理Workfront项目。 平台会决定要调用哪些Workfront操作，并帮您处理与Workfront的对话。

[!DNL Claude]是当前唯一受支持的AI代理平台，但本文中的示例和模式适用于任何支持Workfront MCP服务器的AI代理平台。

本文假定您已设置连接。 有关安装的信息，请参阅[配置Adobe Workfront MCP服务器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)。 有关Workfront MCP服务器的详细信息，请参阅[Adobe Workfront MCP服务器概述](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md)。

## 可用工具

Workfront MCP服务器公开AI代理平台代表您调用的一组工具 — 例如，用于搜索Workfront、创建项目、更新字段和管理审批的工具。 有关按Workfront区域分组的完整参考列表，请参阅[Adobe Workfront MCP服务器工具](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md)。

>[!IMPORTANT]
>
>将AI代理平台连接到Workfront时，它会使用您的Workfront帐户和权限在Workfront中起作用。 平台的操作与您直接在Workfront界面中执行的操作具有相同的效果。
>
>您和您的AI代理平台提供商负责平台在Workfront中执行的操作。 Adobe不负责更改人工智能代理平台对Workfront数据所做的更改。
>
>在让AI代理平台继续处理请求之前，请确认您了解该平台要执行的操作，尤其是更改或删除数据的操作。


## 要问的内容的示例

连接后，在AI代理平台中键入自然语言请求。 AI代理平台确定要调用的Workfront操作并返回结果。

### 查找并查看您的工作

要搜索Workfront中与您正在寻找的项目相匹配的项目，请询问：

* *显示品牌营销团队的所有活动项目。*
* *获取分配给Joan Harris的所有任务。*
* *在“技术”类别下显示“网站重新设计”项目中的所有问题。*

### 创建新项目

要创建项目、任务或其他Workfront项，请询问：

* *从3月10日至4月30日创建一个名为“Q2 Innovation Sandbox”的空白项目。 将我设置为所有者。*
* *将名为“登陆页面QA”的新任务添加到项目中，并计划从4月22日至4月26日执行。*
* *创建新的营销活动记录，名为“2026年夏季促销”。*

### 更新现有项

要更改Workfront中已存在的项目，请询问：

* *更新“设计审阅”任务，使其在4月18日完成，并将其分配给创意团队。*
* *对于“Lucent AI Launch - NA”项目，请将完成日期推迟到4月中旬，并将预算增加到15万美元。*
* *将“夏季促销活动”记录中的预算字段更新为$75,000。*

### 删除项目

要删除Workfront项目，请询问：

* *删除名为“Q1测试营销活动”的项目。*
* *从项目中删除“打印资产生产”任务。*
* *删除名为“旧促销活动”的促销活动记录。*

>[!WARNING]
>
>通过AI代理平台删除Workfront中的项目，与在Workfront界面中删除这些项目相同。 在继续操作之前，请确认AI代理平台将要删除的内容。

### 使用审批

要管理文档和资产审批，请询问：

* *将Sarah Chen和Miguel Alvarez添加为当前文档的批准者。*
* *向资源“Spring Campaign视频”的批准者发送提醒，后者尚未回复。*
* *将“营销启动”审批模板应用于资产“春季促销活动视频”。*


### 使用计划记录

要管理计划记录，请询问：

* *为品牌营销团队创建一个名为“Q2营销计划”的新计划记录。*
* *将名为“社交媒体审核”的新任务添加到计划记录中。*
* *更新“社交媒体审核”任务，使其在4月18日完成，并将其分配给创意团队。*

### 使用工作流

要管理工作流，请询问：

* *将“Q2创新沙盒”项目路由到创新审核委员会。*
* *将“夏季促销活动”记录更新为“准备启动”状态。*
* *批准“夏季营销活动”记录。*


### 在对话中链结请求

您可以在单个对话中链结请求。 AI代理平台会保留上下文，以便每个请求都可以基于前一个请求进行构建。 例如：

1. 请求一组项目：*查找我的过期任务。*
1. 获取列表后，请求对结果执行操作： *将所有结果更新到下个星期五。*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## 注意事项

在使用Workfront MCP服务器时，请牢记以下注意事项。

### AI代理平台可以使用对话前面的信息

AI代理平台有时会重复使用对话中早期的数据，而不是向Workfront索取最新信息。 如果自上次查看AI代理平台以来Workfront中的某些内容发生了变化，您可能会看到过时的信息。

要强制AI代理平台获取新数据，请明确要求获取新数据。 例如：

* *从Workfront获取最新数据。 不使用缓存的结果。*

### Workfront MCP服务器会自动更新

当Adobe发布新版本的Workfront MCP服务器时，您的AI代理平台会自动使用新版本。 您无需重新连接或更改任何内容。

## 数据和安全性

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI agentic platform. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI agentic platform provider, what happens to it after the conversation ends, and any differences between AI agentic platforms (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### 哪些数据离开Workfront

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI agentic platform (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### AI代理平台提供商如何处理您的Workfront数据

<!-- NEEDS DETAIL: For each supported AI agentic platform, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### AI代理平台之间的差异

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI agentic platform handles Workfront data once additional AI agentic platforms are supported. -->

## 日常使用故障诊断

+++ 展开以查看日常使用Workfront MCP服务器的故障排除提示。

| 问题 | 可能的原因 | 修复 |
|---|---|---|
| AI代理平台正在为您提供过时的信息。 | AI代理平台正在重用对话中早期的数据。 | 从Workfront索取最新数据。 |
| AI代理平台从错误的Workfront项目返回数据。 | AI代理平台根据模棱两可的措辞挑选了错误的项目。 | 使用更具体的名称、ID或过滤器再次询问。 |
| 更新或删除操作在Workfront中未生效。 | AI代理平台尚未调用操作，或您的权限不允许执行此操作。 | 通过AI代理平台确认操作已运行，然后检查您的Workfront权限。 |

有关设置和身份验证问题的详细信息，请参阅[配置Adobe Workfront MCP服务器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)中的[设置和身份验证疑难解答](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication)。

+++

## 常见问题

+++ 展开以查看有关使用Workfront MCP服务器的常见问题解答。

### 我可以通过人工智能代理平台处理哪些Workfront项目？

您在Workfront中通过访问级别和对象权限有权访问的任何项目。

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### 我的Workfront数据是被发送到AI代理平台提供商还是由它们存储？

有关详细信息，请参阅本文中的[数据和安全性](#data-and-security)。

### 新版本的Workfront MCP服务器发布后会发生什么情况？

MCP服务器会自动更新。 您无需重新连接或更改任何内容。

### 要使用Workfront MCP服务器，我是否需要知道Workfront API？

不可以。 AI代理平台可将您的自然语言请求转换为正确的Workfront操作。 如果您已经熟悉Workfront API，那么您会觉得熟悉API的操作，但这不是必需的。

+++
