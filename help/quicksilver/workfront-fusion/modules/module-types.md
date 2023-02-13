---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 模块类型
description: “Adobe Workfront Fusion”区分了五种模块：操作模块、搜索模块、触发器模块、聚合器和迭代器。 聚合器和迭代器适用于高级方案。
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 0%

---

# 模块类型

A[!UICONTROL Adobe Workfront Fusion] 区分五类模块：操作模块、搜索模块、触发器模块、聚合器和迭代器。 聚合器和迭代器适用于高级方案。

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

## 操作模块

操作模块是最常见的模块类型。 典型的操作模块会返回单个包，然后该包会传递到下一个模块进行处理。

与触发器模块不同，操作模块可以放置在方案的开头、中间或结尾。 方案可以包含无限数量的操作模块。

>[!INFO]
>
>**示例:**
>
>* **[!DNL Workfront]> [!UICONTROL 上传文件]** 将文件发送到 [!DNL Workfront] 并返回其标识符。
>* **[!UICONTROL 图像] > [!UICONTROL 调整大小]** 接收图像，将其调整为指定的尺寸，然后将调整后的图像传递到下一个操作。


操作类型有四种子类型：创建、读取、更新和删除。 “更新”子类型可启用以下三个操作：

* **擦除字段的内容**. 此操作在评估字段内容以删除关键词时进行(不要与 *空*)。

   ![](assets/erase-content-of-field.png)

* **保持字段内容不变**. 当字段留空或字段内容评估为空（在JSON中以空表示）时，将执行此操作。

   ![](assets/leave-content-field-unchanged-350x231.png)

* **替换字段的内容**. 此操作在上述两种情况以外的所有其他情况下进行。

>[!NOTE]
>
>* 如果您没有看到 `erase` 关键字，则该模块不是更新模块，或者尚未更新为应用程序的最新规范。
>* &quot;[!UICONTROL 空]“ ”不会更改字段内容。 如果需要擦除字段，可使用以下公式：
>
>![](assets/formula-ifempty-name-erase.png)
>
>当字段的内容评估为空时，当前不可能将其保留为不变。

## 搜索模块

典型的“搜索”返回零、一个或多个包，然后将这些包传递到下一个模块进行处理。

您可以在方案的开头、中间或结尾放置搜索。

方案可以包含无限数量的搜索。

>[!INFO]
>
>**示例:**
>
>**[!DNL Workfront]> [!UICONTROL 读取相关记录]**  读取与您指定的搜索查询（在特定父对象中）匹配的记录

## 触发器模块

当给定服务发生更改时，触发器会生成包。 更改可以是创建新记录、删除记录、更新记录等。

每个触发器都可以返回零个、一个或多个包，然后这些包会传递到下一个模块进行处理。

触发器只能放在方案的开头。

每个方案只能包含一个触发器。

[!DNL Workfront Fusion] 区分两种类型的触发器：轮询触发器和即时触发器。

### 轮询触发器

轮询触发器会定期轮询给定服务，即使自上次运行以来没有任何更改。 我们建议您安排包含轮询触发器的方案以定期运行。 如果存在 *更改*，触发器将返回包含有关更改信息的包。 如果没有 *更改*，则触发器不会输出任何包。 有关计划方案的说明，请参阅 [在中计划方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

轮询触发器允许您通过纪元面板选择它们应输出的第一个包。 在您保存触发器或更改触发器设置后，会自动显示该面板。 有关更多信息，请参阅 [选择触发器模块的开始位置 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>在纪元面板中所做的设置仅影响模块的首次执行。 一旦执行模块，它会记住最后输出的束，并撤消通过纪元面板进行的设置。

>[!INFO]
>
>**示例:**
>
>* **[!DNL Workfront]> [!UICONTROL 监视记录]** 返回自上次运行方案后新添加的文件
>
>* **[!DNL Google Sheets]> [!UICONTROL 监视行]** 返回自上次运行该方案后用户添加的新行


### 即时触发器

即时触发器使服务能够通知 [!DNL Workfront Fusion] 关于 *更改* 立即。 我们建议您安排包含即时触发器的方案立即运行。 有关说明，请参阅 [在Adobe Workfront Fusion中计划方案](../../workfront-fusion/scenarios/schedule-a-scenario.md). 另请参阅 [中的即时触发器(Webhook) [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) 有关如何处理传入数据的详细信息。

>[!INFO]
>
>**示例:**
>
>* **[!DNL Workfront]> [!UICONTROL 观看事件]** 在Workfront中发生特定类型的事件（如创建任务）时，会返回信息。
>* **[!DNL Google Sheets]> [!UICONTROL 监视更改]** 每当更新单元格时都会返回信息。


## 聚合器

聚合器是将多个包累加到一个包中的一种模块。

每个聚合器只返回一个包，然后该包传递到下一个模块以进一步处理。

您只能在方案的中间放置聚合器。

方案可以包含无限数量的聚合器。

>[!INFO]
>
>**示例:**
>
>* **[!UICONTROL 存档] > [!UICONTROL 创建存档]** 将收到的文件压缩为zip存档
>* **[!UICONTROL CSV] > [!UICONTROL 聚合到CSV]** 将多个字符串从CSV文件合并到一行中
>* **[!UICONTROL 工具] > [!UICONTROL 文本聚合器]** 将多个字符串组合在一起，形成一个字符串


有关更多信息，请参阅 [中的聚合器模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## 迭代器

迭代器是一种将数组拆分为多个单独包的模块类型。

每个迭代器返回一个或多个包，然后将包传递到下一个模块进行处理。

您只能将迭代器放置在方案的中间。

方案可以包含无限数量的迭代器。

>[!INFO]
>
>**示例:**
>
>**[!UICONTROL 电子邮件] > [!UICONTROL 检索附件]** 将附件数组分解为单独的包

有关更多信息，请参阅 [中的迭代器模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) 和 [在中映射数组 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
