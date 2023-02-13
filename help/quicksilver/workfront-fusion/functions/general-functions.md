---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion中的一般函数
description: Adobe Workfront Fusion映射面板中提供了以下常规函数。
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 2%

---

# 中的常规函数 [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL get（对象或数组）；path)]

返回对象或数组的值路径。 要访问嵌套对象，请使用点表示法。 数组中的第一个项是索引1。

>[!INFO]
>
>**示例:**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`


## [!UICONTROL if（表达式）；value1;value2)]

返回 `value1` 如果表达式的计算结果为true;否则，它将返回 `value2`.

>[!INFO]
>
>**示例:**
>
>* `if( 1 = 1 ; A ; B )`
   >
   >    返回A
>
>* `if( = 2 ; A ; B )`
   >
   >   返回B


## [!UICONTROL ifempty(value1;value2)]

返回 `value1` 如果此值不为空；否则，它将返回 `value2`.

>[!INFO]
>
>**示例:**
>
>* `ifempty(` `A` `;` `B` )
   >
   >   返回A
>
>* `ifempty(` `unknown` `;` `B` )
   >
   >   返回B
>
>* `ifempty(` `""` `;` `B` )
   >
   >   返回B


## [!UICONTROL 开关（表达式）；value1;结果1; [value2;结果2;...]; [else])]

根据值列表计算一个值（称为表达式）；返回与第一个匹配值对应的结果。

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

## [!UICONTROL opt(object);键1; [key2;...])]

忽略对象的给定键，并返回其余键。

>[!INFO]
>
>**示例:**
>
>`omit(` 用户 `;` 密码 `)`
>
>返回用户信息的集合，不包括密码。

## [!UICONTROL pick(object);键1; [key2;...])]

仅选取对象中的给定键。

>[!INFO]
>
>**示例:**
>
>`pick(` 用户 `;` 密码 `;` 电子邮件 `)`
>
>仅返回用户密码和电子邮件地址的集合。
