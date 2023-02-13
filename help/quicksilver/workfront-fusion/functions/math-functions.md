---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront融合中的数学函数
description: 以下数学函数在Adobe Workfront Fusion映射面板中可用。
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 1%

---

# 中的数学函数 [!DNL Adobe Workfront Fusion]

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

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
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 平均值([值数组])average(value1; [value2], ...)]

返回特定数组中数值的平均值或单独输入数值的平均值。

## [!UICONTROL ceil（数字）]

返回大于或等于指定数字的最小整数。

>[!INFO]
>
>**示例:**
>
>* `ceil(` `1.2` `)`
   >
   >   返回2
>
>* `ceil(` `4` `)`
   >
   >   返回4


## [!UICONTROL floor(number)]

返回小于或等于指定数字的最大整数。

>[!INFO]
>
>**示例:**
>
>* `floor(` `1.2` `)`
   >
   >   返回1
>
>* `floor(` `1.9` `)`
   >
   >   返回1
>
>* `floor(` `4` `)`
   >
   >   返回4


## [!UICONTROL formatNumber(number;decimalPOINTS; [decimalSeparator]; [千位分隔符])]

以请求的格式返回数字。 默认情况下，小数点为逗号(,)，千位分隔符为句点(.)。

>[!INFO]
>
>**示例:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>返回123.456.789,000

## [!UICONTROL 最大值([值数组]), max(value1;value2;...)]

返回指定数组中的最大数或单独输入的数字中的最大数。

## [!UICONTROL 最小([值数组]), min(value1;value2;...)]

返回指定数组中的最小数字或单独输入的数字中的最小数字。

## [!UICONTROL parseNumber(number;小数分隔符]

解析带有数字的字符串并返回该数字。 例如， parseNumber(1 756,456;,)

## [!UICONTROL 轮次（数字）]

将数值四舍五入为最接近的整数。

>[!INFO]
>
>**示例:**
>
>* `round(` `1.2` `)`
   >
   >   返回1
>
>* `round(` `1.5` `)`
   >
   >   返回2
>
>* `round(` `1.7` `)`
   >
   >   返回2
> 
>* `round(` `2` `)`
   >
   >   返回2


## [!UICONTROL 总和([值数组]), sum(value1;value2;...)]

返回指定数组中值的总和或单独输入的数字的总和。
