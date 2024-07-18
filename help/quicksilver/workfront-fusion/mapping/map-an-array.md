---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 在 [!DNL Adobe] Workfront Fusion中映射数组
description: 您可以将数组映射到Adobe Workfront Fusion中的模块字段。
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中映射数组

数组是一种特殊类型的项，可以包含以下内容：

* 一个或多个文本值（简单数组）
* 同一类型（复杂数组）的一个或多个集合

>[!INFO]
>
>**示例：** [!UICONTROL 关注电子邮件]模块为每个电子邮件返回一个附件数组。 每个附件表示一个集合，该集合可能包含名称、内容、大小等。

有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)中的[项数据类型。

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

## 映射数组

1. 单击位于目标字段中的按钮。

   >[!INFO]
   >
   >  **示例：**&#x200B;对于上面的示例，您可以单击电子邮件的[!UICONTROL 添加附件]按钮。
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. 在显示的框中，输入项目。

   利用面板，可使用与映射任何其他类型项目相同的方式映射字段。 如果您不想单独填写每个项，但希望将另一个数组映射到目标字段，请使用[!UICONTROL 映射]按钮。 在这种情况下，请确保两个阵列（源阵列和目标阵列）具有相同的结构。

   可以将任意数量的项添加到数组。

您可以使用迭代器将数组划分为单独的包。 有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)中的[[!UICONTROL 迭代器]模块。
