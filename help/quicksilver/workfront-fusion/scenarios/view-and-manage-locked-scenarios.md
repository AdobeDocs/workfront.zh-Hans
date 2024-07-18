---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 管理 [!DNL Adobe Workfront Fusion]中的锁定方案
description: 管理 [!DNL Adobe Workfront Fusion]中的锁定方案
author: Becky
feature: Workfront Fusion
exl-id: 5fccf336-d904-43fe-ad4a-c3ce76dbcad0
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中管理锁定的方案

在某些情况下，某个方案可能会暂时锁定在[!DNL Workfront Fusion]中。 锁定的执行将在2-4小时内自动解锁。 您还可以手动解锁方案。

>[!IMPORTANT]
>
>手动解锁场景可能会导致场景执行出错。

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

## 了解锁定方案

出于多种原因，可能会锁定方案。

Workfront Fusion不支持并行处理计划场景。 这些方案在方案执行开始时会被锁定，在完成时会被解锁。 如果执行中断，场景可能无法解锁。 当用户手动强制停止场景或出现系统问题时，可能会发生这种情况。

此外，Workfront Fusion工程团队可能会锁定场景，因为它会导致性能或其他问题。

无论导致锁定方案的原因如何，该方案都将在锁定2-4小时后自动解锁。

## 解锁锁定的方案

锁定的方案将从锁定的时间起2 - 4小时解锁。 您可以在计划自动解锁方案之前手动解锁该方案。

手动解锁场景可能会导致场景执行出错。 我们建议仅在场景由于设计场景时运行和停止执行而被锁定时，手动解锁场景。 在其他情况下，我们建议您等待场景自动解锁。

>[!IMPORTANT]
>
>手动解锁场景可能会导致场景执行出错。

1. 转至锁定方案的“方案详细信息”页面。
1. 单击屏幕右上角的&#x200B;**[!UICONTROL 选项]**。
1. 选择&#x200B;**[!UICONTROL 解锁执行]**。
1. 单击&#x200B;**[!UICONTROL 解锁]**。
