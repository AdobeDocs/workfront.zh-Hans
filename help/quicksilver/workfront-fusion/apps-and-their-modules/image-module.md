---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 图像模块
description: Adobe Workfront Fusion Image模块允许您获取有关特定图像的信息（尺寸、类型等），将图像转换为另一种文件格式，以及直接更改图像的大小。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 89efa9d5-00c9-4bb5-97b3-2b2f9d73721d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# 图像模块

[!DNL Adobe Workfront Fusion] [!UICONTROL 图像] 利用模块，可获取有关特定图像（尺寸、类型等）的信息，将图像转换为另一种文件格式，并直接更改图像的大小。

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

## [!UICONTROL 图像] 模块及其字段

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
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>选择要转换的图像的源。 您可以选择上一个模块的输出，或者映射数据文件和文件名。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL数据]</td> 
   <td>映射要转换的文件。 如果您在[！UICONTROL源文件]字段中选择了[！UICONTROL映射]，则此字段可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件名]</td> 
   <td>输入已转换文件的名称。 如果您在[！UICONTROL源文件]字段中选择了[！UICONTROL映射]，则此字段可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL I want to]</td> 
   <td>选择是要保持高宽比还是将尺寸更改为指定的高度和宽度。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL根据]</td> 
   <td> <p>选择您希望模块如何确定图像的新大小。 如果您在“我想”字段中选择了保持高宽比，则会显示此字段。 根据此字段中的选择，将显示其他字段。</p> 
    <ul> 
     <li> <p>[！UICONTROL最大宽度]</p> <p>将图像缩小到您指定的宽度。 高度会自动计算。</p> </li> 
     <li> <p>[！UICONTROL最大高度]</p> <p>将图像缩小到您指定的高度。 将自动计算宽度。</p> </li> 
     <li> <p>[！UICONTROL最大高度或宽度]</p> <p>以高度和宽度不超过指定值的方式减少图像。 由于此选项会保持高宽比，因此其中一个尺寸可能小于指定的尺寸。 例如，如果高度和宽度都指定为40，则400x300图像将缩减为40X30。</p> </li> 
     <li> <p>[！UICONTROL最小宽度]</p> <p>将图像放大到您指定的宽度。 高度会自动计算。</p> </li> 
     <li> <p>[！UICONTROL最小高度]</p> <p>将图像放大到您指定的高度。 将自动计算宽度。</p> </li> 
     <li> <p>[！UICONTROL最小高度或宽度]</p> <p>以不小于指定值的方式放大图像。 由于此选项会保持高宽比，因此其中一个尺寸可能大于指定的尺寸。 例如，如果高度和宽度都指定为300，则40x30图像将放大为400X300。</p> </li> 
     <li> <p>[！UICONTROL百分比]</p> <p>根据指定的值按百分比更改图像大小。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL宽度]</td> 
   <td>输入或映射调整大小的图像的所需宽度（以像素为单位）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Height]</td> 
   <td>输入或映射调整大小的图像的所需高度（以像素为单位）。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 转换格式]

此转换器模块更改图像文件的格式。 此模块兼容以下格式：

* PNG
* JPG
* GIF
* BMP

源文件和输出都必须采用以下格式之一。 例如， [!UICONTROL 图像] >[!UICONTROL 转换格式] 模块可以将PNG文件转换为BMP文件，也可以将BMP转换为JPG。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>选择要转换的图像的源。 您可以选择上一个模块的输出，或者映射数据文件和文件名。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL数据]</td> 
   <td>映射要转换的文件。 如果您在[！UICONTROL源文件]字段中选择了[！UICONTROL映射]，则此字段可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件名]</td> 
   <td>输入已转换文件的名称。 如果您在[！UICONTROL源文件]字段中选择了[！UICONTROL映射]，则此字段可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出格式]</td> 
   <td>选择您希望模块将源文件转换为的格式。 </td> 
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
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>选择要转换的图像的源。 您可以选择上一个模块的输出，或者映射数据文件和文件名。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL数据]</td> 
   <td>映射要转换的文件。 如果您在[！UICONTROL源文件]字段中选择了映射，则此字段可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件名]</td> 
   <td>输入已转换文件的名称。 如果您在[！UICONTROL源文件]字段中选择了映射，则此字段可用。</td> 
  </tr> 
 </tbody> 
</table>

## 可能的问题

### 操作因错误而终止

在以下三种情况下，操作可能会因错误而终止：

* 接收的数据不是JPG/GIF/PNG/BMP格式
* 更改图像尺寸时，已超过最大宽度/高度限制。 图像大小不得超过3840像素宽度和2160像素高度
* 更改图像的尺寸或格式时，已超过图像允许的最大大小。
