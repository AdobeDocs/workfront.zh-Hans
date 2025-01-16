---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion场景概述
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]方案概述

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [方案概述](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/scenario-overview.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

>[!NOTE]
>
>除[!DNL Adobe Workfront license]外，[!DNL Adobe Workfront Fusion]还需要[!DNL Adobe Workfront Fusion]许可证。

>[!IMPORTANT]
>
>不应混淆[!DNL Workfront Fusion]方案与[!DNL Workfront Scenario Planner]方案。 有关[!DNL Workfront Scenario Planner]方案的信息，请参阅[概述 [!DNL Scenario Planner] ](../../scenario-planner/scenario-planner-overview.md)。

[!DNL Adobe Workfront Fusion]的作用是自动化您的流程，以便您能够专注于新任务，而不是重复相同的任务。 它的工作方式是，关联应用程序和服务内外的操作，从而创建一个自动传输和转换数据的方案。 您创建的方案会监视应用程序或服务中的数据，并对这些数据进行处理以提供您想要的结果。

场景由一系列模块组成，这些模块指示应如何在应用程序内转换数据或在应用程序和Web服务之间传输数据。

## 方案元素概述

场景由不同的元素构建。 了解这些元素的术语可使文档更易于使用。

### 方案

**方案**&#x200B;是用户创建的一系列自动步骤，创建这些步骤是为了移动和处理数据。 术语“场景”是指连接步骤的整个组。

![方案](assets/entire-scenario-scenario.png)

### 触发器

方案以&#x200B;**触发器**&#x200B;开头。 触发器会监视新的和更新的数据，并在模块中配置的某些条件适用时启动场景。 触发器可以配置为按计划启动方案（轮询），或者在发生数据更改时启动方案（即时）。

![触发器](assets/scenario-trigger.png)

### 模块

触发器后面跟有许多&#x200B;**模块**。 模块表示执行特定操作的方案中的单一步骤。 模块已配置并链接在一起，以创建方案。

![模块](assets/scenario-module.png)

### 路由

方案可分为&#x200B;**个路由**。 路由是场景的一部分，不一定用于给定的数据捆绑。 路由是使用路由器模块和过滤器设置的。

![路由](assets/scenario-route.png)

### 方案区段

方案区段是方案的一部分，由一系列连接到同一应用程序的连续模块组成。 场景区段通常表示应用程序中的简短工作流。

![方案区段](assets/scenario-segment.png)

### 连接器

连接器是给定应用程序的一组模块。 Workfront Fusion提供了用于许多常见工作应用程序(如Workfront、Salesforce和Jira)的连接器，以及可用于任何Web服务的通用连接器。

![连接器](assets/scenario-connectors.png)



## 示例：在[!DNL Adobe Workfront]中自动化进程

>[!NOTE]
>
>此功能适用于以下许可证：
>
>* 工作自动化的[!UICONTROL [!DNL Workfront Fusion]]
>* 用于工作自动化和集成的[!UICONTROL [!DNL Workfront Fusion]]

通过[!DNL Workfront Fusion]，您可以在[!DNL Workfront]中自动执行简单或复杂的工作流，从而节省时间并确保始终如一地执行该流程。

在此示例中，当在[!DNL Workfront]中的任务或问题中的指定字段发生更改时，将触发该方案。 触发时，场景获取相关项目中的信息，并为分配给项目上特定角色的人员创建量身定制的更新。

![](assets/fusion-template-example-350x102.png)

## 示例：正在将[!DNL Workfront]连接到另一个应用或Web服务

>[!NOTE]
>
>此功能适用于以下许可证：
>
>* 用于工作自动化和集成的[!UICONTROL [!DNL Workfront Fusion]]
>

[!DNL Workfront Fusion]还可以连接到其他应用和Web服务。 您可以从其他应用程序访问、导入、处理或导出数据，并将它们与Workfront集成或相互集成。 许多应用程序都有专用的[!DNL Workfront Fusion]连接器。 如果您要访问的应用程序没有专用连接器，则可以使用[!DNL Workfront Fusion]的[!UICONTROL HTTP]或[!UICONTROL SOAP]模块通过应用程序的API连接到该应用程序。

在此示例中，将用户添加到[!DNL Excel]电子表格时会触发该方案。 方案检查用户是否在[!DNL Workfront]中。 如果不存在，则方案将在[!DNL Workfront]中创建用户，并将其Workfront用户ID添加回电子表格。

![](assets/fusion-integration-example--350x171.png)

有关专用连接器的列表，请参阅[应用及其模块](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md)。

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion]可以连接到几乎任何Web服务。 如果要使用的应用程序没有专用的[!DNL Workfront Fusion]连接器，则可以使用以下模块直接连接到Web服务：
>
>* [[!UICONTROL HTTP]模块](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* [[!UICONTROL SOAP]模块](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON]模块](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>
