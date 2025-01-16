---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: ' [!DNL Adobe Workfront Fusion]中的即时触发器(Webhook)'
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的即时触发器(Webhook)

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [即时触发器(webhook)](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/webhooks-reference.html)
>* [查看webhook的队列](https://experienceleague.adobe.com/docs/workfront-fusion/using/manage-scenarios/view-webhook-queue.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

许多服务都提供Webhook，以便在服务发生特定更改时即时发送通知。 若要处理这些通知，我们建议您使用即时触发器。 您可以在[!DNL Adobe Workfront Fusion]中轻松识别这些内容，因为其标记为：

![](assets/instant-350x256.png)

如果服务不提供Webhook，则需要使用轮询触发器定期轮询服务。

有关Workfront Fusion中Webhook的视频介绍，请参阅：

* [Webhook简介](https://video.tv.adobe.com/v/3427025/){target=_blank}
* [中间Webhook](https://video.tv.adobe.com/v/3427030/){target=_blank}

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

## 查看webhook的队列

来自传入webhook的所有消息都存储在webhook的队列中。

1. 单击左侧菜单中的&#x200B;**[!UICONTROL Webhooks]**。
1. 查找要查看其队列的Webhook。
1. 单击带有卡车图标和已接收Webhook数量的按钮。

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >传入webhook数据始终存储在队列中，无论您如何设置选项[!UICONTROL 数据]是机密的（在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)中的[方案设置面板中介绍）。 一旦在场景中处理数据，就会从系统中永久删除该数据。

## 计划即时触发器

如果您的方案包含即时触发器，则可以安排方案立即运行：

![](assets/schedule-setting-350x185.png)

在这种情况下，当[!DNL Workfront Fusion]收到来自服务的新数据时，您的方案将立即运行。 执行场景后，将计算队列中等待的挂起webhook的总量，场景执行的周期与挂起webhook的数量相同，每个周期处理一个webhook。 有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)中的[方案执行、周期和阶段。

>[!NOTE]
>
>* 循环与方案运行不同。 在1个场景运行中可以有多个周期。
>* 当您执行计划立即触发的即时触发器方案时，将应用以下例外：
>
>     * 根据定价计划，两次执行之间的间隔不受最小间隔的限制。
>
>       例如，一旦场景完成执行，将再次检查webhook的队列。 如果存在任何挂起的Webhook，则场景将立即再次执行，并再次处理所有挂起的Webhook。
>   
>     * 将忽略“最大循环数”方案设置并设置为100，这意味着在单个方案执行期间处理挂起的网页挂接不超过100个（每个循环处理1个事件）。
>


如果您使用[!UICONTROL 立即]以外的任何其他计划设置，则方案将以您指定的时间间隔执行。 由于在该间隔内队列中可以收集到多个Webhook，因此建议将[[!UICONTROL 最大循环数]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum)设置为比默认值1更高的值，以便在一次方案运行中处理多个Webhook：

1. 单击方案底部的[!UICONTROL 方案设置]图标![](assets/gear-icon-settings.png)。
1. 在出现的&#x200B;**[!UICONTROL 方案设置]**&#x200B;框中，在&#x200B;**[!UICONTROL 最大循环数]**&#x200B;框中键入一个数字，以指示每次执行方案时要从队列中运行的Webhook数。

## 速率限制

当前的速率限制为每秒5个Webhook。 如果超过限制，将返回429状态代码。

## 非活动Webhook的到期

删除了超过120小时未分配给任何场景的webhook。

## Webhook负载

[!DNL Workfront Fusion]存储webhook负载30天。 创建webhook有效负载超过30天后对其进行访问会导致错误“[!UICONTROL 无法从存储中读取文件。]”

## 错误处理

当使用即时触发器的方案中存在错误时，该方案：

* 立即停止 — 方案设置为立即运行[!UICONTROL 时]。
* 尝试3次不成功（3个错误）后停止 — 场景设置为按计划运行时。

如果在场景执行期间发生错误，则在即时触发器的回滚阶段会将webhook重新放入队列。 在这种情况下，您可以修复场景并重新运行。 有关详细信息，请参阅[方案执行、循环和 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)中的阶段一文中的[回滚](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback)。

如果您的场景中存在Webhook响应模块，则将错误发送到Webhook响应。 Webhook响应模块始终在最后执行（在Scenario设置中的[!UICONTROL Auto commit]选项未启用的情况下）。 有关详细信息，请参阅文章[Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)中的[响应Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi)。

## 自定义Webhook

您可以创建自己的Webhook。 有关详细信息，请参阅[Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)。

## Webhook停用

如果出现以下任一情况，Webhook将自动停用：

* webhook已超过5天未连接到任何场景
* webhook仅用于非活动场景，这些场景已非活动超过30天。

如果停用的Webhook未连接到任何场景并且已处于停用状态超过30天，则会自动删除和取消注册它们。


