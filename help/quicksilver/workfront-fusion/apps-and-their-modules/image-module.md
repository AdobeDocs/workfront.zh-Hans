---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 图像模块
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 89efa9d5-00c9-4bb5-97b3-2b2f9d73721d
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# 图像模块

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [图像模块](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/image-module.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

[!DNL Adobe Workfront Fusion] [!UICONTROL 图像]模块允许您获取有关特定图像（尺寸、类型等）的信息，将图像转换为其他文件格式，并直接更改图像的大小。

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

## [!UICONTROL 图像]模块及其字段

配置此模块时，会显示以下字段。 模块中的粗体标题表示必填字段。

* [[!UICONTROL 调整大小]](#resize)
* [[!UICONTROL 转换格式]](#convert-a-format)
* [[!UICONTROL 提取元数据]](#extract-metadata)

### [!UICONTROL 调整大小]

此转换器模块会根据您指定的条件更改图像的高度和宽度。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source file]</td> 
   <td> <p>选择要转换的图像的源。 您可以选择上一个模块的输出，或者映射数据文件和文件名。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL数据]</td> 
   <td>映射要转换的文件。 如果您在[！UICONTROL Source file]字段中选择了[！UICONTROL Map] ，则此字段可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件名]</td> 
   <td>输入转换文件的名称。 如果您在[！UICONTROL Source file]字段中选择了[！UICONTROL Map] ，则此字段可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL我想]</td> 
   <td>选择是要保持高宽比还是将尺寸更改为指定的高度和宽度。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL根据]</td> 
   <td> <p>选择您希望模块如何确定图像的新大小。 如果您在“我想”字段中选择了保持高宽比，则会显示此字段。 根据在此字段中选择的内容，将显示其他字段。</p> 
    <ul> 
     <li> <p>[！UICONTROL最大宽度]</p> <p>将图像缩小到您指定的宽度。 高度会自动计算。</p> </li> 
     <li> <p>[！UICONTROL最大高度]</p> <p>将图像缩小到您指定的高度。 会自动计算宽度。</p> </li> 
     <li> <p>[！UICONTROL最大高度或宽度]</p> <p>以高度和宽度不超过指定值的方式缩小图像。 由于此选项会保持高宽比，因此其中一个尺寸可能小于指定的尺寸。 例如，如果高度和宽度都指定为40，则400x300图像将减少到40X30。</p> </li> 
     <li> <p>[！UICONTROL最小宽度]</p> <p>将图像放大到您指定的宽度。 高度会自动计算。</p> </li> 
     <li> <p>[！UICONTROL最小高度]</p> <p>将图像放大到您指定的高度。 会自动计算宽度。</p> </li> 
     <li> <p>[！UICONTROL最小高度或宽度]</p> <p>以不小于指定值的高度和宽度来放大图像。 由于此选项会保持高宽比，因此其中一个尺寸可能大于指定的尺寸。 例如，如果高度和宽度都指定为300，则40x30图像将放大为400X300。</p> </li> 
     <li> <p>[！UICONTROL百分比]</p> <p>根据您指定的值按百分比更改图像大小。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL宽度]</td> 
   <td>输入或映射调整大小的图像的所需宽度（以像素为单位）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Height]</td> 
   <td>输入或映射调整大小后图像的所需高度（以像素为单位）。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 转换格式]

此转换器模块更改图像文件的格式。 此模块兼容以下格式：

* PNG
* JPG
* GIF
* BMP

源文件和输出都必须采用以下格式之一。 例如，[!UICONTROL Image] >[!UICONTROL 转换格式]模块可以将PNG文件转换为BMP文件，或将BMP转换为JPG。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source file]</td> 
   <td> <p>选择要转换的图像的源。 您可以选择上一个模块的输出，或者映射数据文件和文件名。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL数据]</td> 
   <td>映射要转换的文件。 如果您在[！UICONTROL Source file]字段中选择了[！UICONTROL Map] ，则此字段可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件名]</td> 
   <td>输入转换文件的名称。 如果您在[！UICONTROL Source file]字段中选择了[！UICONTROL Map] ，则此字段可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出格式]</td> 
   <td>选择您希望模块将源文件转换成的格式。 </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 提取元数据]

此转换器模块返回有关模块的基本信息。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source file]</td> 
   <td> <p>选择要转换的图像的源。 您可以选择上一个模块的输出，或者映射数据文件和文件名。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL数据]</td> 
   <td>映射要转换的文件。 如果您在[！UICONTROL Source file]字段中选择了映射，则此字段可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件名]</td> 
   <td>输入转换文件的名称。 如果您在[！UICONTROL Source file]字段中选择了映射，则此字段可用。</td> 
  </tr> 
 </tbody> 
</table>

## 可能的问题

### 操作因错误而终止

在以下三种情况下，操作可能会因错误而终止：

* 接收的数据不是JPG/GIF/PNG/BMP格式
* 更改图像尺寸时，已超过最大宽度/高度限制。 图像大小不得超过3840像素宽度和2160像素高度
* 更改图像的尺寸或格式时，已超过允许的最大图像大小。
