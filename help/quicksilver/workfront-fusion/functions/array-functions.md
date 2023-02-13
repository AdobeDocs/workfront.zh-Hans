---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion中的数组函数
description: 以下数组函数在Adobe Workfront Fusion映射面板中可用。
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Adobe Workfront Fusion中的数组函数

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

## [!UICONTROL 添加（数组）；value1;value2;...)]

将参数中指定的值添加到数组并返回该数组。

## [!UICONTROL 包含（数组）；value)]

验证数组是否包含值。

## [!UICONTROL distinct(array); [key])]

删除数组内的重复项。 使用“[!UICONTROL key]用于访问复杂对象中属性的参数。 要访问嵌套属性，请使用点表示法。 数组中的第一个项是索引1。

>[!INFO]
>
>**示例：** `distinct(Contacts[];name)`
>
>通过比较“name”属性，删除联系人数组中的重复项

## [!UICONTROL flatten(array)]

创建一个新数组，其中所有子数组元素以递归方式连接到该数组中，直到达到指定的深度。


## [!UICONTROL 连接（数组）；分隔符]

使用每个项之间指定的分隔符，将数组的所有项串联到字符串中。

## [!UICONTROL 键（对象）]

返回给定对象或数组属性的数组。

## [!UICONTROL length（数组）]

返回数组中的项数。

## [!UICONTROL 地图（复杂数组）；键；[筛选键];[筛选的可能值])]

返回包含复杂数组值的基元数组。 此函数允许筛选值。 为键使用原始变量名称。

>[!INFO]
>
>**示例:**
>
>* `map(Emails[];email)`
  >
>  通过电子邮件返回基元数组
>
>* `map(Emails[];email;label;work;home)`
  >
>  返回带有标签等于工作或家庭的电子邮件的原始数组

有关更多信息，请参阅 [在 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)


## [!UICONTROL 合并(array1;array2;...)]

将一个或多个阵列合并到一个阵列中。

## [!UICONTROL 删除（数组）；value1;value2;...)]

删除数组参数中指定的值。 此函数仅对文本或数字的基元数组有效。

## [!UICONTROL 反向（数组）]

数组的第一个元素成为最后一个元素，第二个元素成为倒数第二个元素，依此类推。

## [!UICONTROL 片（阵列）；开始； [end])]

返回仅包含选定项的新数组。

## [!UICONTROL 排序（数组）； [订购]; [key])]

对数组的值进行排序。 的有效值 `order` 参数为：

* `asc`

   （默认） — 升序：类型“数字”的1、2、3、... A、B、C、a、b、c、...表示“文本”类型

* `desc`

   降序顺序：...、3、2、1表示类型“数字”。...、c、b、a、c、B、A表示文本类型。

* `asc ci`

   不区分大小写的升序顺序：A、a、B、b、C、c...表示“文本”类型。

* `desc ci`

   不区分大小写的降序顺序：...、C、c、B、b、A，表示“文本”类型。

使用 `key` 用于访问复杂对象中属性的参数。

为键使用原始变量名称。

要访问嵌套属性，请使用点表示法。

数组中的第一个项是索引1。

>[!INFO]
>
>**示例:**
>
>* `sort(Contacts[];name)`
   >
   >    按默认升序顺序，使用“name”属性对联系人数组进行排序
>
>* `sort(Contacts[];desc;name)`
   >
   >   按“name”属性以降序方式对联系人数组进行排序
>
>* `sort(Contacts[];asc ci;name)`
   >
   >    按“name”属性对联系人数组进行不区分大小写的升序排序
>
>* `sort(Emails[];sender.name)`
   >
   >    按“sender.name”属性对电子邮件数组进行排序


## [!UICONTROL arrayDifference [array1, array2, mode]]

返回两个数组之间的差异。

为 `mode` 参数。

* `classic`:返回一个包含 `array1` 中不存在 `array2`.

* `symmetric`:返回两个数组不通用的元素数组。

   换言之，函数会返回一个包含 `array1` 中不存在 `array2`，以及 `array2` 中不存在 `array1`.

   >[!INFO]
   >
   >**示例:**
   >
   >假定以下数组：
   >
   >
   ```
   >myArray = [1,2,3,4,5]
   >```
   >
   >
   ```
   >yourArray = [3,4,5,6,7]
   >```
   >
   >* `arrayDifference [myArray, yourArray, classic]`
      >
      >    返回结果 `[1,2]`
   >
   >* `arrayDifference [yourArray, myArray, classic]`
      >
      >    返回结果 `[6,7]`
   >
   >* `arrayDifference [myArray, yourArray, symmetric]`
      >
      >    返回结果 `[1,2,6,7]`

