---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 运行方案得分专家
description: 管理 [!DNL Adobe Workfront Fusion]中的锁定方案
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: ed100c6ba32a6fbff6fa68ac7a4bfb38db861b17
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# 在Adobe Workfront Fusion中运行场景评分专家

场景评分专家可以帮助您确保按照最佳实践的方式配置场景。 它会检查您的方案并提供有关其结构和组织的建议。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]许可证**</td> 
  <td> <p>[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p><p>[！UICONTROL [!DNL Workfront Fusion]工作自动化] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

运行方案得分专家

1. 单击左侧面板中的&#x200B;**[!UICONTROL 方案]**&#x200B;选项卡。
1. 选择要运行方案评分专家的方案。
1. 单击方案上的任意位置以进入方案编辑器。
1. 单击屏幕底部附近的“场景评分专家”图标![场景评分专家](assets/scoring-expert-icon.png)。

   此时将打开“场景评分专家”面板。
1. 单击&#x200B;**评估**。

场景评分专家返回10分，并显示哪些检查通过或失败。 如果检查失败，场景评分专家会就如何确保场景满足这些检查提出建议。

![方案得分](assets/scenario-score.png)

## 场景评分检查

方案得分专家使用以下检查：

* 必须命名方案。
* 必须为所有模块设置标签。
* 方案必须按设定的计划运行。

  有关说明，请参阅[计划方案](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md)。
* 方案Blueprint大小必须小于5 MB。

  有关详细信息，请参阅[Fusion性能护栏](/help/quicksilver/workfront-fusion/get-started/fusion-performance-guardrails.md#scenarios)。
* 如果使用Workfront instant trigger模块，则必须对其进行筛选。

  有关说明，请参阅 [!DNL Workfront] > [!UICONTROL 观看活动]模块](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-module)中的[活动订阅筛选器。





