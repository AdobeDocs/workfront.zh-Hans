---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: 配置Adobe Workfront MCP服务器
description: 配置Workfront实例和AI助手，以便通过自然语言对话使用Workfront。
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 4517d45ecc653d27d435a8192a612241120dd33f
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 3%

---


# 配置Adobe Workfront MCP服务器

[!DNL Adobe Workfront] MCP服务器允许您在受支持的AI助手（如Claude或ChatGPT）中通过自然语言对话处理Workfront数据。

在将AI助手连接到Workfront之前，Workfront管理员必须在Workfront实例中启用MCP服务器访问。 对于每个支持的AI助手，连接AI助手的确切步骤有所不同。

有关Workfront MCP服务器的详细信息，请参阅[Adobe Workfront MCP服务器概述](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md)。

## 支持的AI助理

Workfront MCP服务器当前支持以下AI助手：

* [!DNL Claude]

<!-- NEEDS DETAIL: Update this list as Adobe adds support for additional AI assistants (for example, [!DNL Gemini], or [!DNL Microsoft Copilot]). -->

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront package requirement (Select, Prime, Ultimate, Any?) --></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront license requirement (Standard, Work, etc.) --></p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在将Workfront连接到AI助手之前，您必须：

* 拥有活动[!DNL Adobe Workfront]帐户，该帐户具有访问要处理的数据的权限。
* 有权访问类似[!DNL Claude]的AI助手。

  <!-- NEEDS DETAIL: Confirm which Claude tiers are supported. Claude Enterprise is confirmed; Claude Pro and Claude Team support is unconfirmed. -->

### 管理员先决条件

MCP服务器访问由两个不同的管理员控制。 在连接之前，两者都必须启用访问。

* **您的Workfront管理员**&#x200B;必须在Workfront实例中启用MCP服务器访问权限。

* 如果您使用企业版本的AI助手，则AI助手管理员必须为您的组织启用[!DNL Adobe Workfront]连接器。


## 将Workfront连接到克劳德

您为每个[!DNL Claude]帐户连接到Workfront一次。 该连接会向您验证特定Workfront实例，在您选择断开连接之前，您会一直保持连接。


>[!IMPORTANT]
>
>如果您使用[!DNL Claude]企业版，**您的[!DNL Claude]企业管理员**&#x200B;必须为您的组织启用[!DNL Adobe Workfront]连接器。 在此之前，当您在[!DNL Claude]中搜索[!DNL Adobe Workfront]连接器时，该连接器将不会显示。 请先联系您的[!DNL Claude]管理员。


要将Workfront连接到[!DNL Claude]，请执行以下操作：

1. 打开[!DNL Claude]。

1. 导航到连接器区域。

   <!-- NEEDS DETAIL: Exact menu path (for example, "Click Settings, then click Connectors"). -->

1. 在连接器列表中查找&#x200B;**[!DNL Adobe Workfront]**。

   如果您没有看到此项，请参阅本文中的[管理员先决条件](#admin-prerequisites)。

1. 单击&#x200B;**连接**。

   <!-- NEEDS DETAIL: Confirm the exact button label. -->

1. 出现提示时，登录到您的Workfront实例。

   <!-- NEEDS DETAIL: Describe the auth flow — does it open a new browser tab, an in-app window, prompt for a Workfront domain? -->

1. 身份验证完成后，你已连接。

   <!-- NEEDS DETAIL: Add a screenshot of the connected state in Claude. -->

### 验证您的连接

要确认[!DNL Claude]已连接到Workfront，请要求[!DNL Claude]列出Workfront MCP服务器可执行的操作。 例如：

* *您可以执行哪些Workfront操作？*
* *列出您有权访问的Workfront工具。*

[!DNL Claude]返回可用操作的列表。

<!-- NEEDS DETAIL: Add a screenshot of the tool-list response. -->

### 切换到其他Workfront实例

每个连接都向单个Workfront实例验证[!DNL Claude]。 要使用其他实例，请断开并重新连接。

连接到其他Workfront实例：

1. 在[!DNL Claude]中，断开[!DNL Adobe Workfront]连接器。
1. 重新连接连接器。
1. 对新的Workfront实例进行身份验证。

>[!NOTE]
>
>仅注销[!DNL Claude]不会切换Workfront实例。 必须断开并重新连接连接器。

## 使用技能自定义克劳德行为

<!-- NEEDS DETAIL: Confirm whether Adobe is shipping any pre-built Claude skills alongside the MCP server. If yes, list them and link to download or installation guidance. If no, decide whether to mention skills as a user-driven workaround at all, or remove this section. -->

[!DNL Claude]支持由用户创建的称为“技能”的说明集。 您可以使用技能自定义[!DNL Claude]在Workfront中的行为方式。 例如，您可以创建一项技能，告知[!DNL Claude]始终从Workfront中获取最新数据，而不是依赖以前的结果。

## 设置和身份验证疑难解答

| 问题 | 可能的原因 | 修复 |
|---|---|---|
| 在[!DNL Claude]中找不到[!DNL Adobe Workfront]连接器。 | 您的[!DNL Claude]管理员尚未启用它。 | 请联系您的[!DNL Claude]管理员（而不是Workfront管理员），要求他们启用[!DNL Adobe Workfront]连接器。 |
| 您已连接，但看不到您的数据。 | 您使用了错误的Workfront实例进行身份验证。 | 断开连接器，重新连接并验证正确的实例。 |
| 身份验证失败，或连接停止工作。 | 您的身份验证会话已过期或存在连接错误。 | 断开并重新连接连接器。 |
| 您希望切换到其他Workfront实例。 | 单个连接会将您绑定到一个实例。 | 断开新实例的连接、重新连接并进行身份验证。 |

<!-- NEEDS DETAIL: Add additional setup/authentication troubleshooting scenarios discovered during hands-on testing. -->

有关连接后的日常故障排除（例如，陈旧的结果或意外行为），请参阅[使用Adobe Workfront MCP服务器](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)。

## 有关设置的常见问题解答

### 我是否可以同时连接到多个Workfront实例？

不可以。 每个连接都将AI助手与单个Workfront实例关联。 要切换，请断开并重新连接，对新实例进行身份验证。

### 这是否适用于Claude Pro或Claude Team，还是仅适用于Claude Enterprise？

<!-- NEEDS DETAIL: Confirm Claude tier support and answer this directly. -->

### 由哪个管理员启用此功能？

Workfront管理员和AI助理管理员。 您的Workfront管理员可以在Workfront端启用MCP服务器访问。 您的AI助手管理员可在AI助手端启用Workfront访问权限。 对于[!DNL Claude]，[!DNL Claude]企业管理员启用[!DNL Adobe Workfront]连接器。
