---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Workfront Fusion中的流量控制
description: 创建或编辑场景时，您可以配置设置以控制数据流经场景的方式。
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 1%

---

# Adobe Workfront Fusion中的流量控制

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
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] （对于工作自动化和集成），[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p>
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

## 中继器

您可以使用 [!UICONTROL 中继器] 模块重复执行给定次数的任务。 A [!UICONTROL 中继器] 模块逐个生成包。

例如，您可以使用 [!UICONTROL 中继器] 模块发送主题为“Hello 1”、“Hello 2”等的五封电子邮件，通过连接 **[!UICONTROL 电子邮件] >[!UICONTROL 向我发送电子邮件]** 模块到 [!UICONTROL 中继器] 模块。

使用 [!UICONTROL 中继器] 模块：

1. 单击 [!UICONTROL 流量控制] 图标 ![](assets/flow-control-icon.gif) 单击屏幕底部，然后单击 **[!UICONTROL 中继器]** 在显示的菜单中。
1. 单击 [!UICONTROL 中继器] 捆绑，然后单击 **[!UICONTROL 自动连接]** 在显示的框中。
1. 在 [!UICONTROL 流量控制] 框中，键入所需的重复（输出包）数 **[!UICONTROL 重复]** 盒子。

   在我们的电子邮件示例中，您将键入5。

   ![](assets/repeater-2-350x207.png)

   每次重复时，项目的值都会增加到中指定的此值。 **[!UICONTROL 步骤]** 字段，您可以通过选择 **[!UICONTROL 显示高级设置]**. 默认情况下，此数字为1。

1. 单击 **[!UICONTROL 确定]** 关闭 **[!UICONTROL 流量控制]** 盒子。

1. 单击连接到应用程序或服务模块的 [!UICONTROL 中继器] 模块。
1. 在出现的框中，键入要重复的信息。

   在我们的电子邮件示例中，您应键入Hello [!UICONTROL 主题] 框，然后映射 `i` 中继器模块。

   ![](assets/repeater-3-350x207.png)

| 项 | 描述 |
|---|---|
| [!UICONTROL 初始值] | 输入或映射您希望模块设置为的数字 `i` 在第一个迭代中。 默认值为1。 |
| [!UICONTROL 重复] | 输入或映射您希望模块重复的次数。 此数字必须大于或等于0，并且小于或等于10,000。 |
| [!UICONTROL 步骤] | 这是模块增加值所依据的数字 `i`. 默认值为1。 |

{style="table-layout:auto"}

>[!NOTE]
>
>重复次数不由的值决定 `i`，因为它在编程中处于循环中。 模块将重复 [!UICONTROL 重复] 字段。 值 `i` 随的每次迭代更改 [!DNL repeater] 模块，并且可以映射到后续模块。 上面的示例映射了 `i` Hello消息，从而导致消息显示“Hello 1”、“Hello 2”等。

## [!UICONTROL 迭代器]

An [!UICONTROL 迭代器] 是一种特殊类型的模块，可将数组转换为一系列捆绑包。 每个数组项将作为 [!UICONTROL 迭代器] 模块输出。 有关更多信息，请参阅 [[!UICONTROL 迭代器] 中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## 数组汇总

数组聚合器是一种特殊类型的模块，允许将多个捆绑包合并到一个捆绑包中。 有关更多信息，请参阅 [[!UICONTROL 汇总] Adobe Workfront Fusion中的模块](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL 路由器]

此 [!UICONTROL 路由器] 模块允许您将流量分为多条路由，并在每条路由中以不同的方式处理数据。 一次 [!UICONTROL 路由器] 模块接收一个捆绑，然后按照将路由附加到的顺序将其转发到每个连接的路由。 [!UICONTROL 路由器] 模块。 有关更多信息，请参阅 [中的路由器模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
