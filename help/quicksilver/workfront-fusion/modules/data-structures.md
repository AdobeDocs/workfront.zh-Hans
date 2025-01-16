---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: ' [!DNL Adobe Workfront Fusion]中的数据结构'
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的数据结构

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [创建和管理数据存储](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/data-stores.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

数据结构是详细说明要传输到[!DNL Adobe Workfront Fusion]的数据格式的文档。 根据此文档，场景编辑器能够确定哪个模块返回或接收哪种类型的数据。 数据结构文档最常用于序列化/解析数据格式，如JSON、XML、CSV等。

通过在[!UICONTROL 数据结构概述]部分或需要数据结构规范的模块的设置中单击[!UICONTROL 创建新数据结构]按钮，可以创建数据结构。

[[!UICONTROL 模块类型]](../../workfront-fusion/modules/module-types.md)文章中介绍了支持的数据类型。

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
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

## 数据结构生成器

数据结构并不总是必须创建的。 您可以使用内置生成器中的模板简化操作。 通过提供数据示例，生成器将根据您输入的数据示例自动创建数据结构。 然后，可以手动修改所创建的数据结构。

![](assets/data-structure-generator-350x341.jpg)
