---
content-type: reference
product-area: workfront-integrations
keywords: 原生，ootb
navigation-topic: workfront-integrations-navigation-topic
title: Adobe Workfront集成方法
description: 您可以将 [!DNL Adobe Workfront] 与第三方应用程序集成。 这些集成可以扩展 [!DNL Workfront] 的实用工具，并根据贵组织的需求对其进行定制。 您可以使用任意或所有这些集成，具体取决于哪一种集成对给定任务最有用。
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# Adobe Workfront集成方法

您可以将[!DNL Adobe Workfront]与第三方应用程序及其他[!DNL Adobe]产品集成。 这些集成可以扩展[!DNL Workfront]的实用工具，并根据贵组织的需求对其进行定制。 您可以使用任意或所有这些集成，具体取决于哪一种集成对给定任务最有用。

## 内置集成

Workfront提供了多种集成，您可以直接从Workfront配置这些集成，也可以通过安装其他应用程序的Workfront加载项从其他应用程序配置这些集成。 这些内置集成涵盖许多常见用例情景，并侧重于为最终用户扩展和连接用户体验。

Workfront内置的集成主要侧重于个人工作效率和协作。 这些集成减少了单个用户工作流中的中断，使他们能够接收Workfront通知、访问信息并处理Workfront工作项，而无需离开集成应用程序。

内置集成的优点可能包括：

* 其中许多内置集成均可免费使用。 （其他客户则确实需要额外购买。）
* 内置集成涵盖许多企业最常用的应用程序，如[!DNL Slack]、[!DNL Google Drive]或[!DNL Adobe]产品，如[!DNL Adobe Creative Cloud]或[!DNL Adobe Experience Manager]Assets。 如果贵公司已使用这些应用程序，则集成将会顺利进入您用户的现有工作流程。
* 将[!DNL Workfront]与常用应用程序集成可以提高用户的采用率。

>[!INFO]
>
>**示例：**
>
>使用[!DNL Workfront for Microsoft Teams integration]，您可以在[!DNL Microsoft Teams]中接收有关您的[!DNL Workfront]工作项的通知。 在不离开[!DNL Microsoft Teams]的情况下，您可以执行批准、评论或更改工作项状态等操作。 您对[!DNL Microsoft Teams]中的工作项所做的任何更改也反映在[!DNL Workfront]中。

有关内置集成的更多信息，包括当前可用的内置集成列表，请参阅[[!DNL Adobe Workfront] 内置集成概述](../workfront-integrations-and-apps/built-in-integrations-non-admin.md)。

## 自定义OAuth2应用程序

Adobe[!DNL Workfront]管理员可以为您的[!DNL Workfront]实例创建OAuth2应用程序，这将允许其他应用程序访问[!DNL Workfront]。 然后，您的用户可以授予这些其他应用程序访问其[!DNL Workfront]数据的权限。 这样，您就可以将Workfront与您选择的应用程序（包括您自己的内部应用程序）集成。

>[!NOTE]
>
>在OAuth2的上下文中，“创建应用程序”是指在应用程序和服务器(例如Workfront)之间创建此类访问链接的过程。

创建[!UICONTROL OAuth2]应用程序的优点可能包括：

* 用户可以直接在[!DNL Workfront]中使用这些集成，这与内置集成类似。
* 设置或使用[!UICONTROL OAuth2]应用程序不需要其他技术知识，例如熟悉[!DNL Workfront] API。
* 您的组织可以使用未作为[!DNL Workfront]内置应用程序提供的软件。 您仍然可以使用[!UICONTROL OAuth2]应用程序将此软件与[!DNL Workfront]集成，即使此软件是您组织的专有软件。

有关详细信息，请参阅[为Workfront集成创建OAuth2应用程序](../administration-and-setup/configure-integrations/create-oauth-application.md)。

## [!DNL Workfront] API

[!DNL Workfront]提供了一个公共API（应用程序编程接口），通过该接口，您可以扩展和增强您的Workfront体验。 [!DNL Workfront] API的目标是通过引入通过HTTP运行的REST-ful架构来简化您与[!DNL Workfront]的集成。 [!DNL Workfront] API确实需要一些技术知识，但它是一个功能非常强大的工具，可用于检索、创建和修改数据。 您可以自定义API调用以执行非常特定的功能。

此外，[!DNL Workfront]还提供事件订阅API。 当事件订阅支持的[!DNL Workfront]对象上发生操作时，您可以将[!DNL Workfront]配置为将响应发送到所需的端点。 这意味着第三方应用程序在更新发生后不久即可通过[!DNL Workfront] API从[!DNL Workfront]交互中接收更新。

使用[!DNL Workfront] API的优点可能包括：

* 您可以使用[!DNL Workfront] API连接到几乎任何提供公共API的其他Web服务或应用程序。 因此，可以将[!DNL Workfront]与您要使用的几乎任何Web服务或应用程序集成。
* [!DNL Workfront] API的灵活性还扩展到您企业的专有软件。 您可以从自己的软件中使用和修改[!DNL Workfront]数据。
* 由于API对于软件来说非常常见，因此您的内部开发人员可能很熟悉它们。 [!DNL Workfront]使用REST-ful API（最常见的API类型），使开发人员更容易快速上手。

>[!INFO]
>
>**示例：**
>
>以下API调用将注释放入具有指定ID的任务的更新流中。
>
>```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

有关[!DNL Workfront] API的详细信息，请参阅[API基础知识](../wf-api/general/api-basics.md)。

有关事件订阅的详细信息，请参阅[事件订阅API](../wf-api/general/event-subs-api.md)。

## [!DNL Adobe Workfront Fusion]

[!DNL Workfront Fusion]允许您自动执行工作流。 使用[!DNL Workfront Fusion for Work Automation and Integration]许可证，您可以跨多个应用程序和Web服务创建这些自动化，从而创建应用程序协作以执行任务的方案。 场景是使用模块构建的任务或工作流的可视表示形式，这些模块是离散任务，如“下载文档”或“创建项目”。 您可以将多个模块链接在一起以定义工作流，然后在满足触发条件时自动执行工作流。

[!DNL Workfront Fusion]的优点可能包括：

* [!DNL Workfront Fusion]不需要像API那样多的技术知识，因为可视化界面有助于了解和设置工作流。 这意味着开发团队以外的个人可以使用此功能，这可能会节省您的组织时间和资金。
* 由于[!DNL Workfront Fusion]通过API工作，因此它可以访问大多数应用和Web服务。 许多应用程序都拥有用于进行API调用的模块，或者您可以使用HTTP、SOAP或JSON模块与没有专用[!DNL Workfront Fusion]连接器的Web服务进行交互。

>[!INFO]
>
>**示例：**
>
>[!DNL Workfront Fusion]中的以下[!DNL Workfront]模块设置为向所选项目添加评论。 执行模块后，该注释将显示在Workfront中的项目更新流中。
>
>![示例：在Fusion中添加注释](assets/fusion-example-comment-350x416.png)

有关[!DNL Workfront Fusion]的详细信息，请参阅[[!DNL Adobe Workfront Fusion]](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/home)。
