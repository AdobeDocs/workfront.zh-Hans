---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 中的数据结构 [!DNL Adobe Workfront Fusion]
description: 数据结构是一个文档，它详细描述了传输到Adobe Workfront Fusion的数据的格式。 根据此文档，场景编辑器能够确定哪个模块返回或接收哪种类型的数据。 数据结构文档最常用于序列化/解析数据格式，如JSON、XML、CSV等。
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# 中的数据结构 [!DNL Adobe Workfront Fusion]

数据结构是一个文档，它详细描述了要传输到的数据的格式 [!DNL Adobe Workfront Fusion]. 根据此文档，场景编辑器能够确定哪个模块返回或接收哪种类型的数据。 数据结构文档最常用于序列化/解析数据格式，如JSON、XML、CSV等。

您可以通过单击 [!UICONTROL 创建新数据结构] 中的按钮 [!UICONTROL 数据结构概述] 部分，或者在需要数据结构规范的模块的设置中。

有关支持的数据类型，请参见 [[!UICONTROL 模块类型]](../../workfront-fusion/modules/module-types.md) 文章。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

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
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td>
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
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

## 数据结构生成器

数据结构并不总是必须创建的。 您可以使用内置生成器中的模板来简化操作。 通过提供数据示例，生成器将根据您输入的数据示例自动创建数据结构。 然后，可以手动修改创建的数据结构。

![](assets/data-structure-generator-350x341.jpg)
