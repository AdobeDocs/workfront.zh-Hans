---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP服务器概述
description: 了解Adobe Workfront MCP服务器的功能以及它如何让您通过AI代理平台中的自然语言对话来使用Workfront。
author: Courtney
feature: Get Started with Workfront
source-git-commit: f96afd17e9f4e726ac545a9cb0c54ace5a4fcffe
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---


# Adobe Workfront MCP服务器概述

{{highlighted-preview-article-level}}

[!DNL Adobe Workfront] MCP服务器将您的Workfront实例连接到AI代理平台，如[!DNL Claude]或[!DNL ChatGPT]。 在AI代理平台中，您可以通过发出自然语言请求来查找、创建、更新和管理Workfront项目。

例如，您可以询问：

* *显示品牌营销团队的所有活动项目。*
* *更新“设计审阅”任务，使其在4月18日完成。*
* *向资源“Spring Campaign视频”的批准者发送提醒，后者尚未回复。*

您无需了解Workfront API或MCP服务器的工作方式，即可使用Workfront MCP服务器。

>[!IMPORTANT]
>
>目前，Workfront MCP服务器仅适用于美国地区的客户以及使用AWS的客户。

## MCP服务器是什么

MCP服务器是一个连接点，它允许AI代理平台与另一个系统一起使用。 Workfront MCP服务器是您的AI代理平台连接到的内容，因此它可以代表您读取和处理Workfront数据。

MCP代表“模型上下文协议”。 这个标准定义了AI代理平台和外部系统如何相互通信。

## 设置连接

Workfront MCP服务器可与任何与MCP兼容的AI代理平台（如[!DNL Claude]或[!DNL ChatGPT]）配合使用。 在使用它之前，需要发生以下情况：

* Workfront管理员必须在Workfront实例中启用MCP服务器访问权限。
* 您（或您的管理员）必须将AI代理平台连接到Workfront。

有关详细信息，请参阅[配置Adobe Workfront MCP服务器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)。

## 开始使用Workfront MCP服务器

设置后，您可以要求AI代理平台查找、创建、更新和管理自然语言的Workfront项目。

有关详细信息，包括示例请求、要牢记的事项以及有关数据和安全性的信息，请参阅[使用Adobe Workfront MCP服务器](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)。