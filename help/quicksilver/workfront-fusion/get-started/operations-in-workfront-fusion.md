---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion中的操作
description: Adobe Workfront Fusion中的操作是由模块执行的任务。 出于跟踪目的，模块执行的任何成功操作都属于操作。
author: Becky
feature: Workfront Fusion
exl-id: 34268fb6-e485-42be-b751-3ee79bbf5797
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的操作

[!DNL Adobe Workfront Fusion]中的操作是由模块执行的任务。 出于跟踪目的，模块执行的任何成功操作都属于操作。

## 计算操作数时的注意事项

* 通常，任何成功的操作步骤执行都被视为操作。

* 场景中的第一个模块仅运行一次，并始终计为一个操作，即使它不返回捆绑包。

* 其余模块运行的次数取决于它们必须处理的捆绑包数量。  针对一个捆绑包运行一个模块即是一种操作。 聚合器模块例外，该模块被计为每组正在处理的捆绑包进行一次操作。

* 在方案执行的[!UICONTROL 最终化]阶段计算操作。

* 以下&#x200B;**不计算为操作**：

   * 任何过滤步骤。

   * 任何出错或中断的操作。

   * 任何因不符合路由规则而不运行的路由，例如回退或禁用的路由。

   * 任何未运行的操作，可能是因为过滤器不允许数据通过，也可能是因为场景因错误而停止。

## 操作限制

您的组织可能具有每月运营限制。 此计划基于贵组织购买的[!DNL Workfront]计划。 [!UICONTROL Ultimate] [!DNL Workfront]计划提供无限量的操作。

如果您的组织存在每月限制，则会在接近限制时通知您。 如果超出限制，[!DNL Workfront]将联系您的组织，以确保您的计划满足您的需求。

## 查看过去30天内执行的操作数

您可以看到一个图形，其中显示了执行的操作数。 这些图形在以下位置提供：

* **组织仪表板**：整个组织使用的操作
* **团队仪表板**：此团队拥有的方案使用的操作（仅限[!DNL Adobe Experience Cloud]）
* **方案详细信息页面**：此方案使用的操作（仅限[!DNL Adobe Experience Cloud]）
