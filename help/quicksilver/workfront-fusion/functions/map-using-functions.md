---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: 使用 [!DNL Adobe Workfront Fusion]中的函数映射项
description: 映射项时，可以使用函数创建简单或复杂的公式。
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: d175a3d43f13338661d8b7e1cb79038a36522ff9
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# 使用[!DNL Adobe Workfront Fusion]中的函数映射项

映射项时，可以使用函数创建简单或复杂的公式。 [!DNL Adobe Workfront Fusion]中可用的函数类似于Excel中的函数以及某些编程语言中的函数：

* 它们评估一般逻辑、数学、文本、日期和数组。
* 它们允许您执行条件逻辑和项值的转换，例如将文本转换为大写、修剪文本、将日期转换为不同格式等。

有关详细信息，请参阅[在Adobe Workfront Fusion中将信息从一个模块映射到另一个模块](../../workfront-fusion/mapping/map-information-between-modules.md)。


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


## “映射”选项卡概述

打开字段的[!UICONTROL 映射]面板：

1. 单击左侧面板中的&#x200B;**方案**。
1. 选择一个方案。

![](assets/open-functions-bar.png)


### “映射”面板选项卡

以下是“映射”面板中的选项卡：

* **常规函数** ![](assets/toolbar-icon-general-function.png) — 有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md)中的[常规函数。

* **数学函数** ![](assets/toolbar-icon-math-functions.png) — 有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md)中的[数学函数。

* **文本和二进制函数** ![](assets/toolbar-icon-text&binary-functions.png) — 有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md)中的[字符串函数。

* **日期和时间** ![](assets/toolbar-icon-date&time-functions.png) — 有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md)中的[日期和时间函数，以及下面的文章：

   * [ [!DNL Adobe Workfront Fusion]中日期和时间格式的令牌](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [ [!DNL Adobe Workfront Fusion]中用于日期和时间分析的令牌](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **用于处理数组的函数** ![](assets/toolbar-icon-functions-for-arrays.png) — 有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md)中的[数组函数。

* **映射其他函数** ![](assets/toolbar-icon-functions-you-map-from-other-modules.png)显示可从其他模块映射的项目。 此选项卡并非始终可用。

![](assets/functions-toolbar-350x189.png)

## 在字段中插入函数

要将函数插入到字段中，请执行以下操作：

1. 单击函数名称。

   或

   将函数拖到字段中。


>[!BEGINSHADEBOX]

**示例：**&#x200B;某些数据类型会阻止用户输入超过一定数量的字符。 您可以使用子字符串函数将值限制为特定字符数。

在此示例中，子字符串函数将项目名称限制为50个字符。

![](assets/example-meet-length-restriction-350x184.png)

>[!ENDSHADEBOX]

## 嵌套函数

可以将函数相互嵌套。

## 使用[!DNL Google Sheets]函数

如果[!DNL Workfront Fusion]不提供您要使用的函数，但它由[!DNL Google Sheets]提供，您可以按照以下步骤使用它：

1. 在[!DNL Google Sheets]中，创建一个新的空电子表格。
1. 在[!DNL Workfront Fusion]中，打开您的方案。
1. 将&#x200B;**[!DNL Google Sheets]** >**[!UICONTROL 更新单元格]**&#x200B;模块添加到方案。

   有关添加模块的说明，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中创建方案一文中的[在方案中添加模块](../../workfront-fusion/scenarios/create-a-scenario.md#add)。

1. 配置模块：

   1. 在&#x200B;**[!UICONTROL 电子表格]**&#x200B;字段中选择新创建的电子表格。
   1. 将包含[!DNL Google Sheets]函数的公式插入到&#x200B;**[!UICONTROL 值]**&#x200B;字段中。

      您可以像往常一样使用前面的模块的输出。

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. 插入&#x200B;**[!UICONTROL Google工作表] >[!UICONTROL 获取单元格]**&#x200B;模块以获取计算结果。
1. 使用在步骤4中使用的相同单元格ID配置模块。

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
