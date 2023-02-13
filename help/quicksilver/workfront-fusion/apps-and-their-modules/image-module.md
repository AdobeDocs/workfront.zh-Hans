---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 图像模块
description: Adobe Workfront融合图像模块允许您获取有关特定图像（尺寸、类型等）的信息，将图像转换为其他文件格式，并直接更改图像的大小。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 89efa9d5-00c9-4bb5-97b3-2b2f9d73721d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# 图像模块

[!DNL Adobe Workfront Fusion] [!UICONTROL 图像] 利用模块，可获取有关特定图像（尺寸、类型等）的信息，将图像转换为其他文件格式，并直接更改图像的大小。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p>  <p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 图像] 模块及其字段

配置此模块时，将显示以下字段。 模块中的粗体标题表示必填字段。

* [[!UICONTROL 调整大小]](#resize)
* [[!UICONTROL 转换格式]](#convert-a-format)
* [[!UICONTROL 提取元数据]](#extract-metadata)

### [!UICONTROL 调整大小]

此变压器模块会根据您指定的条件更改图像的高度和宽度。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>选择要转换的图像源。 您可以从上一个模块中选择输出，或映射数据文件和文件名。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL数据]</td> 
   <td>映射要转换的文件。 如果您在[!UICONTROL源文件]字段中选择了[!UICONTROL映射] ，则此字段将可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件名]</td> 
   <td>输入已转换文件的名称。 如果您在[!UICONTROL源文件]字段中选择了[!UICONTROL映射] ，则此字段将可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL，我想]</td> 
   <td>选择是要保持高宽比，还是要将尺寸更改为指定的高宽比。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arged to]</td> 
   <td> <p>选择您希望模块如何确定图像的新大小。 如果您选择在“我想要”字段中保持高宽比，则会显示此字段。 根据此字段中的选择显示其他字段。</p> 
    <ul> 
     <li> <p>[!UICONTROL最大宽度]</p> <p>将图像缩小到您指定的宽度。 高度会自动计算。</p> </li> 
     <li> <p>[!UICONTROL最大高度]</p> <p>将图像缩小到您指定的高度。 宽度会自动计算。</p> </li> 
     <li> <p>[!UICONTROL最大高度或宽度]</p> <p>减小图像的高度和宽度不会超过您指定的值。 由于此选项保持高宽比，因此其中一个尺寸可能小于指定尺寸。 例如，如果高度和宽度都指定为40，则400x300的图像将减小为40x30。</p> </li> 
     <li> <p>[!UICONTROL最小宽度]</p> <p>将图像放大到您指定的宽度。 高度会自动计算。</p> </li> 
     <li> <p>[!UICONTROL最小高度]</p> <p>将图像放大到您指定的高度。 宽度会自动计算。</p> </li> 
     <li> <p>[!UICONTROL最小高度或宽度]</p> <p>放大图像的方式为其高度和宽度不小于您指定的值。 由于此选项保持高宽比，因此其中一个尺寸可能大于指定尺寸。 例如，如果高度和宽度都指定为300，则40x30的图像将放大到400X300。</p> </li> 
     <li> <p>[!UICONTROL百分比]</p> <p>根据您指定的值，按百分比更改图像大小。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL宽度]</td> 
   <td>输入或映射大小调整后的图像所需的宽度（以像素为单位）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Height]</td> 
   <td>输入或映射大小调整后图像所需的高度（以像素为单位）。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 转换格式]

此变压器模块更改图像文件的格式。 此模块兼容以下格式：

* PNG
* JPG
* GIF
* BMP

源文件和输出都必须采用以下任一格式。 例如， [!UICONTROL 图像] >[!UICONTROL 转换格式] 模块可以将PNG文件转换为BMP文件，或将BMP转换为JPG。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>选择要转换的图像源。 您可以从上一个模块中选择输出，或映射数据文件和文件名。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL数据]</td> 
   <td>映射要转换的文件。 如果您在[!UICONTROL源文件]字段中选择了[!UICONTROL映射] ，则此字段将可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件名]</td> 
   <td>输入已转换文件的名称。 如果您在[!UICONTROL源文件]字段中选择了[!UICONTROL映射] ，则此字段将可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出格式]</td> 
   <td>选择您希望模块将源文件转换为的格式。 </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 提取元数据]

此变压器模块返回有关模块的基本信息。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>选择要转换的图像源。 您可以从上一个模块中选择输出，或映射数据文件和文件名。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL数据]</td> 
   <td>映射要转换的文件。 如果您在[!UICONTROL源文件]字段中选择了映射，则此字段将可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件名]</td> 
   <td>输入已转换文件的名称。 如果您在[!UICONTROL源文件]字段中选择了映射，则此字段将可用。</td> 
  </tr> 
 </tbody> 
</table>

## 可能的问题

### 操作终止，并出现错误

在以下三种情况下，操作可能会因错误而终止：

* 接收的数据不采用JPG/GIF/PNG/BMP格式
* 更改图像尺寸时，已超出最大宽度/高度限制。 图像大小不能超过3840像素宽度和2160像素高度
* 在更改图像的尺寸或格式时，已超出图像的最大允许大小。
