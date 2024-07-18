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
source-git-commit: c325e16ba0cde4cd48fc3e40358a9ea9ed310659
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion]中的数学函数

<!--Audited: 4/2024-->

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td>  
   <td> <p>任何</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td>  
   <td> <p>新文档： [！UICONTROL Standard]</p><p>或</p><p>当前： [！UICONTROL Work]或更高版本</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td>  
   <td> 
   <p>当前：无[!DNL Workfront Fusion]许可证要求。</p> 
   <p>或</p> 
   <p>旧版：任意 </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">产品</td>  
   <td> 
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront]计划：您的组织必须购买[!DNL Adobe Workfront Fusion]。</li><li>已包括[！UICONTROL Ultimate] [!DNL Workfront]计划： [!DNL Workfront Fusion]。</li></ul> 
   <p>或</p> 
   <p>当前：您的组织必须购买[!DNL Adobe Workfront Fusion]。</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## [!UICONTROL 平均值（[个值数组]）平均值(value1； [value2]， ...)]

返回特定数组中数值的平均值，或单独输入的数值的平均值。

## [!UICONTROL ceil （数字）]

返回大于或等于指定数字的最小整数。

>[!INFO]
>
>**示例：**
>
>* `ceil(` `1.2` `)`
>
>   返回2
>
>* `ceil(` `4` `)`
>
>   返回4

## [!UICONTROL 楼层（数字）]

返回小于或等于指定数字的最大整数。

>[!INFO]
>
>**示例：**
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

## [!UICONTROL 最大值（[个值数组]），最大值(value1；value2； ...)]

返回指定数组中的最大数或单独输入的数字中的最大数。

## [!UICONTROL 分钟（[个值数组]），最小值(value1； value2； ...)]

返回指定数组中的最小数字或单独输入数字中的最小数字。

## [!UICONTROL 轮（数字）]

将数值舍入到最接近的整数。

>[!INFO]
>
>**示例：**
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

## [!UICONTROL sum （[个值数组]）， sum(value1； value2； ...)]

返回指定数组中的值的总和或单独输入的数字的总和。

## [!UICONTROL parseNumber （数字；小数分隔符）]

解析带有数字的字符串并返回数字。 例如， parseNumber(1 756,456；，)

## [!UICONTROL formatNumber (number； decimalPOINTS； [decimalSeparator]；[thousandsSeparator])]

以请求的格式返回一个数字。 默认情况下，小数点为逗号(，)，千位分隔符为句点(.)。

>[!INFO]
>
>**示例：**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>返回123.456.789,000
