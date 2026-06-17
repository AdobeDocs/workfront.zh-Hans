---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: 配置Adobe Workfront MCP服务器
description: 配置Workfront实例和AI代理平台，以便通过自然语言对话使用Workfront。
author: Courtney
feature: Get Started with Workfront
source-git-commit: 3f59326d26a8c9ccd88f14d7d6459e486fcfe8c9
workflow-type: tm+mt
source-wordcount: '1747'
ht-degree: 0%

---


# 配置Adobe Workfront MCP服务器

[!DNL Adobe Workfront] MCP服务器允许您在受支持的AI代理平台上通过自然语言对话处理Workfront数据。

在将AI代理平台连接到Workfront之前，Workfront管理员必须在Workfront实例中启用MCP服务器访问。 对于每个受支持的AI代理平台，连接AI代理平台的确切步骤有所不同。

>[!IMPORTANT]
>
>目前，Workfront MCP服务器仅适用于使用AWS的客户。 不久的将来，使用GCP或Azure的客户将能够使用此功能。

## 支持的AI代理平台

Workfront MCP服务器可与支持模型上下文协议(MCP)的任何AI代理平台配合使用。

本文逐步介绍的连接步骤：

* [!DNL Claude]
* [!DNL ChatGPT]

如果您使用其他MCP兼容的AI代理平台（例如，[!DNL Gemini]或[!DNL Microsoft Copilot]），请按照该平台文档中的步骤添加自定义MCP服务器。 当提示您输入MCP服务器URL时，请输入您所在地区的URL：

| 区域 | URL |
| --- | --- |
| 美国 | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
| 欧盟 | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |

## 先决条件

在将Workfront连接到AI代理平台之前，您必须：

* 拥有活动[!DNL Adobe Workfront]帐户，该帐户具有访问要使用的数据的权限
* 有权访问AI代理平台，如[!DNL Claude]
* 必须在Adobe Identity Management System (IMS)上启用您的Workfront实例。
* 要将MCP与Workfront Planning结合使用，您的组织必须位于包含Adobe Workfront Planning的Workfront程序包上。


### 管理员先决条件

MCP服务器访问由两个不同的管理员控制。

* 您的Workfront管理员通过系统首选项中的两个切换控制Workfront实例的MCP服务器访问：**只读MCP工具**（默认启用）和&#x200B;**写入MCP工具**（默认禁用）。 如果您可以通过AI代理平台找到Workfront项目，但无法创建、更新或删除它们，请让Workfront管理员启用写入操作。

  有关详细信息，请参阅[配置系统首选项](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)。

* 如果您使用企业版AI代理平台，则该平台的管理员必须为您的组织启用[!DNL Adobe Workfront]连接器，或为您提供自定义URL访问权限以连接到Workfront MCP服务器。


## 将Workfront连接到克劳德

您为每个[!DNL Claude]帐户连接到Workfront一次。 该连接会向您验证特定Workfront实例，在您选择断开连接之前，您会一直保持连接。



### 从连接器目录连接到Claude desktop

>[!IMPORTANT]
>
>目前，Claude Connector仅支持连接到美国地区的Workfront MCP服务器。  要连接到EU地区的Workfront实例，请参阅本文中的[使用URL连接到Claude](#connect-to-claude-with-a-url)。

+++ 展开以查看有关将Workfront连接到[!DNL Claude]的分步说明。

要将Workfront连接到[!DNL Claude]，请执行以下操作：

1. 打开[!DNL Claude]。

1. 导航到连接器区域。



1. 在连接器列表中查找&#x200B;**[!DNL Adobe Workfront]**。

   如果您没有看到此项，请参阅本文中的[管理员先决条件](#admin-prerequisites)。

1. 单击&#x200B;**连接**。



1. 出现提示时，登录到您的Workfront实例。


1. 身份验证完成后，你已连接。



+++

### 使用URL连接到Claude

+++ 展开以查看使用URL将Workfront连接到[!DNL Claude]的分步说明。

>[!NOTE]
>
>您必须是企业Claude环境中的所有者才能执行此过程。
>
>有关Claude关于所有者要求的声明，请参阅Claude文档中的[添加自定义连接器](https://support.claude.com/en/articles/11175166-get-started-with-custom-connectors-using-remote-mcp#:~:text=Note%3A%20While,has%20access%20to)。

要使用URL将Workfront连接到[!DNL Claude]，请执行以下操作：

1. 使用您的凭据登录[Claude](https://claude.ai)。
1. 在左侧菜单中，选择&#x200B;**自定义**&#x200B;图标。
1. 选择&#x200B;**连接器**，然后选择&#x200B;**+**&#x200B;图标以添加连接器。
1. 选择&#x200B;**创建应用程序**&#x200B;按钮。
1. 为连接器指定所需的名称（如“Workfront”），然后输入所需的MCP服务器URL：

   | 区域 | URL |
   | --- | --- |
   | 美国 | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
   | 欧盟 | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |

1. 创建连接器后，会弹出登录窗口。 使用您的Adobe ID凭据进行身份验证。 如果您属于多个Workfront实例，请确保选择所需的AEM实例。

   >[!NOTE]
   >
   >您的Workfront实例必须与该实例所在地区的MCP服务器连接。 例如，EU实例必须连接到EU MCP服务器。
   >
   >选择实例时，与MCP服务器区域不兼容的实例将显示为灰色，您无法连接到它们。
   >
   >要连接到与MCP服务器的区域不兼容的实例，请为该区域设置一个具有正确URL的新MCP连接。

+++

### 使用技能自定义克劳德行为

[!DNL Claude]支持由用户创建的称为“技能”的说明集。 您可以使用技能自定义[!DNL Claude]在Workfront中的行为方式。 例如，您可以创建一项技能，告知[!DNL Claude]始终从Workfront中获取最新数据，而不是依赖以前的结果。

要了解有关[!DNL Claude]技能的更多信息，请参阅[Claude用户文档](https://code.claude.com/docs/en/skills)或向Claude寻求技能帮助。

## 连接到ChatGPT

1. 使用您的凭据登录到[ChatGPT](https://chatgpt.com)。
1. 在左下方，选择&#x200B;**您的姓名** → **设置**。
1. 选择&#x200B;**应用程序**，然后启用&#x200B;**开发人员模式**。
1. 选择&#x200B;**创建应用程序**&#x200B;按钮。
1. 为应用程序指定所需的名称（如“Workfront”），然后输入所需的MCP服务器URL：

   | 区域 | URL |
   | --- | --- |
   | 美国 | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
   | 欧盟 | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |

1. 确保身份验证设置为&#x200B;**OAuth**（默认设置），并选中接受复选框以继续。
1. 创建应用程序后，会弹出一个登录窗口。 使用您的Adobe ID凭据进行身份验证。 如果您属于多个Workfront实例，请确保选择所需的AEM实例。

   >[!NOTE]
   >
   >您的Workfront实例必须与该实例所在地区的MCP服务器连接。 例如，EU实例必须连接到EU MCP服务器。
   >
   >选择实例时，与MCP服务器区域不兼容的实例将显示为灰色，您无法连接到它们。
   >
   >要连接到与MCP服务器的区域不兼容的实例，请为该区域设置一个具有正确URL的新MCP连接。


### 使用自定义GPT自定义ChatGPT行为

ChatGPT支持用户创建的称为自定义GPT的助理。 您可以使用自定义GPT自定义ChatGPT与连接器的行为方式。 例如，您可以创建一个自定义GPT，告诉ChatGPT始终从连接的服务中获取最新数据，而不是依赖以前的结果。

要了解有关自定义GPT的更多信息，请参阅[ChatGPT用户文档](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts)或向ChatGPT寻求有关自定义GPT的帮助。

## 验证您的连接

要确认AI代理平台已连接到Workfront，请要求AI代理平台列出Workfront MCP服务器可执行的操作。 例如：

* *您可以执行哪些Workfront操作？*
* *列出您有权访问的Workfront工具。*

您还可以在[Adobe Workfront MCP服务器工具](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md)中查看完整的工具列表。

## 可用工具

Workfront MCP服务器公开由连接的AI代理平台代表您调用的一组工具 — 例如，用于搜索Workfront、创建项目、更新字段和管理审批的工具。 有关按Workfront区域分组的完整参考列表，请参阅[Adobe Workfront MCP服务器工具](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md)。

## 切换到其他Workfront实例

每个连接都向单个Workfront实例验证AI代理平台。 要使用其他实例，请断开并重新连接。

连接到其他Workfront实例：

1. 在AI代理平台中，断开Workfront MCP服务器的连接。
1. 重新连接连接器。
1. 对新的Workfront实例进行身份验证。

>[!NOTE]
>
>* 仅注销不会切换Workfront实例。 必须断开并重新连接连接器。
>
>* 您的Workfront实例必须与该实例所在地区的MCP服务器连接。 例如，EU实例必须连接到EU MCP服务器。
>
>   选择实例时，与MCP服务器区域不兼容的实例将显示为灰色，您无法连接到它们。
>
>   要连接到与MCP服务器的区域不兼容的实例，请为该区域设置一个具有正确URL的新MCP连接。


<!--

## Connect to Gemini

>[!IMPORTANT]
>
>You must be an administrator on the Gemini platform to set up the MCP server. If you aren't an administrator, share these instructions with your administrator so they can set up the connection for you.


To set up the connection between Gemini and the Workfront MCP server, follow the instructions provided by Google for [connecting Gemini to external tools using MCP](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/custom-mcp-server/set-up-custom-mcp-server). 

When prompted for the MCP Server URL, enter the following URL for your Workfront MCP server:  

   | Region | URL |
   | --- | --- |
   | US | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
   | EU | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |
   
-->

<!--
## Connect to Microsoft Copilot

✅ 1) Copilot Studio (most common for agents / enterprise use)
This is the cleanest "paste a URL" flow.
Steps
1. Open your Copilot Studio agent
2. Go to Tools
3. Click:
    * Add a tool → New tool → Model Context Protocol
4. In the wizard, fill in:
    * Server name (anything)
    * Server description
    * ✅ Server URL (your MCP endpoint)
5. Choose auth (if needed):
    * None / API key / OAuth
6. Click Create
👉 That's it—your MCP server is now attached to the agent.
This flow is explicitly documented:
* You add MCP via Tools → Add tool → Model Context Protocol
* Then provide Server name, description, and URL ￼
￼
What happens next
* Copilot discovers tools automatically from the MCP server
* You can enable/disable tools per agent
* The agent calls them when relevant

-->

## 设置和身份验证疑难解答

+++ 展开以查看有关Workfront MCP服务器的设置和身份验证的疑难解答提示。

| 问题 | 可能的原因 | 修复 |
| --- | --- | --- |
| 在[!DNL Claude]中找不到[!DNL Adobe Workfront]连接器。 | 您的[!DNL Claude]管理员尚未启用它。 | 请联系您的[!DNL Claude]管理员（而不是Workfront管理员），要求他们启用[!DNL Adobe Workfront]连接器。 |
| 您已连接，但看不到您的数据。 | 您使用了错误的Workfront实例进行身份验证。 | 断开连接器，重新连接并验证正确的实例。 |
| 身份验证失败，或连接停止工作。 | 您的身份验证会话已过期或存在连接错误。 | 断开并重新连接连接器。 |
| 您希望切换到其他Workfront实例。 | 单个连接会将您绑定到一个实例。 | 断开新实例的连接、重新连接并进行身份验证。 |
| 您无法连接到Workfront，或者您看到一条消息，表明MCP服务器访问被禁用。 | 您的Workfront管理员已关闭实例的MCP服务器访问。 | 请与Workfront管理员联系，要求他们在“系统首选项”中启用MCP服务器访问。 |
| 您要连接到的Workfront实例呈灰显状态，并且您会看到一条消息，指出在您的地区无法连接该实例 | 您的MCP服务器配置区域与实例不同（欧盟或美国）。 | 使用您的Workfront实例所分配到的区域的URL设置MCP服务器。 |
| AI代理平台可以找到您的Workfront项目，但无法创建、更新或删除它们。 | 您的Workfront管理员已禁用Workfront MCP服务器的写入操作。 | 联系Workfront管理员，要求他们在“系统首选项”中启用写入操作。 |

有关连接后的日常故障排除（例如，陈旧的结果或意外行为），请参阅[使用Adobe Workfront MCP服务器](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)。


+++

## 有关设置的常见问题解答

+++ 展开以查看有关设置Workfront MCP服务器的常见问题解答。

### 我是否可以同时连接到多个Workfront实例？

不可以。 每个连接都将AI代理平台绑定到单个Workfront实例。 要切换，请断开并重新连接，对新实例进行身份验证。

### 由哪个管理员启用此功能？

Workfront管理员和AI代理平台管理员。 您的Workfront管理员可以在Workfront端启用MCP服务器访问。 AI代理平台的管理员可在该平台上启用Workfront访问权限。 对于[!DNL Claude]，[!DNL Claude]企业管理员启用[!DNL Adobe Workfront]连接器。

### 如果未在Workfront Identity Management System (IMS)上启用我的Workfront实例，我能否使用Adobe MCP服务器？

不可以。 必须在Adobe Identity Management System (IMS)上启用Workfront实例，才能使用Workfront MCP服务器。 如果您不确定实例是否已在IMS中启用，请与Workfront管理员联系。

+++ 



