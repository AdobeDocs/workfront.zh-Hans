---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion中的聚合器模块
description: 聚合器模块是一种旨在将多捆数据合并到单个捆绑包中的模块。
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 948fe5fc249e0dcb04655f015c8e46493159c3ed
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的[!UICONTROL 聚合器]模块

聚合器模块是一种旨在将多捆数据合并到单个捆绑包中的模块。

有关模块类型的详细信息，请参阅[模块类型](../../workfront-fusion/modules/module-types.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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

+++

## [!UICONTROL 汇总]模块概述

执行[!UICONTROL 汇总]模块时，它将执行以下操作：

* 累计它在单个源模块操作期间收到的所有捆绑包。
* 输出一个包，其数组包含每个累积包的一个项。 数组项的内容取决于特定的[!UICONTROL 聚合器]模块及其设置。

下图显示了[!UICONTROL 聚合器]模块的典型设置：

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL Source Module]</p> </td> 
   <td> <p>捆绑聚合开始的模块。 源模块通常是输出一系列捆绑包的迭代器或搜索模块。</p><p>设置聚合器的源模块（并关闭聚合器的设置）时，源模块和聚合器模块之间的路由将封装在灰色区域中，以便您可以清楚地看到聚合的开始和结束。 
   </p> <p>有关迭代器的详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[！UICONTROL迭代器]模块</p> <p>有关搜索模块的详细信息，请参阅<a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">模块类型</a>中的搜索模块。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL目标结构类型]</p> </td> 
   <td> <p>（仅适用于[！UICONTROL数组汇总]模块。） 聚合数据的目标结构。 默认选项[！UICONTROL自定义]允许您选择应聚合到[！UICONTROL数组聚合器]的输出捆绑包的<code>Array </code>项中的项：</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>在[！UICONTROL Array aggregator]模块之后连接多个模块并返回模块的设置后，[！UICONTROL Target]结构类型下拉菜单将包含以下所有模块及其属于“集合数组”类型的字段，如[!DNL Slack] &gt;[！UICONTROL创建消息]模块的[！UICONTROL附件]字段所示：</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL聚合字段]</td> 
   <td>要包含在聚合器模块输出中的字段。</td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL分组依据]</p> </td> 
   <td> <p>借助[！UICONTROL Group by]字段，可将聚合器的输出拆分为多个组。 [！UICONTROL Group by]字段可以包含一个公式，该公式针对每个聚合器的输入包进行计算。 然后，聚合器为每个不同的公式值输出一个捆绑。 每个捆绑包包含两个项目：</p> 
    <ul> 
     <li><code>Key </code>包含非重复值。</li> 
     <li><code>Array </code>包含公式计算为<code>Key </code>值的捆绑包中的聚合数据。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>在空聚合后停止处理</p> </td> 
   <td> <p>默认情况下，即使没有捆绑包到达[！UICONTROL聚合]模块（例如，因为已在途中全部被过滤掉），[！UICONTROL聚合]模块也会输出聚合结果。 如果启用了选项[！UICONTROL Stop processing after an empty aggregation]，在这种情况下，[！UICONTROL Aggregator]模块将不会生成任何输出捆绑，并且流将停止。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>源模块与[!UICONTROL 聚合器]模块之间模块生成的捆绑包未由[!UICONTROL 聚合器]模块输出，因此流中的[!UICONTROL 聚合器]之后的模块无法访问这些捆绑包。 如果需要源模块和[!UICONTROL 聚合器]模块之间的模块输出的捆绑包中的任何数据，请确保在[!UICONTROL 聚合器]模块的设置中包含给定项（在[!UICONTROL 数组聚合器]模块设置的[!UICONTROL 聚合字段]字段中包含）。


## 聚合器如何工作的示例场景

此示例方案显示如何压缩所有电子邮件附件并将ZIP文件上传到[!DNL Dropbox]。

![](assets/dropbox-archive-350x87.png)

以下方案显示如何：

* 第一个模块监视接收电子邮件的邮箱： [!UICONTROL 电子邮件] >[!UICONTROL 监视电子邮件]触发器将输出包含项目`Attachments[]`的包，该项目是一个包含所有电子邮件附件的数组。

* 第二个模型迭代电子邮件的附件：[!UICONTROL 电子邮件] >[!UICONTROL 迭代附件]迭代器逐个从`Attachments[]`数组获取项目，然后作为单独的捆绑包进一步发送它们。

* 第三个模块聚合[!UICONTROL 电子邮件] >[!UICONTROL 迭代附件]模块输出的包： [!UICONTROL 存档] >[!UICONTROL 创建存档聚合]聚合它收到的所有包，并输出包含ZIP文件的单个包。

* 最后一个模块将生成的ZIP文件上载到[!DNL Dropbox]： [!DNL Dropbox] > [!UICONTROL 上载文件]从[!UICONTROL 存档] > [!UICONTROL 创建存档]模块获取ZIP文件并将其上载到[!DNL Dropbox]。



以下是[!UICONTROL 存档] > [!UICONTROL 创建存档]聚合器的示例设置：

![](assets/archive-create-an-archive-350x484.png)
