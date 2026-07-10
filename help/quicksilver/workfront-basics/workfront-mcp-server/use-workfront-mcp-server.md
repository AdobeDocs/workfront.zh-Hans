---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: 使用Adobe Workfront MCP服务器
description: 使用Adobe Workfront MCP服务器可通过人工智能代理平台中的自然语言对话，搜索、创建、更新和管理Workfront项目。
author: Courtney
feature: Get Started with Workfront
source-git-commit: 5592c1b93b5e44c732f92d626ed878d2c4647ceb
workflow-type: tm+mt
source-wordcount: '1896'
ht-degree: 0%

---


# 使用Adobe Workfront MCP服务器

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览Sandbox”环境中可用。</span>

[!DNL Adobe Workfront] MCP服务器允许您通过询问自然语言的AI代理平台来查找、创建、更新和管理Workfront项目。 平台会决定要调用哪些Workfront操作，并帮您处理与Workfront的对话。

>[!IMPORTANT]
>
>目前，Workfront MCP服务器仅适用于使用AWS的客户。

## 先决条件

* 您必须在AI代理平台和Workfront MCP服务器之间建立连接。 有关设置说明，请参阅[配置Adobe Workfront MCP服务器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)。
* 必须在Adobe Identity Management System (IMS)上启用您的Workfront实例。
* 您必须拥有对要处理的项目具有必要访问级别和对象权限的Workfront帐户。
* 要将MCP与Workfront Planning结合使用，您的组织必须位于包含Adobe Workfront Planning的Workfront程序包上。

本文假定您已设置连接。 有关安装的信息，请参阅[配置Adobe Workfront MCP服务器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)。

## 可用工具

Workfront MCP服务器会公开AI代理平台代表您调用的一组工具。 例如，用于搜索Workfront、创建项目、更新字段和管理审批的工具。 有关完整参考列表，请参阅[Adobe Workfront MCP服务器工具](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md)。

>[!IMPORTANT]
>
>将AI代理平台连接到Workfront时，它会使用您的Workfront帐户和权限在Workfront中起作用。 平台的操作与您直接在Workfront界面中执行的操作具有相同的效果。<br>
>
>您和您的AI代理平台提供商负责平台在Workfront中执行的操作。 Adobe不负责对Workfront数据进行AI代理平台更改。<br>
>
>在让AI代理平台继续处理请求之前，请确认您了解该平台要执行的操作，尤其是更改或删除数据的操作。


## 要问的内容的示例

连接后，在AI代理平台中键入自然语言请求。 AI代理平台确定要调用的Workfront操作并返回结果。

>[!NOTE]
>
>由于Workfront设置区域中的管理员控件，某些操作可能不可用。 例如，如果Workfront管理员已禁用MCP服务器的写入操作，则您可能无法创建项目。


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

<!--
* *Remove Anna Jones from all approvals in this project, and replace with Sione Carter.*
-->


### 使用计划记录

>[!IMPORTANT]
>
>* 要将MCP与Workfront Planning结合使用，您的组织必须位于包含Adobe Workfront Planning的Workfront程序包上。

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


## 注意事项

在使用Workfront MCP服务器时，请牢记以下注意事项：

### AI代理平台可以使用对话前面的信息

AI代理平台有时会重复使用对话中早期的数据，而不是向Workfront索取最新信息。 如果自上次查看AI代理平台以来Workfront中的某些内容发生了变化，您可能会看到过时的信息。

要强制AI代理平台获取新数据，请明确要求获取新数据。 例如：

* *从Workfront获取最新数据。 不使用缓存的结果。*

### 检查Workfront MCP服务器的更新

您可能需要定期刷新与Workfront MCP服务器的连接，以确保您拥有最新的工具和功能。

大多数更新应该会自动进行。 但是，我们建议定期查看Workfront发行说明。


## 数据和安全性

Workfront MCP服务器工具与API调用的工作方式一致。 Workfront不存储提示、响应或任何其他数据。 您可以通过Workfront平台访问您所需要的Workfront数据。

您的访问级别和对象权限决定了您可以查询或写入Workfront的内容。 您的Workfront管理员可以在Workfront设置区域中控制MCP读取和写入操作。

### 哪些数据离开Workfront

AI代理平台提供商可以访问您通过Workfront MCP服务器与之交互的Workfront数据。 有关详细信息，请咨询您的AI代理平台提供商。


### AI代理平台提供商如何处理您的Workfront数据

Workfront无法控制AI代理平台提供商处理您的Workfront数据的方式。 有关详细信息，请咨询您的AI代理平台提供商。

## 日常使用故障诊断

+++ 展开以查看日常使用Workfront MCP服务器的故障排除提示。

| 问题 | 可能的原因 | 修复 |
| --- | --- | --- |
| AI代理平台正在为您提供过时的信息。 | AI代理平台正在重用对话中早期的数据。 | 从Workfront索取最新数据。 |
| AI代理平台从错误的Workfront项目返回数据。 | AI代理平台根据模棱两可的措辞挑选了错误的项目。 | 使用更具体的名称、ID或过滤器再次询问。 |
| 更新或删除操作在Workfront中未生效。 | 您的Workfront管理员已禁用Workfront MCP服务器的写入操作，或者您无权对特定项目执行该操作。 | 通过AI代理平台确认该操作已运行。 然后，检查是否已为Workfront MCP服务器启用写入操作，以及您是否有权更改该项目。 |

有关设置和身份验证问题的详细信息，请参阅[配置Adobe Workfront MCP服务器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)中的[设置和身份验证疑难解答](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication)。

+++

## 常见问题

+++ 展开以查看有关使用Workfront MCP服务器的常见问题解答。

### 什么是AI代理平台？

AI代理平台是一种AI工具，可以在以下位置代表您执行操作：
其他系统，而不仅仅是回答问题。 当您将一个连接到Workfront时
通过MCP服务器，可以查找、创建、更新和删除Workfront
项根据您以自然语言询问的内容而定。 示例包括Claude
Desktop、ChatGPT和其他与MCP兼容的AI客户端。


### 我是否需要成为Workfront管理员才能使用Workfront MCP服务器？

不可以。 任何Workfront用户都可以通过连接的使用Workfront MCP服务器
AI代理平台。 AI代理平台使用您的Workfront进行操作
帐户、访问级别和对象权限，因此您只能执行您自己的操作
可能已经直接在Workfront中执行了上述操作。

### 为什么AI代理平台不能为我创建、更新或删除项目？

您的Workfront管理员可控制中允许的MCP操作
Workfront设置区域。 如果禁用写入操作，则AI代理平台
仍然可以查找和读取Workfront项目，但无法进行更改。 您也可以
需要具有对特定项目的正确访问级别和对象权限
您正在合作。

### AI代理平台在更改或删除Workfront数据之前是否会询问我？

这取决于人工智能的平台，而不是Workfront。 大多数平台
提示您在用户运行操作（尤其是删除操作）之前进行确认。在批准请求之前，请阅读平台声明将要执行的操作：
这些更改在Workfront中发生的方式与做出更改时的方式相同
您自己也在界面中。

<!--

### Can I undo something the AI agentic platform did in Workfront?

Changes the AI agentic platform makes in Workfront work the same way as 
changes you make in the interface. If Workfront supports undoing or 
restoring a particular action (for example, restoring a deleted item from 
the Recycle Bin), the same options apply. If Workfront doesn't normally let 
you undo an action, you can't undo it through the AI agentic platform either.

-->

### 为什么AI代理平台返回错误的Workfront项目？

AI代理平台会根据您使用的单词选择项目。 如果您的
请求不明确（例如，两个项目具有相似的名称）
可能会选错对象。 再次询问更具体的名称、ID、日期、
或过滤以缩小结果范围。


### 我可以通过人工智能代理平台处理哪些Workfront项目？

通过您的访问级别和在Workfront中有权访问的任何项目
对象权限。 这包括项目、任务、问题、文档、
审批、规划记录等。

### 其他人能否看到我与人工智能代理平台的对话？

Workfront不会存储您的提示或AI代理平台的响应。AI代理平台的所有提供者控制对话的方式
存储或共享。 与您的AI代理平台提供商联系，以了解
详细信息。

### 我是否需要知道Workfront API或要使用哪种MCP工具？

不可以。 AI代理平台可将您的自然语言请求转换为
Workfront的正确操作并为您选择正确的工具。 如果您是
已经熟悉Workfront API，操作将会很熟悉，
但这不是必要条件。

### 我的Workfront数据是被发送到AI代理平台提供商还是由它们存储？

有关详细信息，请参阅此中的[数据和安全性](#data-and-security)
文章。

### 新版本的Workfront MCP服务器发布后会发生什么情况？

MCP服务器通常会自动更新，但有时您可能需要刷新与MCP服务器的连接才能查看最新的工具和功能。

### 如果未在Workfront Identity Management System (IMS)上启用我的Workfront实例，我能否使用Adobe MCP服务器？

不可以。 必须在Adobe Identity Management System (IMS)上启用Workfront实例，才能使用Workfront MCP服务器。 如果您不确定实例是否已在IMS中启用，请与Workfront管理员联系。


+++
