---
content-type: reference
product-area: workfront-integrations
keywords: 原生，ootb
navigation-topic: workfront-integrations-navigation-topic
title: Adobe Workfront集成方法
description: 您可以集成 [!DNL Adobe Workfront] 第三方应用程序。 这些集成可以扩展 [!DNL Workfront] 并根据贵组织的需求量身定制。 您可以使用任何或所有这些集成，具体取决于哪些集成对给定任务最有用。
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 685186f76cd89e69eac0a07bff9a39e2e28f9429
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 0%

---

# Adobe Workfront集成方法

您可以集成 [!DNL Adobe Workfront] 第三方应用程序。 这些集成可以扩展 [!DNL Workfront] 并根据贵组织的需求量身定制。 您可以使用任何或所有这些集成，具体取决于哪些集成对给定任务最有用。

## 内置集成

Workfront提供了各种集成，您可以直接从Workfront或其他应用程序中配置这些集成，方法是安装该应用程序的Workfront加载项。 这些内置集成涵盖许多常见的用例情景，并着重于扩展和连接最终用户的用户体验。

Workfront内置集成主要侧重于个人工作效率和协作。 这些集成可减少单个用户工作流程的中断，从而让他们能够接收Workfront通知、访问信息并对Workfront工作项执行操作，而无需离开集成的应用程序。

内置集成的优势可能包括：

* 其中许多内置集成可免费使用。 （其他客户确实需要额外购买。）
* 内置集成涵盖企业使用的许多最常见应用程序，如Slack、 [!DNL Google Drive]，或Adobe产品，例如 [!DNL Adobe Creative Cloud] 或 [!DNL Adobe Experience Manager] 资产。 如果您的公司已经使用这些应用程序，则集成将顺利地进入用户的现有工作流程。
* 集成 [!DNL Workfront] 使用常用的应用程序可以提高用户的采用率。

>[!INFO]
>
>**示例:**
>
>使用 [!DNL Workfront for Microsoft integration]，您可以在 [!DNL Microsoft Teams] 关于 [!DNL Workfront] 工作项。 不离开 [!DNL Microsoft Teams]，则可以执行批准、注释或更改工作项状态等操作。 您对 [!DNL Microsoft] 团队会反映在 [!DNL Workfront] 也是。

有关内置集成的更多信息（包括当前可用的内置集成列表），请参阅 [[!DNL Adobe Workfront] 内置集成概述](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## 自定义OAuth2应用程序

Adobe [!DNL Workfront] 管理员可以为实例创建OAuth2应用程序 [!DNL Workfront]，允许其他应用程序访问Workfront。 然后，您的用户可以授予其他应用程序访问其Workfront数据的权限。 这样，您就可以将Workfront与您选择的应用程序集成，包括您自己的内部应用程序。

>[!NOTE]
>
>在OAuth2的上下文中，“创建应用程序”是指在应用程序和服务器(如Workfront)之间创建此类访问链接的过程。

创建 [!UICONTROL OAuth2] 申请可能包括：

* 用户可以在 [!DNL Workfront]，与内置集成类似。
* 设置或使用 [!UICONTROL OAuth2] 应用程序不需要其他技术知识，例如熟悉 [!DNL Workfront] API。
* 贵组织可能使用未作为 [!DNL Workfront] 内置应用程序。 您仍可以将此软件与 [!DNL Workfront] 使用 [!UICONTROL OAuth2] 应用程序，即使该软件是贵组织的专有软件。

有关更多信息，请参阅 [为Workfront集成创建OAuth2应用程序](../administration-and-setup/configure-integrations/create-oauth-application.md).

## Workfront API

Workfront提供了公共API（应用程序编程接口），可让您扩展和增强Workfront体验。 Workfront API的目标是通过引入通过HTTP运行的REST风格架构，简化您自己与Workfront的集成构建。 Workfront API确实需要一些技术知识，但它是一款用于检索、创建和修改数据的非常强大的工具。 您可以自定义API调用以执行非常具体的功能。

此外， [!DNL Workfront] 提供了事件订阅API。 在 [!DNL Workfront] 事件订阅支持的对象，您可以配置 [!DNL Workfront] 向所需的端点发送响应。 这意味着第三方应用程序可以从接收更新 [!DNL Workfront] 通过 [!DNL Workfront] API发生后不久。

使用 [!DNL Workfront] API可能包括以下内容：

* 您可以使用 [!DNL Workfront] 用于连接到几乎任何其他提供公共API的Web服务或应用程序的API。 因此，可以集成 [!DNL Workfront] 几乎所有您想要使用的web服务或应用程序。
* 的 [!DNL Workfront] API的灵活性也延伸到您企业的专有软件。 您可以使用和修改 [!DNL Workfront] 来自您自己软件的数据。
* 由于API在软件中非常常见，因此您的内部开发人员可能非常熟悉它们。 [!DNL Workfront] 使用REST风格的API（最常用的API类型），从而更加便于开发人员快速掌握。

>[!INFO]
>
>**示例:**
>
>以下API调用会使用指定的ID向任务的更新流中添加注释。
>
>
```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

有关 [!DNL Workfront] API，请参阅 [API基础知识](../wf-api/general/api-basics.md).

有关事件订阅的更多信息，请参阅 [事件订阅API](../wf-api/general/event-subs-api.md).

## Adobe Workfront Fusion

Workfront Fusion允许您自动执行工作流。 使用 [!DNL Workfront Fusion for Work Automation and Integration] 许可证，您可以跨多个应用程序和web服务创建这些自动化，从而创建应用程序协同工作以执行任务的情景。 方案是使用模块构建的任务或工作流的可视表示形式，模块是离散任务，如“下载文档”或“创建项目”。 您将模块链在一起以定义工作流，然后在满足触发条件时自动执行工作流。

优势 [!DNL Workfront Fusion] 可能包括：

* Workfront Fusion不像API那么需要技术知识，因为可视化界面有助于了解和设置工作流。 这意味着开发团队以外的个人可以使用它，这可以节省您的组织时间和资金。
* 自 [!DNL Workfront Fusion] 它通过API工作，可以访问大多数应用程序和Web服务。 许多应用程序都具有用于进行API调用的模块，或者您可以使用HTTP、SOAP或JSON模块与没有专用Web服务的Web服务进行交互 [!DNL Workfront Fusion] 连接器。

>[!INFO]
>
>**示例:**
>
>以下 [!DNL Workfront] 模块 [!DNL Workfront Fusion] 设置为向选定项目添加评论。 执行模块后，该注释将显示在Workfront中项目的更新流中。
>
>![](assets/fusion-example-comment-350x416.png)

有关Workfront Fusion的更多信息，请参阅 [Adobe Workfront Fusion](../workfront-fusion/workfront-fusion-2.md).
