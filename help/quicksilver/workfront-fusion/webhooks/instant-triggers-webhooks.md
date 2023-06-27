---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: 中的即时触发器(Webhook) [!DNL Adobe Workfront Fusion]
description: 许多服务都提供Webhook，以便在服务发生特定更改时即时发送通知。 若要处理这些通知，我们建议您使用即时触发器。 本文介绍Adobe Workfront Fusion中即时触发器的用途和功能。
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# 中的即时触发器(Webhook) [!DNL Adobe Workfront Fusion]

许多服务都提供Webhook，以便在服务发生特定更改时即时发送通知。 若要处理这些通知，我们建议您使用即时触发器。 您可以轻松地在以下位置识别这些内容： [!DNL Adobe Workfront Fusion] 由于它们的标记：

![](assets/instant-350x256.png)

如果服务不提供Webhook，则需要使用轮询触发器定期轮询服务。

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

## 查看webhook的队列

来自传入webhook的所有消息都存储在webhook的队列中。

1. 单击 **[!UICONTROL Webhook]** 在左侧的菜单中。
1. 查找要查看其队列的Webhook。
1. 单击带有Truck图标和已接收Webhook数量的按钮。

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >无论如何设置选项，传入webhook数据始终存储在队列中 [!UICONTROL 数据] 是保密的(详见 [中的方案设置面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md))。 一旦在场景中处理了数据，就会从系统中永久删除该数据。

## 计划即时触发器

如果您的方案包含即时触发器，则可以安排方案立即运行：

![](assets/schedule-setting-350x185.png)

在这种情况下，您的方案将在以下情况下立即运行： [!DNL Workfront Fusion] 接收来自服务的新数据。 执行场景后，将计算队列中等待的挂起Webhook的总量，场景执行的周期与存在挂起Webhook的周期相同，每个周期处理一个Webhook。 有关更多信息，请参阅 [场景执行、周期和阶段 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

>[!NOTE]
>
>* 周期与方案运行不同。 在1个场景运行中可以有多个周期。
>* 当您执行计划立即触发即时触发的方案时，将应用以下异常：
>
>     * 根据定价计划，两次执行之间的间隔不受最小间隔的限制。
>
>       例如，一旦场景完成执行，将再次检查webhook的队列。 如果存在任何挂起的Webhook，则场景将立即再次执行，并再次处理所有挂起的Webhook。
>   
>     * “最大循环数”方案设置将被忽略并设置为100，这意味着在单个方案执行期间不会处理超过100个挂起Webhook（每个周期处理1个事件）。
>


如果您使用任何其他计划设置，而不是 [!UICONTROL 立即]，则场景按您指定的时间间隔执行。 由于在该间隔内队列中可以收集到多个Webhook，因此建议设置 [[!UICONTROL 最大循环数]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) 设置为高于默认值1的值，以便在一个场景运行中处理更多webhook：

1. 单击 [!UICONTROL 方案设置] 图标 ![](assets/gear-icon-settings.png) 位于场景底部。
1. 在 **[!UICONTROL 方案设置]** 框中，键入数字 **[!UICONTROL 最大循环数]** 框，指示每次执行场景时要运行的队列中的Webhook数。

## 速率限制

当前的速率限制为每秒5个Webhook。 如果超过限制，则返回429状态代码。

## 非活动Webhook的到期

删除了超过120小时未分配给任何场景的webhook。

## Webhook负载

[!DNL Workfront Fusion] 将webhook有效负载存储30天。 在创建webhook有效负载超过30天后对其进行访问会导致错误»[!UICONTROL 无法从存储中读取文件。]”

## 错误处理

当场景中存在使用即时触发器的错误时，场景：

* 立即停止 — 当场景设置为运行时 [!UICONTROL 立即].
* 尝试3次不成功（3个错误）后停止 — 当场景设置为按计划运行时。

如果在场景执行期间发生错误，则在即时触发器的回滚阶段将webhook放回队列中。 在这种情况下，您可以修复场景并重新运行它。 有关更多信息，请参阅 [回滚](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) 在文章中 [场景执行、周期和阶段 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

如果您的场景中存在Webhook响应模块，则将错误发送到Webhook响应。 Webhook响应模块始终在最后执行(如果 [!UICONTROL 自动提交] 未启用方案设置中的选项)。 有关更多信息，请参阅 [响应Webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) 在文章中 [Webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## 自定义Webhook

您可以创建自己的Webhook。 有关更多信息，请参阅 [Webhook](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webhook停用

如果满足以下任一条件，Webhook将自动停用：

* webhook已超过5天未连接到任何场景
* webhook仅用于非活动场景，这些场景已非活动超过30天。

如果停用的Webhook未连接到任何场景并且处于停用状态超过30天，则会自动删除和取消注册。


