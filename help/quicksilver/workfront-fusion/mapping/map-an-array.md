---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 在中映射数组 [!DNL Adobe] Workfront Fusion
description: 您可以将数组映射到Adobe Workfront Fusion中的模块字段。
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# 在中映射数组 [!DNL Adobe Workfront Fusion]

数组是一种特殊类型的项目，可以包含以下内容：

* 一个或多个文本值（简单数组）
* 同一类型的一个或多个集合（复杂数组）

>[!INFO]
>
>**示例：** 的 [!UICONTROL 观看电子邮件] 模块会为每封电子邮件返回一个附件数组。 每个附件都表示一个可能包含名称、内容、大小等内容的集合。

有关更多信息，请参阅 [中的项目数据类型 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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

## 映射数组

1. 单击位于目标字段中的按钮。

   >[!INFO]
   >
   >  **示例：** 对于上例，您可以单击 [!UICONTROL 添加附件] 按钮。
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. 在显示的框中，输入项目。

   利用面板，可以像映射任何其他类型项目一样映射字段。 如果您不想单独填写每个项目，但想要将另一个数组映射到目标字段，请使用 [!UICONTROL 地图] 按钮。 在这种情况下，请确保两个数组（源数组和目标数组）具有相同的结构。

   您可以向数组中添加任意数量的项目。

您可以使用迭代器将数组分为单个包。 有关详细信息，请参阅 [[!UICONTROL 迭代器] 模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
