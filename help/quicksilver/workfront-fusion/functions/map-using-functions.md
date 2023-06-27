---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: 使用中的函数映射项 [!DNL Adobe Workfront Fusion]
description: 映射项时，可以使用函数创建简单或复杂的公式。
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# 使用中的函数映射项 [!DNL Adobe Workfront Fusion]

映射项时，可以使用函数创建简单或复杂的公式。

中可用的函数 [!DNL Adobe Workfront Fusion] 与Excel中的函数以及某些编程语言中的函数类似。 它们评估一般逻辑、数学、文本、日期和数组。 它们允许您执行项目值的条件逻辑和转换，例如将文本转换为大写、修剪文本、将日期转换为其他格式等。 有关更多信息，请参阅 [在Adobe Workfront Fusion中将信息从一个模块映射到另一个模块](../../workfront-fusion/mapping/map-information-between-modules.md).

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

## 将函数插入字段

如果单击某个字段，则 [!UICONTROL 映射] 面板显示。 映射面板包含多个选项卡：

![](assets/functions-toolbar-350x189.png)

第一个选项卡 ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) （在打开面板时显示）显示可从其他模块映射的项目。

其他选项卡包含下列类型的函数：

* **常规函数** ![](assets/toolbar-icon-general-function.png)  — 请参阅 [中的常规函数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) 了解更多信息。

* **数学函数** ![](assets/toolbar-icon-math-functions.png)  — 请参阅 [中的数学函数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) 了解更多信息。

* **文本和二进制函数** ![](assets/toolbar-icon-text&binary-functions.png)  — 请参阅 [中的字符串函数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) 了解更多信息。

* **日期和时间** ![](assets/toolbar-icon-date&time-functions.png)  — 请参阅 [中的日期和时间函数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) 和以下文章以了解更多信息。

   * [日期和时间格式的令牌 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [中的日期和时间解析令牌 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **使用数组的函数** ![](assets/toolbar-icon-functions-for-arrays.png)  — 请参阅 [中的数组函数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) 了解更多信息。

要将函数插入到字段中，请执行以下操作：

1. 单击函数名称。

   或

   将函数拖到字段中。

>[!INFO]
>
>**示例：** 某些数据类型会阻止用户输入超过一定数量的字符。 您可以使用子字符串函数将值限制为特定字符数。
>
>在此示例中，子字符串函数将项目名称限制为50个字符。
>
>![](assets/example-meet-length-restriction-350x184.png)

## 嵌套函数

可以将函数相互嵌套。

## 使用 [!DNL Google Sheets] 函数

如果 [!DNL Workfront Fusion] 不提供您要使用的功能，但它的特点是 [!DNL Google Sheets]中，您可以按照以下步骤使用它：

1. In [!DNL Google Sheets]，创建一个新的空电子表格。
1. In [!DNL Workfront Fusion]，打开您的场景。
1. 添加 **[!DNL Google Sheets]** >**[!UICONTROL 更新单元格]** 模块到场景。

   有关添加模块的说明，请参阅 [在场景中添加模块](../../workfront-fusion/scenarios/create-a-scenario.md#add) 在文章中 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. 配置模块：

   1. 选择新创建的电子表格 **[!UICONTROL 电子表格]** 字段。
   1. 插入包含 [!DNL Google Sheets] 函数移入 **[!UICONTROL 值]** 字段。

      您可以像往常一样使用前面的模块的输出。

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. 插入 **[!UICONTROL Google工作表] >[!UICONTROL 获取单元格]** 模块获取计算结果。
1. 使用在步骤4中使用的相同单元格ID配置模块。

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
