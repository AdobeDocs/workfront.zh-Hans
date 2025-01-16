---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Workfront Fusion中的流量控制
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Adobe Workfront Fusion中的流量控制

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [流量控制](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/flow-control.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

创建或编辑场景时，您可以配置设置以控制数据流经场景的方式。

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td>
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## 中继器

您可以使用[!UICONTROL 中继器]模块按指定次数重复执行任务。 [!UICONTROL 中继器]模块逐个生成包。

例如，您可以通过将&#x200B;**[!UICONTROL 电子邮件] >[!UICONTROL 向我发送电子邮件]**&#x200B;模块连接到[!UICONTROL 中继器]模块，使用[!UICONTROL 中继器]模块发送主题为“Hello 1”、“Hello 2”等的五封电子邮件。

要使用[!UICONTROL 中继器]模块：

1. 单击屏幕底部的[!UICONTROL 流量控制]图标![](assets/flow-control-icon.gif)，然后在显示的菜单中单击&#x200B;**[!UICONTROL 中继器]**。
1. 单击[!UICONTROL 中继器]包，然后在显示的框中单击&#x200B;**[!UICONTROL 自动连接]**。
1. 在出现的[!UICONTROL 流量控制]框中，在&#x200B;**[!UICONTROL 重复]**&#x200B;框中键入所需的重复（输出包）数。

   在我们的电子邮件示例中，您将键入5。

   ![](assets/repeater-2-350x207.png)

   每次重复时，该项的值将增加在&#x200B;**[!UICONTROL 步骤]**&#x200B;字段中指定的值，您可以通过选择&#x200B;**[!UICONTROL 显示高级设置]**&#x200B;来查看该字段。 默认情况下，此数字为1。

1. 单击&#x200B;**[!UICONTROL 确定]**&#x200B;以关闭&#x200B;**[!UICONTROL 流量控制]**&#x200B;框。

1. 单击连接到[!UICONTROL 中继器]模块的应用或服务模块。
1. 在出现的框中，键入要重复的信息。

   在我们的电子邮件示例中，您可以在[!UICONTROL 主题]框中键入Hello，然后从中继器模块映射`i`。

   ![](assets/repeater-3-350x207.png)

| 项 | 描述 |
|---|---|
| [!UICONTROL 初始值] | 输入或映射您希望模块在第一个迭代中设置为`i`的数字。 默认值为1。 |
| [!UICONTROL 重复] | 输入或映射您希望模块重复执行的次数。 此数字必须大于或等于0，并且小于或等于10,000。 |
| [!UICONTROL 步骤] | 这是模块增加`i`值所依据的数字。 默认值为1。 |

{style="table-layout:auto"}

>[!NOTE]
>
>重复次数不是由`i`的值确定的，因为它在编程中处于循环中。 模块将重复[!UICONTROL 重复]字段中指示的次数。 值`i`随[!DNL repeater]模块的每个迭代而更改，可以映射到以后的模块。 上面的示例将`i`的值映射到Hello消息中，从而生成显示“Hello 1”、“Hello 2”等的消息。

## [!UICONTROL 迭代器]

[!UICONTROL 迭代器]是一种将数组转换为一系列捆绑的特殊模块类型。 在[!UICONTROL 迭代器]模块输出中，每个数组项都将是一个单独的捆绑包。 有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)中的[[!UICONTROL 迭代器]模块。

## 数组汇总

数组聚合器是一种特殊类型的模块，允许将多个捆绑合并为一个捆绑包。 有关详细信息，请参阅Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md)中的[[!UICONTROL 聚合器]模块。

## [!UICONTROL 路由器]

[!UICONTROL 路由器]模块允许您将流量分为多条路由，并以不同的方式处理每条路由中的数据。 一旦[!UICONTROL 路由器]模块收到捆绑包，它会按照路由连接到[!UICONTROL 路由器]模块的顺序将其转发到每个连接的路由。 有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md)中的[路由器模块。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
