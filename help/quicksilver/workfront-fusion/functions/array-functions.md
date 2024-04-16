---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion中的数组函数
description: Adobe Workfront Fusion映射面板中提供了以下数组函数。
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: 033a9f4aa1f191e5e3cabd0c0f232128fa6bce5d
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 1%

---

# Adobe Workfront Fusion中的数组函数

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
   <p>当前：否 [!DNL Workfront Fusion] 许可证要求。</p> 
   <p>或</p> 
   <p>旧版：任意 </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">产品</td>  
   <td> 
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront] 计划：您的组织必须购买 [!DNL Adobe Workfront Fusion].</li><li>[！UICONTROL Ultimate] [!DNL Workfront] 计划： [!DNL Workfront Fusion] 中包含。</li></ul> 
   <p>或</p> 
   <p>当前：您的组织必须购买 [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

有关的信息 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 函数

* [加入](#join-array-separator)
* [length](#length-array)
* [键](#keys-object)
* [切片](#slice-array-start-end)
* [合并](#merge-array1-array2)
* [包含](#contains-array-value)
* [移除](#remove-array-value1-value2)
* [添加](#add-array-value1-value2)
* [映射](#map-complex-array-keykey-for-filteringpossible-values-for-filtering)
* [随机播放]
* [sort](#sort-array-order-key)
* [反向](#reverse-array)
* [flatten](#flatten-array)
* [distinct](#distinct-array-key)
* [toCollection]
* [toArray](#toarray)
* [arrayDifference](#arraydifference-array1-array2-mode)
* [删除重复项]

### [!UICONTROL 连接（数组；分隔符）]

将数组的全部项串联到一个字符串中，在每个项之间使用指定的分隔符。

### [!UICONTROL 长度（数组）]

返回数组中的项数。

### [!UICONTROL 键（对象）]

返回给定对象或数组的属性的数组。

### [!UICONTROL 片(数组；起始； [结束])]

返回仅包含选定项目的新数组。

### [!UICONTROL 合并(array1； array2； ...)]

将一个或多个阵列合并到一个阵列中。

### [!UICONTROL 包含（数组；值）]

验证数组是否包含值。

### [!UICONTROL 移除（数组；值1；值2； ...）]

删除数组的参数中指定的值。 此函数仅对文本或数字的原始数组有效。

### [!UICONTROL 添加（数组；值1；值2； ...）]

将参数中指定的值添加到数组中并返回该数组。

### [!UICONTROL 映射(复数组；键；[筛选键]；[筛选的可能值])]

返回包含复杂数组的值的原始数组。 此函数允许过滤值。 对键使用原始变量名称。

>[!INFO]
>
>**示例：**
>
>* `map(Emails[];email)`
>
>  返回带有电子邮件的原始数组
>
>* `map(Emails[];email;label;work;home)`
>
>  返回带有标签等于工作或主页的原始数组

有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)

### 随机播放

### [!UICONTROL 排序(数组； [订购]； [键])]

对数组的值进行排序。 的有效值 `order` 参数为：

* `asc`

  （默认） — 升序：类型“数字”为1、2、3、...。 A， B， C， a， b， c， ...表示文字

* `desc`

  降序： ...， 3， 2， 1表示类型“数字”。...， c， b， a， C， B， A代表文字。

* `asc ci`

  不区分大小写的升序：A、a、B、b、C、c...表示文本类型。

* `desc ci`

  不区分大小写降序： ...， C， c， B， b， A，用于类型“文本”。

使用 `key` 用于访问复杂对象内部的属性的参数。

对键使用原始变量名称。

要访问嵌套属性，请使用点表示法。

数组中的第一项是索引1。

>[!INFO]
>
>**示例：**
>
>* `sort(Contacts[];name)`
>
>    按“name”属性以默认升序排序联系人数组
>
>* `sort(Contacts[];desc;name)`
>
>   按“name”属性降序排列联系人数组
>
>* `sort(Contacts[];asc ci;name)`
>
>    按“name”属性以不区分大小写的升序对联系人数组排序
>
>* `sort(Emails[];sender.name)`
>
>    按“sender.name”属性对电子邮件数组排序

### [!UICONTROL 反向（数组）]

数组的第一个元素成为最后一个元素，第二个元素成为倒数第二个元素，依此类推。

### [!UICONTROL 扁平化（数组）]

创建一个新数组，其中所有子数组元素以递归方式连接到该数组，直至指定深度。

### [!UICONTROL distinct (array； [键])]

删除数组中的重复项。 使用&quot;[!UICONTROL 键]”参数访问复杂对象中的属性。 要访问嵌套属性，请使用点表示法。 数组中的第一项是索引1。

>[!INFO]
>
>**示例：** `distinct(Contacts[];name)`
>
>通过比较“name”属性，删除联系人数组中的重复项

### toCollection

### toArray

此函数将一个集合转换为键值对的数组。

>[!INFO]
>
>**示例：**
>
>给定收藏集
>
>`{ key1: "value1", key2: "value2:}`
>
>函数
>
>`toArray({ key1: "value1", key2: "value2:})`
>
>返回键值对的数组
>
>`[{ key1: "value1"}, { key2: "value2"}]`

### [!UICONTROL arrayDifference [阵列1，阵列2，模式]]

返回两个数组之间的差值。

输入以下值之一 `mode` 参数。

* `classic`：返回包含的所有元素的新数组 `array1` 中不存在的 `array2`.

* `symmetric`：返回两个数组不共用的元素数组。

  换句话说，此函数返回一个数组，其中包含的所有元素。 `array1` 中不存在的 `array2`，以及的所有元素 `array2` 中不存在的 `array1`.

  >[!INFO]
  >
  >**示例：**
  >
  >给定以下数组：
  >
  >```
  >myArray = [1,2,3,4,5]
  >```
  >
  >```
  >yourArray = [3,4,5,6,7]
  >```
  >
  >* `arrayDifference [myArray, yourArray, classic]`
  >
  >    返回 `[1,2]`
  >
  >* `arrayDifference [yourArray, myArray, classic]`
  >
  >    返回 `[6,7]`
  >
  >* `arrayDifference [myArray, yourArray, symmetric]`
  >
  >    返回 `[1,2,6,7]`

### 删除重复项

## 关键字

### emptyarray
