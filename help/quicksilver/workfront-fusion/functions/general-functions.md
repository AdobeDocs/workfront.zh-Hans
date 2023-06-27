---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion中的常规函数
description: Adobe Workfront Fusion映射面板中提供了以下常规函数。
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 3%

---

# 中的常规函数 [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL get（对象或数组；路径）]

返回对象或数组的值路径。 要访问嵌套对象，请使用点表示法。 数组中的第一项是索引1。

>[!INFO]
>
>**示例:**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`

## [!UICONTROL if （表达式；值1；值2）]

返回 `value1` 如果表达式的计算结果为true，则返回 `value2`.

>[!INFO]
>
>**示例:**
>
>* `if( 1 = 1 ; A ; B )`
>
>    返回
>
>* `if( = 2 ; A ; B )`
>
>   返回B

## [!UICONTROL imfempty (value1； value2)]

返回 `value1` 如果此值不为空，则会返回 `value2`.

>[!INFO]
>
>**示例:**
>
>* `ifempty(` `A` `;` `B` )
>
>   返回
>
>* `ifempty(` `unknown` `;` `B` )
>
>   返回B
>
>* `ifempty(` `""` `;` `B` )
>
>   返回B

## [!UICONTROL 开关(表达式；值1；结果1； [value2； result2； ...]； [else])]

根据值列表评估一个值（称为表达式）；返回与第一个匹配值对应的结果。

>[!INFO]
>
>**示例:**
>
>* `switch( B ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   返回2
>
>* `switch( C ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   返回3
>
>* `switch( X ; A ; 1 ; B ; 2 ; C ; 3 ; 4 )`
>
>  返回4

## [!UICONTROL omit(object； key1； [key2； ...])]

省略对象的给定键并返回其余键。

>[!INFO]
>
>**示例:**
>
>`omit(` 用户 `;` 密码 `)`
>
>返回用户信息的集合，不包括密码。

## [!UICONTROL pick(object； key1； [key2； ...])]

仅从对象中选取给定的键。

>[!INFO]
>
>**示例:**
>
>`pick(` 用户 `;` 密码 `;` 电子邮件 `)`
>
>仅返回用户的密码和电子邮件地址的集合。
