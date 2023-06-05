---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在中管理锁定的方案 [!DNL Adobe Workfront Fusion]
description: 在中管理锁定的方案 [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 014434dc-7548-42d1-bacd-89ddf627b647
source-git-commit: 9050684504f2335f5631f63978a9f65c25fd8d5f
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# 在中管理锁定的方案 [!DNL Adobe Workfront Fusion]

在某些情况下，场景可能会被暂时锁定 [!DNL Workfront Fusion]. 锁定的执行将在2-4小时内自动解锁。 您还可以手动解锁方案。

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
  <td> <p>[！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p><p>[！UICONTROL [!DNL Workfront Fusion] 工作自动化] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 了解锁定的方案

出于多种原因，方案可能会被锁定。

Workfront Fusion不支持并行处理计划场景。 这些方案将在方案执行开始时锁定，并在完成后解锁。 如果执行中断，场景可能无法解锁。 当用户手动强制停止场景或出现系统问题时，可能会发生这种情况。

此外，Workfront Fusion工程团队可能会锁定场景，因为它会导致性能或其他问题。

无论锁定场景的原因如何，该场景都将在锁定后2-4小时内自动解锁。

## 解锁锁定的方案

锁定的场景将从被锁定时起2-4小时解锁。 在计划自动解锁方案之前，您可以手动解锁该方案。

手动解锁场景可能会导致场景执行出错。 我们建议仅在场景由于设计场景时运行和停止执行而被锁定时手动解锁场景。 在其他情况下，我们建议您等待场景自动解锁。

>[!IMPORTANT]
>
>手动解锁场景可能会导致场景执行出错。

1. 转到锁定方案的“方案详细信息”页面。
1. 单击 **[!UICONTROL 选项]** 在屏幕右上角。
1. 选择 **[!UICONTROL 解锁执行]**.
1. 单击 **[!UICONTROL 解锁]**.
