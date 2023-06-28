---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: JSON模块
description: Adobe Workfront Fusion JSON应用程序提供了用于处理JSON格式数据的模块，以便Adobe Workfront Fusion可以进一步处理数据内容或创建新的JSON内容。
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 0%

---

# [!UICONTROL JSON] 模块

此 [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] 应用程序提供用于处理JSON格式数据的模块，以便 [!DNL Adobe Workfront Fusion] 可以进一步处理数据内容，或创建新的JSON内容。

## 访问要求

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
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] （对于工作自动化和集成），[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p>
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

## 解析JSON

* [数据结构](#data-structure)
* [集合与数组](#collection-vs-array)

### 数据结构

数据结构描述了JSON数据的组织方式，并允许将单个JSON项目映射到场景中的其他模块。 如果不提供Data结构，则可以手动执行模块，并且 [!DNL Workfront Fusion] 将从提供的JSON构建结构：

1. 添加 [!UICONTROL 解析JSON] 模块到场景。
1. 在 **[!UICONTROL JSON字符串]** 字段中，输入要从中构建数据结构的JSON。
1. 不要将其他模块连接到 [!UICONTROL 解析JSON] 模块尚未完成。 因为 [!DNL Workfront Fusion] 尚不了解JSON数据的结构，尚无法映射来自的数据 [!UICONTROL 解析JSON] 模块到场景中的其他模块。
1. 手动运行方案。 这允许 [!UICONTROL 解析JSON] 模块，用于识别您提供的JSON中的JSON结构。
1. 您现在可以连接以下模块。 解析JSON模块中的项目现在可用于映射。

有关更多信息，请参阅 [中的数据结构 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md).

### 集合与数组

如果JSON字符串字段包含集合 `{ ... }`，输出是包含集合项目的单个捆绑。

>[!INFO]
>
>**示例:**
>
>```
>{
>       "name" : "Peter",
>
>    
>   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

如果JSON字符串字段包含数组 `[ ... ]`，则输出是一系列捆绑包。 每个包都包含数组的一个元素。

>[!INFO]
>
>**示例:**
>
>```
>[
>   {
>       "name" : "Peter",
>       "ID" : 1
>   },
>
>  
> {
>       "name" : "Mike",
>       "ID" : 2
>   }
>]
>```
>
>![](assets/json-array.png)

## [!UICONTROL JSON] 模块及其字段

配置时 [!DNL JSON] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还可能会显示其他JSON字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [聚合到JSON](#aggregate-to-json)
* [将JSON转换为XML](#convert-json-to-xml)
* [解析JSON](#parse-json)
* [创建JSON](#create-json)
* [转换JSON](#transform-json)

### [!UICONTROL 聚合到JSON]

此聚合器模块将上一个模块的输出聚合到JSON中。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL源模块] </td> 
   <td> <p>选择用于输出要聚合到JSON的数据的模块。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL数据结构]</td> 
   <td> <p>选择要用于创建JSON的数据结构。 数据结构决定了该模块中可用的其他字段。 有关更多信息，请参阅 <a href="#data-structure" class="MCXref xref">数据结构</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL缩进]</td> 
   <td> <p> 选择是要使用制表符、两个空格还是四个空格缩进JSON。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL分组依据]</td> 
   <td>定义要将聚合输出分组依据的表达式。 此表达式可以包含一个或多个映射项。 然后，使用此表达式的值将聚合的数据分成多个组。 每个组输出为一个单独的包，其中包含一个键（求值的表达式）和一个值（聚合文本）。 您可以在后续模块中将该键用作过滤器。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL停止处理空聚合]</td> 
   <td>启用此选项可在没有结果时停止场景。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 将JSON转换为XML]

此操作模块将JSON字符串转换为XML。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL JSON字符串] </td> 
   <td> <p>输入或映射要转换为XML的JSON。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 解析JSON]

此操作模块将JSON字符串解析为数据结构，允许您访问JSON字符串中的数据。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL数据结构]</td> 
   <td> <p>选择要用于创建JSON的数据结构。 有关更多信息，请参阅 <a href="#data-structure" class="MCXref xref">数据结构</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL JSON字符串] </td> 
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
   <td> <p>选择要用于创建JSON的数据结构。 有关更多信息，请参阅 <a href="#data-structure" class="MCXref xref">数据结构</a> 本文章中。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 转换JSON]

此操作模块会将对象转换为JSON字符串。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL对象]</td> 
   <td> <p>输入或映射要转换为JSON的对象。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 将数据记录转换为JSON

>[!INFO]
>
>**示例：** 以下示例说明如何转换数据记录 [!DNL Google Sheets] 转换为JSON格式：
>
>1. 放置 [!DNL Google Sheets] > [!UICONTROL 选择行] 模块以获取数据。 设置模块以从检索行 [!DNL Google] 电子表格。 设置&#x200B;**[!UICONTROL 返回的最大行数]** 数量较少，但出于测试目的，会大于1（例如，3）。 执行 [!DNL Google Sheets] 模块，方法是右键单击该模块并选择“**[!UICONTROL 仅运行此模块]**.” 验证模块的输出。
>
1. 连接 [!UICONTROL 数组汇总] 模块位于 [!DNL Google Sheets] 模块。 在模块的设置中，选择 [!DNL Google Sheets] 中的模块 **[!UICONTROL 源节点]** 字段。 暂时保留其他字段不变。
>
1. Connect [!UICONTROL JSON] > [!UICONTROL 创建JSON] 模块位于 [!UICONTROL 数组汇总] 模块。 模块设置需要描述JSON格式的数据结构。 单击 **[!UICONTROL 添加]** 以打开数据结构设置。 创建此数据结构的最简单方法是从JSON示例中自动生成此数据结构。 单击 **[!UICONTROL 生成器]** 并将JSON示例粘贴到 **[!UICONTROL 示例数据]** 字段：
>
**示例:**
>   
>```
>{
>
>"books": [
>
>{
>
>"id": "ID",
>
>"title": "Title",
>
>"author": "Author"
>
>}
>
>]
>
>}
>```
>
1. 单击&#x200B;**[!UICONTROL 保存]**。此 [!UICONTROL 规范] 数据结构中的字段现在包含生成的结构。
1. 将数据结构的名称更改为更具体的名称，然后单击 **[!UICONTROL 保存]**. 与root数组属性对应的字段在JSON模块的设置中显示为可映射字段。
>
1. 单击 **[!UICONTROL 映射]** 按钮并映射 `Array[]` 数组聚合器输出中的项。
>
1. 单击 **[!UICONTROL 确定]** 关闭 [!UICONTROL JSON] 模块的设置。
>
1. 打开 [!UICONTROL 数组汇总] 模块。 更改 **[!UICONTROL 目标结构]** 起始日期 [!UICONTROL 自定义] 到 [!UICONTROL JSON] 对应于根数组属性的模块字段。 从映射项目 [!DNL Google Sheets] 模块到相应的字段。
>
1. 单击 **[!UICONTROL 确定]** 关闭 [!UICONTROL 数组汇总] 模块的设置。
>
1. 运行方案。
>
此 [!UICONTROL JSON] 模块输出正确的JSON格式。
>
1. 打开 [!DNL Google Sheets] 模块并增加 [!UICONTROL 返回的最大行数] 数，以大于电子表格中用于处理所有数据的行数。

## 故障排除

### 无法映射以下位置的数据： [!UICONTROL 解析JSON] 模块

确保JSON内容正确映射到 [!UICONTROL 解析JSON] 模块，并确保数据结构已正确定义。 有关更多信息，请参阅 [将数据记录转换为JSON](#transforming-data-records-to-json) 本文章中。

### 在JSON中使用条件语句时，模块失败

使用条件语句(例如 `if` 在JSON中，将引号放在条件语句之外。

>[!INFO]
>
**示例:**
>
![](assets/quotes-in-json-350x120.png)
