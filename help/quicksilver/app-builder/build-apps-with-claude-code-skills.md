---
title: 使用Claude代码技能构建App Builder应用程序
description: 通过描述您所需的内容，使用一组Claude代码技能构建自定义Adobe Workfront App Builder应用程序，而不是自己运行设置和部署步骤。
author: Becky
feature: Digital Content and Documents
hide: true
source-git-commit: 366cc4ffea48295b00389b5ee36f2df42b2c8a07
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 4%

---


# 使用Claude代码技能构建App Builder应用程序

技能包允许[!DNL Claude]（或任何支持克劳德格式技能的AI编码工具，如[!DNL Claude Code]或[!DNL OpenAI Codex]）为[!DNL Workfront]构建自定义[!DNL Adobe App Builder]应用程序。 如果您有权访问这些工具之一，则可以构建UI扩展，方法是以纯英语描述您想要的内容，而无需开发人员经验或手动设置步骤。

Workfront UI Extensions 由 Adobe App Builder 提供支持，允许客户和合作伙伴创建自定义的用户体验。 UI扩展允许您修改组织的Workfront体验，以更好地满足组织的需求，这些需求可以提高效率、提供无缝且相互关联的体验，并显着提升用户满意度，并帮助您的组织实现其独特愿景。

有关Workfront UI扩展的更多信息，请参阅[使用Adobe App Builder为Workfront创建自定义应用程序](/help/quicksilver/app-builder/app-builder.md)。

## UI可扩展性技能

利用UI扩展性技能，AI编码工具可以在Workfront中管理UI扩展的创建。 您描述了所需的功能，它完成实际操作，例如设置工具、在[!DNL Adobe App Builder]中创建项目、构建应用程序、将其部署到Adobe的云中，以及在Workfront中运行该应用程序。 只有在需要您执行操作的决策或登录时，您才会参与该过程。 本文使用[!DNL Claude]作为示例，但这些说明适用于任何支持Claude Skills的AI编码工具。

## 先决条件

在开始之前，请确保您拥有：

* **支持Claude Skills**&#x200B;的AI编码环境，如[!DNL Claude Code]。

  有关Claude Skills的详细信息，请参阅[什么是技能？](https://support.claude.com/en/articles/12512176-what-are-skills) 在克劳德文档中。

* **访问技能**。

  * 您可以在[https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md](https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md)中找到相关技能。

    如果未为您打开此链接，请要求您的管理员授予您访问权限。
  * 技能发布在Adobe的公共技能市场([adobe/skills](https://github.com/adobe/skills))中。 在[!DNL Claude Code]中，运行：

    ```
    /plugin marketplace add adobe/skills
    ```

    ```
    /plugin install app-builder@adobe-skills
    ```

* **[!DNL Adobe App Builder]访问权限，使用开发人员角色**。 您的Adobe组织需要App Builder许可证，并且您必须作为开发人员添加到该许可证中。 这是允许[!DNL Claude]打开Adobe Developer Console并创建项目的内容。

  要检查是否满足此先决条件，请执行以下操作：

  1. 打开 [Adobe Developer Console](https://developer.adobe.com/console)。
  1. 确认右上角显示的组织是否正确。
  1. 单击&#x200B;**新建项目** > **从模板创建项目**。
  1. 检查列表中是否显示&#x200B;**App Builder**。

     * 如果您在列表中看到&#x200B;**App Builder**，则表示您有权访问。
     * 如果没有&#x200B;**从模板创建项目**&#x200B;选项，或者没有&#x200B;**App Builder**&#x200B;选项，则您还没有访问权限。 要求您的Workfront或Adobe管理员将您添加为开发人员（在“Adobe Admin Console”>“用户”>“开发人员”中），并确认您的组织拥有App Builder许可证。
* **Workfront MCP服务器已连接**，因此[!DNL Claude]使用真正的Workfront API，而不是猜测数据类型、字段和命令。

  要检查Workfront MCP服务器是否已连接，请询问[!DNL Claude]： *“您能看到Workfront MCP资源吗？”*

  有关更多信息和说明，请参阅配置Workfront MCP服务器一文中的[将Adobe Workfront连接到Claude](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#connect-workfront-to-claude)。
