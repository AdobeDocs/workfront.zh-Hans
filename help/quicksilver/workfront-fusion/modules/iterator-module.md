---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion中的迭代器模块
description: 迭代器模块是一种特殊类型的模块，可将数组转换为一系列包。 每个数组项作为单独的束输出。
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: a2060e7179f2295bfd42da84bd7bca9862ad0a17
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# [!UICONTROL 迭代器] 模块 [!DNL Adobe Workfront Fusion]

安 [!UICONTROL 迭代器] 模块是一种特殊类型的模块，可将数组转换为一系列包。 每个数组项作为单独的束输出。

有关更多信息，请参阅 [模块类型](../../workfront-fusion/modules/module-types.md) 和 [在Adobe Workfront Fusion中映射数组](../../workfront-fusion/mapping/map-an-array.md).

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
   <td>贵组织必须购买Adobe Workfront Fusion和Adobe Workfront才能使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 迭代器] 模块配置

您设置 [!UICONTROL 迭代器] 模块。 的 [!UICONTROL 数组] 字段包含要转换或拆分为单独包的数组。

![](assets/set-up-iterator-350x190.jpg)

有关更多信息，请参阅 [在Adobe Workfront Fusion中配置模块设置](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**示例:**
>
>* 以下方案显示如何检索带有附件的电子邮件，并将附件另存为选定文件中的单个文件 [!DNL Dropbox] 文件夹。
   >
   >   电子邮件可以包含一组附件。 的 [!UICONTROL 迭代器] 插入到第一个模块之后的模块将允许您单独处理每个附件。 的 [!UICONTROL 迭代器] 模块将附件数组拆分为单个包。 每个带有一个附件的束，然后在选定的 [!DNL Dropbox] 文件夹。 的 [!UICONTROL 迭代器] 模块设置如上所示：the [!UICONTROL 数组] 字段应包含 `Attachments` 数组。
   >
   >   ![](assets/attachments-array-350x154.jpg)
>
>* 为方便起见，许多 [!DNL Workfront Fusion] 应用程序提供专用 [!UICONTROL 迭代器] 模块，并简化设置。 例如， [!UICONTROL 电子邮件] 应用程序包含特殊 [!UICONTROL 迭代器] 模块 [!UICONTROL 电子邮件] > [!UICONTROL 迭代附件] 会产生与将军相同的结果 [!UICONTROL 迭代器] 模块。
   >
   >   ![](assets/specialized-iterators-350x135.jpg)



## 疑难解答：“映射”面板不显示下方的可映射项目 [!UICONTROL 迭代器] 模块

当 [!UICONTROL 迭代器] 模块没有有关数组项结构的信息，在模块中的映射面板位于 [!UICONTROL 迭代器] 模块下仅显示2个项目 [!UICONTROL 迭代器] 模块：`Total number of bundles` 和 `Bundle order position`:

![](assets/mapping-panel-doesnt-display-350x147.png)

这是因为每个模块都负责提供有关其输出项目的信息，以便这些项目能够在后续模块的映射面板中正确显示。 但是，有些模块可能无法提供此信息；例如， [!UICONTROL JSON] > [!UICONTROL 解析JSON] 或 [!UICONTROL Webhooks] > [!UICONTROL 自定义Webhook] 缺少数据结构的模块。

解决方案是手动执行方案，使模块了解其输出的项目，以便它能够向以下模块提供信息。

例如，如果您的 [!UICONTROL JSON] > [!UICONTROL 解析JSON] 模块（不具有数据结构），如下所示：

![](assets/json-parse-json-350x285.png)

如果你连接 [!UICONTROL 迭代器] 模块，则无法将模块的输出映射到其设置面板中的Array字段 [!UICONTROL 迭代器] 模块：

![](assets/connect-iterator-module-350x146.png)

要解决此问题，请在方案编辑器中手动启动方案。 您可以在 [!UICONTROL JSON] > [!UICONTROL 解析JSON] 模块，以阻止流程进一步继续。 或者，您也可以右键单击 [!UICONTROL JSON] > [!UICONTROL 解析JSON] 模块和选择 **[!UICONTROL 仅运行此模块]** 从上下文菜单中，仅执行 [!UICONTROL JSON] > [!UICONTROL 解析JSON] 模块。

当 [!UICONTROL JSON] > [!UICONTROL 解析JSON] 执行后，它会了解它输出的项目并将此信息提供给所有后续模块，包括迭代器模块。 迭代器设置中的映射面板随后显示以下项目：

![](assets/mapping-panel-displays-items-350x131.png)

此外，在模块中的映射面板在 [!UICONTROL 迭代器] 模块显示数组项目中包含的项目：

![](assets/items-contained-in-array-350x156.png)

如果在模块的映射面板中看不到某些项目，请运行一次方案，以便所有模块都可以了解它们输出的项目，并将此信息提供给以下模块。
