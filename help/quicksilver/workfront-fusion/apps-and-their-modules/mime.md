---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: MIME模块
description: 您可以在Adobe Workfront Fusion中使用MIME类型。 多用途Internet邮件扩展(MIME)类型是允许软件识别在Internet上共享的不同类型数据的标签。 Web服务器和浏览器使用MIME类型来确定应对文件执行的操作。 例如，在浏览器中处理MIME类型为text/html的文件的方式与处理MIME类型为image/jpeg的文件的方式不同。 MIME类型的功能与操作系统和硬件无关。
author: Becky
feature: Workfront Fusion
exl-id: ebbf6ad0-a1d0-47f8-849f-7bba1e0763d3
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# [!UICONTROL MIME] 模块

您可以在Adobe Workfront Fusion中使用MIME类型。 多用途Internet邮件扩展(MIME)类型是允许软件识别在Internet上共享的不同类型数据的标签。 Web服务器和浏览器使用MIME类型来确定应对文件执行的操作。 例如，MIME类型为的文件 `text/html` 将在浏览器中以不同于MIME类型文件的方式处理 `image/jpeg`. MIME类型的功能与操作系统和硬件无关。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL MIME] 模块及其字段

### [!UICONTROL 获取MIME类型]

此转换器模块返回与给定名称、路径或扩展名关联的MIME类型。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件]</td> 
   <td> <p>输入或映射要确定其MIME类型的文件。 </p> <p>您可以使用以下方式输入文件：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL文件路径]</strong> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>/file/image.jpeg</p> </li> 
     <li><strong>[!UICONTROL文件名]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>image.jpeg</p> </li> 
     <li><strong>[!UICONTROL文件扩展名]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>jpeg</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 获取文件扩展名]

此转换器模块返回给定MIME类型的原始文件扩展名。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL MIME类型]</td> 
   <td> <p>输入或映射要确定其文件扩展名的MIME类型。 </p> </td> 
  </tr> 
 </tbody> 
</table>
