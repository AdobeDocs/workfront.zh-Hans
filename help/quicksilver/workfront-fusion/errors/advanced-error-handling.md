---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 中的高级错误处理 [!DNL Adobe] Workfront Fusion
description: 高级错误处理技术包括过滤和嵌套。
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---

# 中的高级错误处理 [!DNL Adobe Workfront Fusion]

高级错误处理技术包括过滤和嵌套。

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
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 筛选

在错误处理程序路由上可以进行两种过滤。

* [向错误处理程序路由添加过滤器](#adding-a-filter-to-the-error-handler-route)
* [向错误处理程序路由添加路由器后跟过滤器](#adding-a-router-followed-by-filters-to-the-error-handler)

### 向错误处理程序路由添加过滤器

您可以使用过滤器控制错误处理程序路由处理哪些错误。 这样，您只能处理特定类型的错误。 如果错误未通过筛选器，则会将其视为没有为给定模块定义错误处理程序路由。

>[!INFO]
>
>**示例:**
>
>![](assets/filter-error-handling-350x238.png)

### 添加 [!UICONTROL 路由器] 后跟过滤器到错误处理程序

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>在本例中，错误发生在 [!UICONTROL 创建文件夹] 模块(A)，具有常规路由和错误处理程序路由。 后面是路由器，其中一条路由具有定义特定类型错误（发生数据错误）的过滤器，另一条路由是所有其他错误的默认路由。 第一条路由以 [!UICONTROL 恢复] 指令，该指令包含从模块A恢复方案的替代值([!UICONTROL 创建文件夹])，而第二条路由以 [!UICONTROL 回滚] 指令，该指令可立即停止方案执行。

请参阅 [处理中的错误 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) 有关各种错误类型的详细信息，请参阅 [!DNL Workfront Fusion] 进行流程和评估。

### 示例方案

您可以设置此示例情景，以了解这些过滤器如何用于错误处理。

使用现有 [!DNL Dropbox] 文件夹来上传文件，而不是创建新文件

如果您使用 [!UICONTROL 创建文件夹] 模块打开 [!DNL Dropbox] 并且已存在同名文件夹，则模块将引发数据错误，如下所示：

![](assets/dropbox-350x276.png)

完整方案：

![](assets/dropbox-scenario-350x190.png)

1. 的 [!UICONTROL 工具] > [!UICONTROL 设置变量] 模块包含文件夹名称
1. 的 [!UICONTROL HTTP] >[!UICONTROL 获取文件] 模块将获取需要上传到文件夹的文件
1. 的 [!UICONTROL Dropbox] >[!UICONTROL 创建文件夹] 如果文件夹已与模块中映射的文件夹同名，则模块会引发错误
1. 错误处理程序路由（透明气泡）包含用于过滤错误的路由器
1. 第一条路由是针对名为“数据错误”(Data Error)的指定类型错误（我们已知）：

   1. 如果发生数据错误，并且错误详细信息通过过滤器，则 [!UICONTROL Dropbox] >[!UICONTROL 列出文件夹模块中的所有文件/子文件夹] 列出了 [!DNL Dropbox]
   1. 后续过滤器与文件夹名称匹配
   1. 的 [!UICONTROL 恢复] 指令指定现有文件夹的文件夹ID和文件夹路径，方案执行将从 [!UICONTROL Dropbox] >[!UICONTROL 创建文件夹] 而不是尝试创建新文件夹，这次它会使用 [!UICONTROL 恢复] 指令将文件移动到下一个模块，并在现有文件夹中上传文件

1. 第二条路由适用于所有其他错误，并以 [!UICONTROL 回滚] 指令，该指令会导致立即停止方案

第5份声明的详细说明如下：

要在后续模块中使用现有文件夹([!UICONTROL 上传文件] )，则需要向模块添加错误处理程序路由，并获取要映射到的文件夹路径 [!UICONTROL 恢复] 指令模块如下：

![](assets/add-error-handler-route-350x113.png)

第一条路由上的筛选器设置为仅处理在具有相同名称的文件夹已存在时出现的特定错误（数据错误）：

![](assets/condition-350x327.png)

的 [!UICONTROL Dropbox] >[!UICONTROL 列出文件夹中的所有文件] 模块配置为返回目标文件夹中的所有文件夹。 以下过滤器仅传递我们最初尝试创建的过滤器（文件夹名称存储在33中）。 文件夹名称项):

![](assets/condition2-350x193.png)

最终， [!UICONTROL 恢复] 指令将文件夹路径作为失败模块的输出。 请注意，文件夹ID留空，因为“[!UICONTROL 上传文件]“模块：

![](assets/flow-control-350x190.png)

## 嵌套

无论模块位于何处，都可以在除路由器以外的所有模块上创建和实现错误处理程序路由。 因此，可以为已属于为另一个模块创建的现有错误处理程序路径的一部分的模块创建错误处理程序路径。

以下是嵌套错误处理程序路由的示例：

![](assets/nested-error-handling-route-350x174.png)

在此方案中，第二错误处理程序路由嵌套在第一错误处理程序路由下。 如果 [!UICONTROL Dropbox] >[!UICONTROL 创建文件夹模块] 如果遇到错误，则执行将移至Route 1(如果 [!UICONTROL 发生数据错误] 过滤器后，将执行下一个模块，然后执行 [!UICONTROL 恢复] 指令模块（如果未发生错误） [!UICONTROL Dropbox] >[!UICONTROL 列出所有文件/子文件夹] 在文件夹模块中。

但是，如果 [!DNL Dropbox] 模块，则执行将移至错误处理程序路由2，并以 [!UICONTROL 忽略] 指令。 的 [!UICONTROL 恢复指令] 在这种情况下，不会执行模块。

这是过滤和嵌套错误处理程序的组合。

