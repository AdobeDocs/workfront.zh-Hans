---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion中的数学函数
description: Adobe Workfront Fusion映射面板中提供了以下数学函数。
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 2%

---

# 中的数学函数 [!DNL Adobe Workfront Fusion]

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
   <td>
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 平均([值数组])平均值(值1； [value2]， ...)]

返回特定数组中的数值的平均值，或单独输入的数值的平均值。

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

## [!UICONTROL floor（数字）]

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

## [!UICONTROL formatNumber (数字；decimalPOINTS； [decimalSeparator]； [千位分隔符])]

以请求的格式返回一个数字。 默认情况下，小数点为逗号(，)，千位分隔符为句点(.)。

>[!INFO]
>
>**示例:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>返回123.456.789,000

## [!UICONTROL 最大值([值数组])， max(value1；value2； ...)]

返回指定数组中的最大数字或单独输入的数字中的最大数字。

## [!UICONTROL 分钟([值数组])， min(value1； value2； ...)]

返回指定数组中的最小数字或单独输入的数字中的最小数字。

## [!UICONTROL parseNumber （数字；小数分隔符）]

解析带有数字的字符串并返回数字。 例如，parseNumber(1 756,456；，)

## [!UICONTROL round（数字）]

将数值四舍五入到最接近的整数。

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

## [!UICONTROL sum ([值数组])、sum(value1； value2； ...)]

返回指定数组中的值的总和或单独输入的数字的总和。
