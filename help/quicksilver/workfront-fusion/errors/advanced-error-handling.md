---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: ' [!DNL Adobe] Workfront Fusion中的高级错误处理'
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1031'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的高级错误处理

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [将筛选和嵌套添加到错误处理路由](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/advanced-error-handling.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

高级错误处理技术包括筛选和嵌套。

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

## 筛选

在错误处理程序路由中可能会进行两种筛选。

* [将过滤器添加到错误处理程序路由](#adding-a-filter-to-the-error-handler-route)
* [将路由器后跟过滤器添加到错误处理程序路由](#adding-a-router-followed-by-filters-to-the-error-handler)

### 将过滤器添加到错误处理程序路由

您可以使用过滤器来控制错误处理程序路由处理哪些错误。 这允许您仅处理特定类型的错误。 如果错误未通过过滤器，则会将其视为没有为给定模块定义错误处理程序路由。

>[!INFO]
>
>**示例：**
>
>![](assets/filter-error-handling-350x238.png)

### 正在将[!UICONTROL 路由器]后跟过滤器添加到错误处理程序

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>在此示例中，错误发生在[!UICONTROL 创建文件夹]模块(A)，该模块具有常规路由和错误处理程序路由。 后一种路由器具有定义特定错误类型（发生数据错误）的过滤器，而另一路由是所有其他错误的默认路由。 第一个路由以[!UICONTROL Resume]指令结束，该指令包含从模块A恢复的方案的替代值（[!UICONTROL 创建文件夹]），而第二个路由以[!UICONTROL Rollback]指令结束，该指令立即停止方案的执行。

有关各种错误类型以及[!DNL Workfront Fusion]如何处理并评估它们的详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md)中处理错误。

### 示例场景

您可以设置此示例场景，以了解这些过滤器如何用于错误处理。

使用现有[!DNL Dropbox]文件夹上传文件，而不是创建新文件

如果您在[!DNL Dropbox]上使用[!UICONTROL 创建文件夹]模块，并且已存在同名文件夹，则该模块将引发数据错误，如下所示：

![](assets/dropbox-350x276.png)

完整方案：

![](assets/dropbox-scenario-350x190.png)

1. [!UICONTROL 工具] > [!UICONTROL 设置变量]模块包含文件夹名称
1. [!UICONTROL HTTP] >[!UICONTROL 获取文件]模块会获取需要上载到文件夹的文件
1. 如果已存在与模块中映射的文件夹同名的文件夹，则[!UICONTROL Dropbox] >[!UICONTROL 创建文件夹]模块会引发错误
1. 错误处理程序路由（透明气泡）包含用于过滤错误的路由器
1. 第一条　路由用于我们已知的、名为“数据错误”的指定错误类型：

   1. 如果发生数据错误且错误详细信息通过筛选器，[!UICONTROL Dropbox] >[!UICONTROL 列出文件夹模块中的所有文件/子文件夹]将列出[!DNL Dropbox]中的所有文件夹
   1. 后续筛选器与文件夹名称匹配
   1. [!UICONTROL Resume]指令指定现有文件夹的文件夹ID和文件夹路径，方案执行从[!UICONTROL Dropbox] >[!UICONTROL 创建文件夹]模块继续，但这次它使用[!UICONTROL Resume]指令中的值移动到下一个模块并将文件上载到现有文件夹中，而不是尝试创建新文件夹

1. 第二个路由用于所有其他错误，并以[!UICONTROL Rollback]指令结束，该指令会导致立即停止该方案

第5个声明的详细说明如下：

若要在后续模块（[!UICONTROL 上传下面的文件]）中使用现有文件夹，您需要添加错误处理程序路由到模块，并获取要映射到[!UICONTROL Resume]指令模块的文件夹路径，如下所示：

![](assets/add-error-handler-route-350x113.png)

第一条　路由上的过滤器设置为仅处理同名文件夹已存在时出现的特定错误（数据错误）：

![](assets/condition-350x327.png)

[!UICONTROL Dropbox] >[!UICONTROL 列出文件夹]模块中的所有文件已配置为返回目标文件夹中的所有文件夹。 以下过滤器只审核我们最初尝试创建的过滤器（文件夹名称存储在33中）。 文件夹名称项目)：

![](assets/condition2-350x193.png)

最终，[!UICONTROL Resume]指令提供文件夹路径作为失败模块的输出。 请注意，文件夹ID已留空，因为“[!UICONTROL 上载文件]”模块不需要它：

![](assets/flow-control-350x190.png)

## 嵌套

无论模块位于何处，均可在除路由器之外的所有模块中创建和实施错误处理程序路由。 因此，可以为已经属于为其他模块创建的现有错误处理程序路由一部分的模块创建错误处理程序路由。

以下是嵌套错误处理程序路由的示例：

![](assets/nested-error-handling-route-350x174.png)

在此方案中，第二个错误处理程序路由嵌套在第一个错误处理程序路由下。 因此，如果[!UICONTROL Dropbox] >[!UICONTROL 创建文件夹模块]遇到错误，则执行将移至Route 1；如果传递了[!UICONTROL 数据错误发生]筛选器，则在文件夹模块中的[!UICONTROL Dropbox] >[!UICONTROL 列出所有文件/子文件夹]未发生错误时，将依次执行下一个模块和[!UICONTROL Resume]指令模块。

但是，如果此[!DNL Dropbox]模块发生错误，则执行将移至错误处理程序路由2并以[!UICONTROL Ignore]指令结束。 在这种情况下，未执行[!UICONTROL Resume指令]模块。

这是过滤和嵌套错误处理程序的组合。

