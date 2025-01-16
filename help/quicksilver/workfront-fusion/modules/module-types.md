---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 模块类型
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 0%

---

# 模块类型

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [模块概述](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/module-overview.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

A[!UICONTROL Adobe Workfront Fusion]将模块分为五种类型：操作模块、搜索模块、触发器模块、聚合器和迭代器。 聚合器和迭代器适用于高级方案。

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

## 操作模块

操作模块是最常见的模块类型。 典型操作模块会返回单个捆绑包，然后传递给下一个模块进行处理。

与触发器模块不同，操作模块可以放置在方案的开头、中间或结尾。 方案可以包含无限数量的操作模块。

>[!INFO]
>
>**示例：**
>
>* **[!DNL Workfront]> [!UICONTROL 上载文件]**&#x200B;将文件发送到[!DNL Workfront]并返回其标识符。
>* **[!UICONTROL 图像] > [!UICONTROL 调整大小]**&#x200B;接收图像，将其大小调整为指定的尺寸，然后将调整大小的图像传递到下一个操作。

“操作”类型有四个子类型：“创建”、“读取”、“更新”和“删除”。 Update子类型启用以下三个操作：

* **擦除字段**&#x200B;的内容。 当字段的内容被评估为擦除关键字（不要与&#x200B;*empty*&#x200B;混淆）时，将发生此操作。

  ![](assets/erase-content-of-field.png)

* **字段的内容保持不变**。 当字段留空或字段内容计算为空（在JSON中通过null表示）时，会发生此操作。

  ![](assets/leave-content-field-unchanged-350x231.png)

* **替换字段**&#x200B;的内容。 除上述两种情况外，此操作还会发生在所有其他情况下。

>[!NOTE]
>
>* 如果您在映射面板中未看到`erase`关键字，则该模块不是更新模块，或者未更新为应用程序的最新规范。
>* “[!UICONTROL Empty]”不会更改字段内容。 如果必须拭除该字段，可以使用以下公式：
>
>![](assets/formula-ifempty-name-erase.png)
>
>在字段的内容被评估为空时，当前无法保持该字段不变。

## 搜索模块

典型的搜索会返回零、一个或多个包，然后这些包将传递到下一个模块进行处理。

您可以将搜索放置在方案的开头、中间或结尾。

方案可以包含无限数量的搜索。

>[!INFO]
>
>**示例：**
>
>**[!DNL Workfront]> [!UICONTROL 读取相关记录]**&#x200B;读取在特定父对象中与指定的搜索查询匹配的记录

## 触发器模块

当给定服务发生更改时，触发器将生成捆绑包。 更改可以是创建新记录、删除记录、更新记录等。

每个触发器可以返回零、一个或多个包，这些包随后传递给下一个模块进行处理。

触发器只能在方案的开头放置。

每个方案只能包含一个触发器。

[!DNL Workfront Fusion]区分两种类型的触发器：轮询触发器和即时触发器。

### 轮询触发器

轮询触发器会定期轮询给定服务，即使自上次运行以来未发生任何更改。 我们建议您安排包含轮询触发器的方案定期运行。 如果存在&#x200B;*更改*，则触发器将返回包含有关更改信息的包。 如果没有&#x200B;*change*，则触发器不会输出任何包。 有关计划方案的说明，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md)中计划方案。

轮询触发器允许您选择它们应通过epoch面板输出的第一个包。 保存触发器或更改触发器设置后，面板会自动显示。 有关详细信息，请参阅[选择触发器模块在[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md)中的开始位置。

>[!NOTE]
>
>在Epoch面板中进行的设置仅影响模块的首次执行。 执行模块后，该模块会记住最后输出的捆绑，并撤消通过epoch面板所做的设置。

>[!INFO]
>
>**示例：**
>
>* **[!DNL Workfront]> [!UICONTROL 监视记录]**&#x200B;返回自上次运行方案以来新添加的文件
>
>* **[!DNL Google Sheets]> [!UICONTROL 观察行]**&#x200B;返回自上次运行方案以来用户添加的新行

### 即时触发器

即时触发器使服务能够立即通知[!DNL Workfront Fusion]有关&#x200B;*更改*&#x200B;的信息。 我们建议您安排一个包含即时触发器的方案立即运行。 有关说明，请参阅[在Adobe Workfront Fusion中计划方案](../../workfront-fusion/scenarios/schedule-a-scenario.md)。 另请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)中的[即时触发器(webhook)，以了解如何处理传入数据的详细信息。

>[!INFO]
>
>**示例：**
>
>* 在Workfront中发生特定类型的事件（如创建任务）时，**[!DNL Workfront]> [!UICONTROL 关注事件]**&#x200B;会返回信息。
>* 每当更新单元格时，**[!DNL Google Sheets]> [!UICONTROL 监视更改]**&#x200B;将返回信息。

## 汇总

聚合器是一种将多个捆绑累积到单个捆绑中的模块。

每个聚合器仅返回一个捆绑包，该捆绑包随后传递到下一个模块以供进一步处理。

只能将聚合放置在场景的中间位置。

方案可以包含无限数量的聚合器。

>[!INFO]
>
>**示例：**
>
>* **[!UICONTROL 存档] > [!UICONTROL 创建存档]**&#x200B;将接收的文件压缩为zip存档
>* **[!UICONTROL CSV] > [!UICONTROL 聚合到CSV]**&#x200B;将CSV文件中的多个字符串合并到一行
>* **[!UICONTROL 工具] > [!UICONTROL 文本聚合器]**&#x200B;将多个字符串组合为一个字符串

有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md)中的[聚合器模块。

## 迭代器

迭代器是一种将数组拆分为多个单独捆绑包的模块。

每个迭代器都会返回一个或多个包，然后这些包将传递到下一个模块进行处理。

只能将迭代器放置在场景的中间位置。

方案可以包含无限数量的迭代器。

>[!INFO]
>
>**示例：**
>
>**[!UICONTROL 电子邮件] > [!UICONTROL 检索附件]**&#x200B;将附件数组分成单独的包

有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)中的[迭代器模块和 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md)中的[映射数组。
