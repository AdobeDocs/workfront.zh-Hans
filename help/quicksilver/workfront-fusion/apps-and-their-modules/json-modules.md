---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: JSON模块
description: Adobe Workfront Fusion JSON应用程序提供了用于处理JSON格式数据的模块，以便Adobe Workfront Fusion能够进一步处理数据内容或创建新的JSON内容。
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 0%

---

# [!UICONTROL JSON] 模块

的 [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] 应用程序提供了用于处理JSON格式数据的模块，以便 [!DNL Adobe Workfront Fusion] 可以进一步处理数据内容，或创建新的JSON内容。

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 解析JSON

* [数据结构](#data-structure)
* [集合与数组](#collection-vs-array)

### 数据结构

数据结构描述了JSON数据的组织方式，并允许将单个JSON项目映射到方案中的其他模块。 如果不提供数据结构，则可以手动执行模块和 [!DNL Workfront Fusion] 将从提供的JSON构建结构：

1. 添加 [!UICONTROL 解析JSON] 模块。
1. 在 **[!UICONTROL JSON字符串]** 字段中，输入要从中构建数据结构的JSON。
1. 请勿将其他模块连接到 [!UICONTROL 解析JSON] 模块。 因为 [!DNL Workfront Fusion] 尚不知道JSON数据的结构，因此尚无法映射 [!UICONTROL 解析JSON] 模块添加到方案中的其他模块。
1. 手动运行方案。 这允许 [!UICONTROL 解析JSON] 用于从您提供的JSON中标识JSON结构的模块。
1. 您现在可以连接以下模块。 解析JSON模块中的项目现在可用于映射。

有关更多信息，请参阅 [中的数据结构 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md).

### 集合与数组

如果JSON字符串字段包含集合 `{ ... }`，则输出是一个包含集合项的包。

>[!INFO]
>
>**示例:**
>
>
```
>{
>       "name" : "Peter",
>
>    
   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

如果JSON字符串字段包含数组 `[ ... ]`，则输出是一系列包。 每个包都包含数组的一个元素。

>[!INFO]
>
>**示例:**
>
>
```
>[
>   {
>       "name" : "Peter",
>       "ID" : 1
>   },
>
>  
 {
>       "name" : "Mike",
>       "ID" : 2
>   }
>]
>```
>
>![](assets/json-array.png)

## [!UICONTROL JSON] 模块及其字段

配置 [!DNL JSON] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除这些字段外，可能还会显示其他JSON字段，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [聚合到JSON](#aggregate-to-json)
* [将JSON转换为XML](#convert-json-to-xml)
* [解析JSON](#parse-json)
* [创建JSON](#create-json)
* [转换JSON](#transform-json)

### [!UICONTROL 聚合到JSON]

此聚合模块将来自先前模块的输出聚合到JSON中。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源模块] </td> 
   <td> <p>选择用于输出要聚合到JSON的数据的模块。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL数据结构]</td> 
   <td> <p>选择要创建JSON的数据结构。 数据结构确定此模块中可用的其他字段。 有关更多信息，请参阅 <a href="#data-structure" class="MCXref xref">数据结构</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL缩进]</td> 
   <td> <p> 选择要使用制表符、两个空格还是四个空格缩进JSON。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by]</td> 
   <td>定义要将聚合输出分组为的表达式。 此表达式可以包含一个或多个映射的项目。 然后，使用此表达式的值将聚合数据分成组。 每个组以一个单独的包的形式输出，包含键（计算的表达式）和值（聚合的文本）。 您可以在后续模块中将键用作过滤器。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL空聚合后停止处理]</td> 
   <td>启用此选项可在没有结果时停止方案。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 将JSON转换为XML]

此操作模块会将JSON字符串转换为XML。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON字符串] </td> 
   <td> <p>输入或映射要转换为XML的JSON。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 解析JSON]

此操作模块将JSON字符串解析为数据结构，以便您访问JSON字符串内的数据。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL数据结构]</td> 
   <td> <p>选择要创建JSON的数据结构。 有关更多信息，请参阅 <a href="#data-structure" class="MCXref xref">数据结构</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON字符串] </td> 
   <td> <p>输入或映射要解析的JSON。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 创建JSON]

此操作模块从数据结构创建JSON。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">数据结构</td> 
   <td> <p>选择要创建JSON的数据结构。 有关更多信息，请参阅 <a href="#data-structure" class="MCXref xref">数据结构</a> 在本文中。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 转换JSON]

此操作模块会将对象转换为json字符串。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL对象]</td> 
   <td> <p>输入或映射要转换为JSON的对象。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 将数据记录转换为JSON

>[!INFO]
>
>**示例：** 以下示例显示如何从转换数据记录 [!DNL Google Sheets] 为JSON格式：
>
>1. 将 [!DNL Google Sheets] > [!UICONTROL 选择行] 模块来获取数据。 设置模块以从 [!DNL Google] 电子表格。 设置&#x200B;**[!UICONTROL 返回的最大行数]** 值较小，但出于测试目的大于1（例如，3）。 执行 [!DNL Google Sheets] 模块，方法是右键单击该模块并选择“**[!UICONTROL 仅运行此模块]**.&quot; 验证模块的输出。
1. 连接 [!UICONTROL 阵列聚合器] 模块之后 [!DNL Google Sheets] 模块。 在模块的设置中，选择 [!DNL Google Sheets] 模块 **[!UICONTROL 源节点]** 字段。 暂时保留其他字段。
1. 连接 [!UICONTROL JSON] > [!UICONTROL 创建JSON] 模块之后 [!UICONTROL 阵列聚合器] 模块。 模块的设置需要描述JSON格式的数据结构。 单击 **[!UICONTROL 添加]** 打开数据结构设置。 创建此数据结构的最简单方法是从JSON示例自动生成此数据结构。 单击 **[!UICONTROL 发电机]** 并将您的JSON示例粘贴到 **[!UICONTROL 示例数据]** 字段：

   **示例:**
   ```
   {
   
   "books": [
   
   {
   
   "id": "ID",
   
   "title": "Title",
   
   "author": "Author"
   
   }
   
   ]
   
   }
   ```
1. 单击&#x200B;**[!UICONTROL 保存]**。的 [!UICONTROL 规范] “数据结构”中的字段现在包含生成的结构。
1. 将数据结构的名称更改为更具体的内容，然后单击 **[!UICONTROL 保存]**. 与根数组属性对应的字段在JSON模块的设置中显示为可映射的字段。
1. 单击 **[!UICONTROL 地图]** 按钮，并映射 `Array[]` 项。
1. 单击 **[!UICONTROL 确定]** 关闭 [!UICONTROL JSON] 模块的设置。
1. 打开的设置 [!UICONTROL 阵列聚合器] 模块。 更改 **[!UICONTROL 目标结构]** 从 [!UICONTROL 自定义] 到 [!UICONTROL JSON] 对应于根数组属性的模块字段。 映射 [!DNL Google Sheets] 模块。
1. 单击 **[!UICONTROL 确定]** 关闭 [!UICONTROL 阵列聚合器] 模块的设置。
1. 运行方案。
   的 [!UICONTROL JSON] 模块输出正确的JSON格式。
1. 打开的设置 [!DNL Google Sheets] 模块并增加 [!UICONTROL 返回的最大行数] 值大于电子表格中的行数以处理所有数据。


## 疑难解答

### 无法映射 [!UICONTROL 解析JSON] 模块

确保将JSON内容正确映射到 [!UICONTROL 解析JSON] 模块，且数据结构已正确定义。 有关更多信息，请参阅 [将数据记录转换为JSON](#transforming-data-records-to-json) 在本文中。

### 在JSON中使用条件语句时模块失败

使用条件语句时，例如 `if` 在JSON中，将引号放置在条件语句的外部。

>[!INFO]
**示例:**
![](assets/quotes-in-json-350x120.png)
