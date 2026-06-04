---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: 计算投资组合中净值的风险
description: 在Portfolio Optimizer中，[!UICONTROL 净值的风险]指示符将测量潜在风险，并考虑Portfolio Optimizer中显示的所有项目提供的净值。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
TQID: https://experienceleague.adobe.com/mClkaUv0y-Y9wiqg4oJivWYtmJDuKG701nOr5TU5rCA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c10f2e93-7a58-4212-aa24-684c265ebe76id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 178
ht-degree: 0%

---

# 计算投资组合中[!UICONTROL 净值风险]

在[!UICONTROL Portfolio Optimizer]中，[!UICONTROL 净值的风险]指示符将潜在风险计算在内，并考虑[!UICONTROL Portfolio Optimizer]中显示的所有项目提供的[!UICONTROL 净值]。

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
>[!UICONTROL 净值风险]指标根据您在[!UICONTROL Portfolio Optimizer]中显示的项目进行计算，而不是根据与该项目组合关联的所有项目进行计算。
