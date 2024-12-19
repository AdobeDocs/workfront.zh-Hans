---
title: JSONata模块
description: Adobe Workfront Fusion JSONata连接器提供了一个用于处理JSON格式数据的模块，以便Adobe Workfront Fusion可以进一步处理数据内容。
author: Becky
feature: Workfront Fusion
source-git-commit: b7a6ecd9089c3a5517c56b849b860d57a900dade
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 1%

---

# [!UICONTROL JSONata]模块

[!DNL Adobe Workfront Fusion] [!UICONTROL JSONata]连接器允许您查询JSON对象。 此模块不需要连接。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td>
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

+++

## JSONata模块及其字段

### 评估

此操作模块可查询JSON对象并返回数组。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL表达式]</td> 
   <td>输入要用于计算JSON对象的表达式。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL数据] </td> 
   <td> 输入要计算的JSON对象。  </td> 
  </tr> 
  </tbody>
  </table>

>[!BEGINSHADEBOX]

**示例**：

目标是从以下JSON对象返回名称数组：

```JSON
{
  "people": [
    { "name": "Alice", "age": 30 },
    { "name": "Bob", "age": 25 },
    { "name": "Charlie", "age": 35 }
  ]
}
```

1. 在表达式字段中，输入`people.name`。
1. 在数据字段中，输入JSON对象。

模块返回从JSON对象拉取的名称数组。

>[!ENDSHADEBOX]
