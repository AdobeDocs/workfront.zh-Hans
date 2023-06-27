---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion中的操作
description: Adobe Workfront Fusion中的操作是由模块执行的任务。 出于跟踪目的，模块执行的任何成功操作都是操作。
author: Becky
feature: Workfront Fusion
source-git-commit: 8d82fd10a6742f13f62b5479fafa5b42e567700f
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# 中的操作 [!DNL Adobe Workfront Fusion]

中的操作 [!DNL Adobe Workfront Fusion] 是由模块执行的任务。 出于跟踪目的，模块执行的任何成功操作都是操作。

## 计算操作数时的注意事项

* 通常，任何成功的操作步骤执行都被视为操作。

* 场景中的第一个模块仅运行一次，并始终计为一个操作，即使它不返回捆绑包。

* 其余模块的运行次数取决于它们必须处理的捆绑包数量。  针对一个捆绑包运行一个模块即为一个操作。 聚合器模块是一个例外，该模块被计为每组正在处理的捆绑包中的一个操作。

* 操作计数在 [!UICONTROL 最终完成] 场景执行阶段。

* 以下是 **非** 计为操作：

   * 任何筛选步骤。

   * 出错或停止的任何操作。

   * 因不符合路由规则而不运行的任何路由，例如回退或禁用的路由。

   * 未运行的任何操作，可能是因为过滤器不允许数据通过，也可能是因为场景由于错误而停止。

## 操作限制

贵组织可能有每月运营限制。 这是基于 [!DNL Workfront] 计划贵组织购买的计划。 此 [!UICONTROL Ultimate] [!DNL Workfront] 计划提供无限的操作。

如果您的组织存在每月限制，则会在接近限制时通知您。 如果你超过限制， [!DNL Workfront] 将与贵组织联系，确保您的计划满足您的需求。

## 查看过去30天内执行的操作数

您可以看到一个图形，其中显示了执行的操作数。 这些图表在以下位置提供：

* **组织信息板**：整个组织使用的操作
* **团队信息板**：此团队拥有的方案使用的操作([!DNL Adobe Experience Cloud] 仅限)
* **“方案详细信息”页面**：此方案使用的操作([!DNL Adobe Experience Cloud] 仅限)

