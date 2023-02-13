---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: 计算组合中的风险对净值
description: 在Portfolio优化器中， [!UICONTROL 净值风险] 指标衡量潜在风险时，会考虑Portfolio优化器中显示的所有项目提供的净值。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# 计算 [!UICONTROL 净值风险] 组合中

在 [!UICONTROL Portfolio优化程序], [!UICONTROL 净值风险] 指标衡量潜在风险，并考虑 [!UICONTROL 净值] 中显示的所有项目提供的 [!UICONTROL Portfolio优化程序]. 

为了在产品组合中实现最高效，您希望看到 [!UICONTROL 风险] 指示器低且 [!UICONTROL 净值] 指标很高。 

的 [!UICONTROL 风险] 和 [!UICONTROL 净值] 指标是从彼此关系的角度来表示的。

[!DNL Adobe Workfront] 计算 [!UICONTROL 风险] 和 [!UICONTROL 净值] 指标使用以下公式：

* 的 [!UICONTROL 风险] 指标通过以下公式计算：

   ```
   Risk indicator = Risk / (Risk + Net Value)
   ```

* 的 [!DNL Net Value] 指标由以下公式计算：

   ```
   Net Value indicator = 1 - Risk / (Risk + Net Value)
   ```

   或

   ```
   Net Value indicator = Net Value / (Risk + Net Value)
   ```

>[!NOTE]
>
>的 [!UICONTROL 净值风险] 指示器会根据您在 [!UICONTROL Portfolio优化程序]，而不是与项目组合关联的所有项目上。 
