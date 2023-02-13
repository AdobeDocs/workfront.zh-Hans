---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion中的聚合模块
description: 聚合器模块是一种模块类型，旨在将多个数据包合并到单个数据包中。
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '752'
ht-degree: 0%

---

# [!UICONTROL 聚合器] 模块 [!DNL Adobe Workfront Fusion]

聚合器模块是一种模块类型，旨在将多个数据包合并到单个数据包中。

有关模块类型的更多信息，请参阅 [模块类型](../../workfront-fusion/modules/module-types.md).

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

## [!UICONTROL 聚合器] 模块

当 [!UICONTROL 聚合器] 模块执行时，会执行以下操作：

* 在单个源模块的操作期间，累积它接收的所有包。
* 输出单个包，其中数组包含每个累积包一个项。 数组项目的内容取决于特定 [!UICONTROL 聚合器] 模块及其设置。

下图显示了 [!UICONTROL 聚合器] 模块：

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL源模块]</p> </td> 
   <td> <p>将从中启动捆绑聚合的模块。 源模块通常是输出一系列包的迭代器或搜索模块。 当您设置聚合器的源模块（并关闭聚合器的设置）时，源模块和聚合器模块之间的路由将封装在灰色区域中，以便您能够清楚地看到聚合的开始和结束。 
   </p> <p>有关迭代器的更多信息，请参阅 <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">中的[!UICONTROL迭代器]模块 [!DNL Adobe Workfront Fusion]</a></p> <p>有关搜索模块的更多信息，请参阅 <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">模块类型</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Target结构类型]</p> </td> 
   <td> <p>（仅适用于[!UICONTROL数组聚合器]模块。） 数据应汇总到的目标结构。 默认选项[!UICONTROL Custom]允许您选择应聚合到A[!UICONTROL Ray Aggregator]输出包中的项目 <code>Array </code>项目：</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>在[!UICONTROL Array aggregator]模块之后连接更多模块并返回到模块的设置后，[!UICONTROL Target]结构类型下拉列表将包含所有以下模块及其类型为“集合数组”的字段，如 [!DNL Slack] &gt;[!UICONTROL创建消息]模块：</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL聚合字段]</td> 
   <td>选择要包含在聚合模块输出中的字段。</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>借助[!UICONTROL Group by]字段，聚合器的输出可以拆分为多组。 [!UICONTROL Group by]字段可以包含一个公式，该公式将针对每个聚合器的输入包进行计算。 然后，聚合器为每个不同公式的值输出一个包。 每个包都包含两个项目：</p> 
    <ul> 
     <li><code>Key </code>包含非重复值。</li> 
     <li><code>Array </code>包含从公式计算到的包中的聚合数据 <code>Key </code>值。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>空聚合后停止处理</p> </td> 
   <td> <p>默认情况下，即使没有到达[!UICONTROL Aggregator]模块的包（例如，由于这些包在路途中被全部过滤掉），[!UICONTROL Aggregator]模块也会输出聚合结果。 如果启用了选项[!UICONTROL Stop processing an empty aggregation]（空聚合后停止处理），则[!UICONTROL Aggregator]模块在这种情况下不会生成任何输出包，并且流将停止。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>由源模块和 [!UICONTROL 聚合器] 模块不由 [!UICONTROL 聚合器] 模块，因此在 [!UICONTROL 聚合器]. 如果需要源模块与 [!UICONTROL 聚合器] 模块，请确保在 [!UICONTROL 聚合器] 模块的设置(如 [!UICONTROL 聚合字段] 字段 [!UICONTROL 阵列聚合器] 模块)。


>[!INFO]
>
>**示例：** 用例：压缩所有电子邮件附件并将ZIP上传到 [!DNL Dropbox]
>
>以下方案显示了如何：
>
>* 观看传入电子邮件的邮箱： [!UICONTROL 电子邮件] >[!UICONTROL 观看电子邮件] 触发器将输出包含项目的包 `Attachments[]`，这是一个包含所有电子邮件附件的数组。
>
>* 迭代电子邮件的附件： [!UICONTROL 电子邮件] >[!UICONTROL 迭代附件] 迭代器从 `Attachments[]` 逐个数组，并作为单独的包进一步发送它们。
>
>* 聚合由 [!UICONTROL 电子邮件] >[!UICONTROL 迭代附件] 模块： [!UICONTROL 存档] >[!UICONTROL 创建存档聚合器] 累积它接收的所有包，并输出包含ZIP文件的单个包。
>
>* 将生成的ZIP文件上传到 [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL 上传文件] 从 [!UICONTROL 存档] > [!UICONTROL 创建存档] 模块，并将其上传到 [!DNL Dropbox].
>
>![](assets/dropbox-archive-350x87.png)
>
>以下是 [!UICONTROL 存档] > [!UICONTROL 创建存档] 聚合：
>
>![](assets/archive-create-an-archive-350x484.png)
