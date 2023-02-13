---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: 使用 [!DNL Adobe Workfront Fusion]
description: 映射项目时，可以使用函数创建简单或复杂的公式。
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# 使用 [!DNL Adobe Workfront Fusion]

映射项目时，可以使用函数创建简单或复杂的公式。

中可用的函数 [!DNL Adobe Workfront Fusion] 与Excel和某些编程语言中的函数类似。 它们评估常规逻辑、数学、文本、日期和数组。 它们允许您对项目值执行条件逻辑和转换，例如将文本转换为大写、修剪文本、将日期转换为其他格式等。 有关更多信息，请参阅 [在Adobe Workfront Fusion中，将信息从一个模块映射到另一个模块](../../workfront-fusion/mapping/map-information-between-modules.md).

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

## 将函数插入字段

如果单击某个字段，则 [!UICONTROL 映射] 面板。 映射面板包含多个选项卡：

![](assets/functions-toolbar-350x189.png)

第一个选项卡 ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) （在打开面板时显示）显示可从其他模块映射的项目。

其他选项卡包含以下类型的函数：

* **一般函数** ![](assets/toolbar-icon-general-function.png)  — 请参阅 [中的常规函数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) 以了解更多信息。

* **数学函数** ![](assets/toolbar-icon-math-functions.png)  — 请参阅 [中的数学函数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) 以了解更多信息。

* **文本和二进制函数** ![](assets/toolbar-icon-text&binary-functions.png)  — 请参阅 [中的字符串函数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) 以了解更多信息。

* **日期和时间** ![](assets/toolbar-icon-date&time-functions.png)  — 请参阅 [中的日期和时间函数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) 和以下文章以了解更多信息。

   * [中用于日期和时间格式的令牌 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [用于在中解析日期和时间的令牌 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **使用数组的函数** ![](assets/toolbar-icon-functions-for-arrays.png)  — 请参阅 [中的数组函数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) 以了解更多信息。

要将函数插入字段，请执行以下操作：

1. 单击函数名称。

   或

   将函数拖到字段中。

>[!INFO]
>
>**示例：** 某些数据类型会阻止用户输入多于特定数量的字符。 您可以使用子字符串函数将值限制为特定数量的字符。
>
>在此示例中，子字符串函数将项目名称限制为50个字符。
>
>![](assets/example-meet-length-restriction-350x184.png)

## 嵌套函数

您可以相互嵌套函数。

## 使用 [!DNL Google Sheets] 函数

如果 [!DNL Workfront Fusion] 不包含您想要使用的函数，但其特征是 [!DNL Google Sheets]，您可以通过以下步骤使用它：

1. 在 [!DNL Google Sheets]，则创建新的空电子表格。
1. 在 [!DNL Workfront Fusion]，打开您的方案。
1. 添加 **[!DNL Google Sheets]** >**[!UICONTROL 更新单元格]** 模块。

   有关添加模块的说明，请参阅 [在方案中添加模块](../../workfront-fusion/scenarios/create-a-scenario.md#add) 在文章中 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. 配置模块：

   1. 在 **[!UICONTROL 电子表格]** 字段。
   1. 插入包含 [!DNL Google Sheets] 函数 **[!UICONTROL 值]** 字段。

      您可以像往常一样使用前面模块的输出。

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. 插入 **[!UICONTROL Google工作表] >[!UICONTROL 获取手机]** 模块获取计算结果。
1. 使用步骤4中使用的相同单元格ID配置模块。

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
