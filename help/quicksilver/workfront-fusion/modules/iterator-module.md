---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion中的迭代器模块
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的[!UICONTROL 迭代器]模块

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [迭代器模块](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/iterator-module.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

[!UICONTROL 迭代器]模块是一种特殊类型的模块，可将数组转换为一系列捆绑包。 每个数组项将作为单独的捆绑包输出。

有关详细信息，请参阅[模块类型](../../workfront-fusion/modules/module-types.md)和[在Adobe Workfront Fusion中映射数组](../../workfront-fusion/mapping/map-an-array.md)。

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
   <td>您的组织必须购买Adobe Workfront Fusion和Adobe Workfront，才能使用本文中所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## [!UICONTROL 迭代器]模块配置

您设置的[!UICONTROL 迭代器]模块与设置任何其他模块相同。 [!UICONTROL Array]字段包含要转换或拆分为单独捆绑的数组。

![](assets/set-up-iterator-350x190.jpg)

有关详细信息，请参阅[在Adobe Workfront Fusion中配置模块的设置](../../workfront-fusion/modules/configure-a-modules-settings.md)。

>[!INFO]
>
>**示例：**
>
>* 以下方案显示如何检索带有附件的电子邮件，并将附件另存为选定[!DNL Dropbox]文件夹中的单个文件。
>
>   电子邮件可以包含一系列附件。 在第一个模块之后插入的[!UICONTROL 迭代器]模块将允许您单独处理每个附件。 [!UICONTROL 迭代器]模块将附件数组拆分为单个包。 然后，每个带有一个附件的包都会在选定的[!DNL Dropbox]文件夹中一次保存一个。 上面显示了[!UICONTROL 迭代器]模块设置：[!UICONTROL 数组]字段应包含`Attachments`数组。
>
>   ![](assets/attachments-array-350x154.jpg)
>
>* 为方便起见，许多[!DNL Workfront Fusion]应用都提供了经过简化设置的专用[!UICONTROL 迭代器]模块。 例如，[!UICONTROL 电子邮件]应用包含特殊的[!UICONTROL 迭代器]模块[!UICONTROL 电子邮件] > [!UICONTROL 迭代附件]，这将产生与常规[!UICONTROL 迭代器]模块相同的结果。
>
>   ![](assets/specialized-iterators-350x135.jpg)


## 疑难解答：映射面板在[!UICONTROL 迭代器]模块下不显示可映射项

当[!UICONTROL 迭代器]模块没有有关数组项的结构信息时，[!UICONTROL 迭代器]模块后面的模块中的映射面板在[!UICONTROL 迭代器]模块下只显示2个项：`Total number of bundles`和`Bundle order position`：

![](assets/mapping-panel-doesnt-display-350x147.png)

这是因为每个模块负责提供有关其输出的项的信息，以便这些项目可以在后续模块的映射面板中正确显示。 但是，在某些情况下，多个模块可能无法提供此信息；例如，[!UICONTROL JSON] > [!UICONTROL 解析JSON]或[!UICONTROL Webhook] > [!UICONTROL 自定义Webhook]模块缺少数据结构。

解决方案是手动执行场景，使模块了解它输出的项目，以便它可以向以下模块提供信息。

例如，如果您的[!UICONTROL JSON] > [!UICONTROL 解析JSON]模块没有数据结构，如下所示：

![](assets/json-parse-json-350x285.png)

如果将[!UICONTROL 迭代器]模块连接到该模块，则无法将模块的输出映射到[!UICONTROL 迭代器]模块的设置面板中的Array字段：

![](assets/connect-iterator-module-350x146.png)

要解决此问题，请在方案编辑器中手动启动方案。 在[!UICONTROL JSON] > [!UICONTROL 解析JSON]模块后，您可以取消这些模块的链接，以防止流进一步继续。 或者，您可以右键单击[!UICONTROL JSON] > [!UICONTROL 解析JSON]模块，然后从上下文菜单中选择&#x200B;**[!UICONTROL 仅运行此模块]**&#x200B;以仅执行[!UICONTROL JSON] > [!UICONTROL 解析JSON]模块。

执行[!UICONTROL JSON] > [!UICONTROL 解析JSON]时，它会学习它输出的项目并将此信息提供给所有后续模块，包括迭代器模块。 然后，迭代器设置中的映射面板会显示以下项目：

![](assets/mapping-panel-displays-items-350x131.png)

此外，在[!UICONTROL 迭代器]模块之后连接的模块中的映射面板将显示数组的项中包含的项：

![](assets/items-contained-in-array-350x156.png)

如果在模块的映射面板中看不到某些项目，请运行场景一次，以便所有模块都可以了解它们输出的项目，并将此信息提供给以下模块。
