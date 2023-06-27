---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion中的聚合器模块
description: 聚合器模块是一种旨在将多包数据合并到单个包中的模块。
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# [!UICONTROL 汇总] 中的模块 [!DNL Adobe Workfront Fusion]

聚合器模块是一种旨在将多包数据合并到单个包中的模块。

有关模块类型的更多信息，请参阅 [模块类型](../../workfront-fusion/modules/module-types.md).

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

## [!UICONTROL 汇总] 模块

当 [!UICONTROL 汇总] 模块执行，它执行以下操作：

* 累计它在单个源模块操作期间收到的所有包。
* 输出一个包，其数组包含每个累积包的一个项。 数组项目的内容取决于特定的 [!UICONTROL 汇总] 模块及其设置。

下图显示了 [!UICONTROL 汇总] 模块：

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL源模块]</p> </td> 
   <td> <p>包聚合将从中启动的模块。 源模块通常是输出一系列捆绑包的迭代器或搜索模块。 设置聚合器的源模块（并关闭聚合器的设置）时，源模块和聚合器模块之间的路由将封装在灰色区域中，以便您可以清楚地看到聚合的开始和结束。 
   </p> <p>有关迭代器的详细信息，请参见 <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">中的[！UICONTROL Iterator]模块 [!DNL Adobe Workfront Fusion]</a></p> <p>有关搜索模块的更多信息，请参阅中的搜索模块。 <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">模块类型</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL目标结构类型]</p> </td> 
   <td> <p>（仅适用于[！UICONTROL Array aggregator]模块。） 数据应汇总到的目标结构。 默认选项[！UICONTROL自定义]允许您选择应聚合到A[！UICONTROL数组聚合器]的输出捆绑包中的项 <code>Array </code>项目：</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>在[！UICONTROL Array aggregator]模块之后连接多个模块并返回模块的设置后，[！UICONTROL Target]结构类型下拉列表将包含以下所有模块及其属于集合数组类型的字段，如的[！UICONTROL Attachments]字段中所示 [!DNL Slack] &gt;[！UICONTROL创建消息]模块：</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL聚合字段]</td> 
   <td>选择要包含在聚合器模块输出中的字段。</td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL分组依据]</p> </td> 
   <td> <p>借助[！UICONTROL Group by]字段，可将聚合器的输出拆分为多个组。 [！UICONTROL Group by]字段可以包含为每个聚合器的输入包求值的公式。 然后，聚合器为每个不同的公式值输出一个捆绑。 每个捆绑包包含两个项目：</p> 
    <ul> 
     <li><code>Key </code>包含不同的值。</li> 
     <li><code>Array </code>包含经过公式计算的捆绑包中的聚合数据 <code>Key </code>值。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>在空聚合后停止处理</p> </td> 
   <td> <p>默认情况下，[！UICONTROL聚合]模块输出聚合结果，即使没有捆绑包到达[！UICONTROL聚合]模块也是如此（例如，因为已在途中过滤掉所有捆绑包）。 如果启用了选项[！UICONTROL Stop processing after an empty aggregator]，在这种情况下，[！UICONTROL Aggregator]模块将不会生成任何输出捆绑包，并且流将停止。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>源模块与模块之间生成的包 [!UICONTROL 汇总] 模块不由输出 [!UICONTROL 汇总] 模块，因此它们不可由流中的模块在访问 [!UICONTROL 汇总]. 如果您需要源模块与之间的模块输出的包中的任何数据， [!UICONTROL 汇总] 模块中，确保将给定项目包含在 [!UICONTROL 汇总] 模块的设置(与 [!UICONTROL 聚合字段] 字段。 [!UICONTROL 数组汇总] 模块)。


>[!INFO]
>
>**示例：** 用例：压缩所有电子邮件附件并将ZIP上传到 [!DNL Dropbox]
>
>以下方案显示如何：
>
>* 监视接收电子邮件的邮箱： [!UICONTROL 电子邮件] >[!UICONTROL 观看电子邮件] 触发器将输出一个包含项目的捆绑包 `Attachments[]`，这是一个包含所有电子邮件附件的数组。
>
>* 迭代电子邮件的附件： [!UICONTROL 电子邮件] >[!UICONTROL 迭代附件] 迭代器从以下位置获取项目： `Attachments[]` 逐个数组并将它们作为单独的捆绑包进一步发送。
>
>* 聚合以下项输出的包： [!UICONTROL 电子邮件] >[!UICONTROL 迭代附件] 模块： [!UICONTROL 存档] >[!UICONTROL 创建存档汇总] 累计它收到的所有包，并输出包含ZIP文件的单个包。
>
>* 将生成的ZIP文件上传到 [!DNL Dropbox]： [!DNL Dropbox] > [!UICONTROL 上传文件] 从获取ZIP文件 [!UICONTROL 存档] > [!UICONTROL 创建存档] 模块并将其上传到 [!DNL Dropbox].
>
>![](assets/dropbox-archive-350x87.png)
>
>以下是的示例设置 [!UICONTROL 存档] > [!UICONTROL 创建存档] 汇总：
>
>![](assets/archive-create-an-archive-350x484.png)
