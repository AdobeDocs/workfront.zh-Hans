---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 中的数据结构 [!DNL Adobe Workfront Fusion]
description: 数据结构是一个文档，详细描述传输到Adobe Workfront Fusion的数据格式。 根据本文档，方案编辑器能够确定哪些模块返回或接收哪种类型的数据。 数据结构文档最常用于序列化/解析数据格式，如JSON、XML、CSV等。
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# 中的数据结构 [!DNL Adobe Workfront Fusion]

数据结构是详细描述要传输到的数据格式的文档 [!DNL Adobe Workfront Fusion]. 根据本文档，方案编辑器能够确定哪些模块返回或接收哪种类型的数据。 数据结构文档最常用于序列化/解析数据格式，如JSON、XML、CSV等。

您可以通过单击 [!UICONTROL 创建新数据结构] 按钮 [!UICONTROL 数据结构概述] 部分或需要数据结构规范的模块设置中。

支持的数据类型在 [[!UICONTROL 模块类型]](../../workfront-fusion/modules/module-types.md) 文章。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 数据结构生成器

数据结构并不总是需要创建。 您可以使用我们内置生成器中的模板来简化操作。 通过提供数据示例，生成器将根据您输入的数据示例自动创建数据结构。 然后，可以手动修改创建的数据结构。

![](assets/data-structure-generator-350x341.jpg)
