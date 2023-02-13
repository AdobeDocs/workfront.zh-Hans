---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Workfront聚变中的流量控制
description: 创建或编辑方案时，您可以配置设置以控制数据通过方案的流动方式。
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 1%

---

# Adobe Workfront聚变中的流量控制

创建或编辑方案时，您可以配置设置以控制数据通过方案的流动方式。

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p>   <p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 中继器

您可以使用 [!UICONTROL 中继器] 模块，以按给定次数重复任务。 A [!UICONTROL 中继器] 模块会生成一个接一个的包。

例如，您可以使用 [!UICONTROL 中继器] 模块通过连接 **[!UICONTROL 电子邮件] >[!UICONTROL 给我发封电子邮件]** 模块 [!UICONTROL 中继器] 模块。

使用 [!UICONTROL 中继器] 模块：

1. 单击 [!UICONTROL 流量控制] 图标 ![](assets/flow-control-icon.gif) ，然后单击 **[!UICONTROL 中继器]** 中。
1. 单击 [!UICONTROL 中继器] 捆绑，然后单击 **[!UICONTROL 自动连接]** 框中。
1. 在 [!UICONTROL 流量控制] 框中，键入您希望在 **[!UICONTROL 重复]** 框中。

   在我们的电子邮件示例中，您需要键入5。

   ![](assets/repeater-2-350x207.png)

   项目的值会在每次重复时递增，此值在 **[!UICONTROL 步骤]** 字段，您可以通过选择 **[!UICONTROL 显示高级设置]**. 默认情况下，此数字为1。

1. 单击 **[!UICONTROL 确定]** 关闭 **[!UICONTROL 流量控制]** 框中。

1. 单击连接到 [!UICONTROL 中继器] 模块。
1. 在显示的框中，键入要重复的信息。

   在我们的电子邮件示例中，您应在 [!UICONTROL 主题] 框，然后映射 `i` 从中继器模块。

   ![](assets/repeater-3-350x207.png)

| 项 | 描述 |
|---|---|
| [!UICONTROL 初始值] | 输入或映射希望模块设置为的数字 `i` 在第一个小版本中。 默认值为1。 |
| [!UICONTROL 重复] | 输入或映射希望模块重复的次数。 此数字必须大于或等于0，且小于或等于10,000。 |
| [!UICONTROL 步骤] | 这是模块增加值时所依据的数字 `i`. 默认值为1。 |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
>
>重复次数不由 `i`，因为它在编程中处于循环中。 模块将重复 [!UICONTROL 重复] 字段。 值 `i` 每次迭代的更改 [!DNL repeater] 模块，并且可以映射到以后的模块。 上例将 `i` 在Hello消息中，生成的消息如下所示：“Hello 1”、“Hello 2”等。

## [!UICONTROL 迭代器]

安 [!UICONTROL 迭代器] 是一种特殊类型的模块，可将数组转换为一系列包。 每个数组项目将是 [!UICONTROL 迭代器] 模块输出。 有关更多信息，请参阅 [[!UICONTROL 迭代器] 模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## 阵列聚合器

阵列聚合器是一种特殊类型的模块，它允许将多个包合并到一个包中。 有关更多信息，请参阅 [[!UICONTROL 聚合器] Adobe Workfront Fusion中的模块](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL 路由器]

的 [!UICONTROL 路由器] 模块允许您将流量分支到多条路由中，并以不同方式处理每条路由中的数据。 一次 [!UICONTROL 路由器] 模块接收一个包，它将它转发给每个连接的路由，这些路由按路由附加到的顺序排列 [!UICONTROL 路由器] 模块。 有关更多信息，请参阅 [中的路由器模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
