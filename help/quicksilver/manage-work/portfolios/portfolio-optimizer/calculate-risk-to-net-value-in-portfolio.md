---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: 计算投资组合中净值的风险
description: 在Portfolio优化程序中，[!UICONTROL 净值的风险]指示符将测量潜在风险，并考虑Portfolio优化程序中显示的所有项目提供的净值。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# 计算投资组合中[!UICONTROL 净值风险]

在[!UICONTROL Portfolio优化器]中，[!UICONTROL 净值的风险]指示符将潜在风险考虑在内[!UICONTROL Portfolio优化器]中显示的所有项目提供的[!UICONTROL 净值]。 

为了在投资组合中实现最高效率，您想要看到[!UICONTROL 风险]指标低，[!UICONTROL 净值]指标高。 

[!UICONTROL 风险]和[!UICONTROL 净值]指标是从它们相互关系的角度表示的。

[!DNL Adobe Workfront]使用以下公式计算[!UICONTROL 风险]和[!UICONTROL 净值]指标：

* [!UICONTROL 风险]指标按以下公式计算：

  ```
  Risk indicator = Risk / (Risk + Net Value)
  ```

* [!DNL Net Value]指标按以下公式计算：

  ```
  Net Value indicator = 1 - Risk / (Risk + Net Value)
  ```

  或

  ```
  Net Value indicator = Net Value / (Risk + Net Value)
  ```

>[!NOTE]
>
>[!UICONTROL 净值风险]指标根据您在[!UICONTROL Portfolio优化器]中显示的项目进行计算，而不是根据与该项目组合关联的所有项目进行计算。 
