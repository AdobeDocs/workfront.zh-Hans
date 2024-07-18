---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: MIME模块
description: 您可以在Adobe Workfront Fusion中使用MIME类型。 多用途Internet邮件扩展(MIME)类型是允许软件识别在Internet上共享的不同类型数据的标签。 Web服务器和浏览器使用MIME类型来确定应该对文件执行的操作。 例如，具有MIME类型text/html的文件在浏览器中的处理方式与MIME类型image/jpeg的文件有所不同。 MIME类型独立于操作系统和硬件。
author: Becky
feature: Workfront Fusion
exl-id: ebbf6ad0-a1d0-47f8-849f-7bba1e0763d3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# [!UICONTROL MIME]模块

您可以在Adobe Workfront Fusion中使用MIME类型。 多用途Internet邮件扩展(MIME)类型是允许软件识别在Internet上共享的不同类型数据的标签。 Web服务器和浏览器使用MIME类型来确定应该对文件执行的操作。 例如，在浏览器中处理MIME类型为`text/html`的文件的方式与MIME类型为`image/jpeg`的文件的方式不同。 MIME类型独立于操作系统和硬件。

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

## [!UICONTROL MIME]模块及其字段

### [!UICONTROL 获取MIME类型]

此转换器模块返回与给定名称、路径或扩展名关联的MIME类型。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件]</td> 
   <td> <p>输入或映射要为其确定MIME类型的文件。 </p> <p>您可以使用以下方式输入文件：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL文件路径]</strong> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>/file/image.jpeg</p> </li> 
     <li><strong>[！UICONTROL文件名]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例：</b></span></span>image.jpeg</p> </li> 
     <li><strong>[！UICONTROL文件扩展名]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例：</b></span></span>jpeg</p> </li> 
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
   <td role="rowheader">[！UICONTROL MIME类型]</td> 
   <td> <p>输入或映射要确定其文件扩展名的MIME类型。 </p> </td> 
  </tr> 
 </tbody> 
</table>
