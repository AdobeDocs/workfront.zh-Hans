---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 中的高级错误处理 [!DNL Adobe] Workfront Fusion
description: 高级错误处理技术包括筛选和嵌套。
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# 中的高级错误处理 [!DNL Adobe Workfront Fusion]

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

## 筛选

在错误处理程序路由上可能会进行两种过滤。

* [向错误处理程序路由添加过滤器](#adding-a-filter-to-the-error-handler-route)
* [向错误处理程序路由添加后跟过滤器的路由器](#adding-a-router-followed-by-filters-to-the-error-handler)

### 向错误处理程序路由添加过滤器

您可以使用过滤器来控制错误处理程序路由处理哪些错误。 这允许您仅处理特定类型的错误。 如果错误未通过过滤器，则会将其视为没有为给定模块定义错误处理程序路由。

>[!INFO]
>
>**示例:**
>
>![](assets/filter-error-handling-350x238.png)

### 添加 [!UICONTROL 路由器] 后跟错误处理程序的过滤器

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>在此示例中，错误发生在 [!UICONTROL 创建文件夹] 模块(A)，具有常规路由和错误处理程序路由。 后一个路由器后有一个路由，其中一条路由的过滤器定义特定类型的错误（发生数据错误），另一条是所有其他错误的默认路由。 第一条　路由以 [!UICONTROL 恢复] 指令，其中包含要从模块A恢复的方案的替代值([!UICONTROL 创建文件夹])，而第二条路由的结尾是 [!UICONTROL 回滚] 立即停止场景执行的指令。

参见 [处理以下对象时出错： [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) ，以了解有关各种错误类型及其使用方法的详细信息 [!DNL Workfront Fusion] 处理和评估它们。

### 示例场景

您可以设置此示例情景，以了解这些过滤器如何用于错误处理。

使用现有 [!DNL Dropbox] 文件夹以上传文件而不是创建新文件

如果您使用 [!UICONTROL 创建文件夹] 模块打开 [!DNL Dropbox] 并且已存在同名文件夹，模块将引发数据错误，如下所示：

![](assets/dropbox-350x276.png)

完整方案：

![](assets/dropbox-scenario-350x190.png)

1. 此 [!UICONTROL 工具] > [!UICONTROL 设置变量] 模块包含文件夹名称
1. 此 [!UICONTROL HTTP] >[!UICONTROL 获取文件] 模块会获取需要上传到文件夹的文件
1. 此 [!UICONTROL Dropbox] >[!UICONTROL 创建文件夹] 如果已存在与模块中映射的文件夹同名的文件夹，则模块会引发错误
1. 错误处理程序路由（透明气泡）包含用于过滤错误的路由器
1. 第一条　路由适用于我们已知的、名为“数据错误”的指定错误类型：

   1. 如果发生数据错误，并且错误详细信息通过过滤器，则 [!UICONTROL Dropbox] >[!UICONTROL 列出文件夹模块中的所有文件/子文件夹] 列出了中的所有文件夹 [!DNL Dropbox]
   1. 后续筛选条件与文件夹名称匹配
   1. 此 [!UICONTROL 恢复] 指令指定现有文件夹的文件夹ID和文件夹路径，场景执行从 [!UICONTROL Dropbox] >[!UICONTROL 创建文件夹] 模块，但此时它使用的不是尝试创建新文件夹，而是来自于 [!UICONTROL 恢复] 用于移到下一个模块并在现有文件夹中上传文件的指令

1. 第二个路由用于所有其他错误，并以 [!UICONTROL 回滚] 导致立即停止方案的指令

以下是第5个声明的详细说明：

要在后续模块中使用现有文件夹([!UICONTROL 上传文件] （如下所示），您需要添加指向模块的错误处理程序路由，并获取要映射到的文件夹路径 [!UICONTROL 恢复] 指令模块如下：

![](assets/add-error-handler-route-350x113.png)

第一条　路由上的过滤器设置为仅处理当同名文件夹已存在时出现的特定错误（数据错误）：

![](assets/condition-350x327.png)

此 [!UICONTROL Dropbox] >[!UICONTROL 列出文件夹中的所有文件] 模块配置为返回目标文件夹中的所有文件夹。 以下过滤器仅传递我们最初尝试创建的过滤器（文件夹名称存储在33中）。 文件夹名称项目)：

![](assets/condition2-350x193.png)

最终， [!UICONTROL 恢复] 指令提供文件夹路径作为故障模块的输出。 请注意，文件夹ID已留空，因为“[!UICONTROL 上传文件]&#39;模块：

![](assets/flow-control-350x190.png)

## 嵌套

无论模块位于何处，均可在除路由器之外的所有模块上创建和实施错误处理程序路由。 因此，可以为某个模块创建错误处理程序路由，该模块已经是为其他模块创建的现有错误处理程序路由的一部分。

以下是嵌套错误处理程序路由的示例：

![](assets/nested-error-handling-route-350x174.png)

在此方案中，第二个错误处理程序路由嵌套在第一错误处理程序路由下。 所以，如果 [!UICONTROL Dropbox] >[!UICONTROL 创建文件夹模块] 遇到错误，执行将移至Route 1 ，如果 [!UICONTROL 发生数据错误] 通过过滤器，执行下一个模块，然后执行 [!UICONTROL 恢复] 指令模块 [!UICONTROL Dropbox] >[!UICONTROL 列出所有文件/子文件夹] 在文件夹模块中。

但是，如果出现错误，则 [!DNL Dropbox] 模块中，然后执行移动到错误处理程序路由2并以以下内容结束 [!UICONTROL 忽略] 指令。 此 [!UICONTROL Resume指令] 在这种情况下，模块不会执行。

这是过滤和嵌套错误处理程序的组合。

