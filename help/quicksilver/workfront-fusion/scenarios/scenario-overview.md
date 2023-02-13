---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion方案概述
description: Adobe Workfront Fusion除了需要Adobe Workfront许可证之外，还需要Adobe Workfront Fusion许可证。
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 方案概述

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 需要 [!DNL Adobe Workfront Fusion] 除 [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>[!DNL Workfront Fusion] 不应将情景与 [!DNL Workfront Scenario Planner] 方案。 有关 [!DNL Workfront Scenario Planner] 方案，请参阅 [的 [!DNL Scenario Planner] 概述](../../scenario-planner/scenario-planner-overview.md).

的角色 [!DNL Adobe Workfront Fusion] 是自动执行您的流程，以便您能够专注于新任务，而不是一遍又一遍地重复相同的任务。 它可以通过在应用程序和服务内部以及之间链接操作来工作，从而创建一种可自动传输和转换数据的方案。 您创建的方案会监控应用程序或服务中的数据，并处理该数据以提供所需的结果。

方案由一系列模块组成，这些模块指示数据应如何在应用程序内进行转换或在应用程序和Web服务之间进行传输。

## 示例：在 [!DNL Adobe Workfront]

>[!NOTE]
>
>此功能适用于以下许可证：
>
>* [!UICONTROL [!DNL Workfront Fusion] 工作自动化]
>* [!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成）]
>


[!DNL Workfront Fusion] 使您能够在 [!DNL Workfront]，可节省时间并确保流程始终如一地执行。

在此示例中，当任务或问题中的指定字段发生更改时，将触发方案 [!DNL Workfront]. 触发该方案时，将获取相关项目中的信息，并为分配给项目上特定角色的人员创建量身定制的更新。

![](assets/fusion-template-example-350x102.png)

## 示例：连接 [!DNL Workfront] 到其他应用程序或web服务

>[!NOTE]
>
>此功能适用于以下许可证：
>
>* [!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成）]
>


[!DNL Workfront Fusion] 还可以连接到其他应用程序和web服务。 您可以从其他应用程序访问、导入、处理或导出数据，并将它们与Workfront集成或相互集成。 许多应用程序都有专用 [!DNL Workfront Fusion] 连接器。 如果您要访问的应用程序没有专用连接器，则可以使用 [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] 或 [!UICONTROL SOAP] 模块通过其API连接到应用程序。

在此示例中，当用户添加到 [!DNL Excel] 电子表格。 方案会检查用户是否在 [!DNL Workfront]. 如果没有，则方案将在 [!DNL Workfront] 并将其Workfront用户ID重新添加到电子表格中。

![](assets/fusion-integration-example--350x171.png)

有关专用连接器的列表，请参阅 [应用程序及其模块](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] 几乎可以连接到任何web服务。 如果要使用的应用程序没有专用 [!DNL Workfront Fusion] 连接器中，您可以使用以下模块直接连接到web服务：
>
>* [[!UICONTROL HTTP] 模块](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* [[!UICONTROL SOAP] 模块](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON] 模块](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>

