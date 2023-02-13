---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: “Workfront Fusion版本活动：2022年11月7日一周”
description: 本页介绍2022年11月7日这一周在Adobe Workfront Fusion中所做的所有增强。
author: Luke
feature: Product Announcements, Workfront Fusion
hidefromtoc: true
exl-id: 802db851-39bb-4f40-8a66-ecb8c8b3ced6
source-git-commit: 9aaba3062bc5d1166c37821a6a3216f7f1d965b1
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Workfront Fusion版本活动：2022年11月7日这一周

**Webhook队列优化**

Fusion的Webhook队列已在此版本中进行优化。 接受webhook的服务现在与排队和其他进程分开。 此更改使Fusion能够以更快、更一致的速率处理Webhook队列。

在实施此更改期间，我们能够更好地了解排队Webhook事件的预期日志处理时间。 Fusion的Webhook查看器页面应不早于1分钟。

要查看当前排队的Webhook事件，请在左侧导航中导航到Webhook。 分子中带数字的卡车图标表示该网页钩的队列事件。 单击卡车图标可查看已排队的事件。

![](assets/fusion-webhook-queue-1866x567.png)


**现在，将停用或删除未使用的Web挂接**

我们对Workfront Fusion处理未使用网络挂接的方式进行了一些更改。 现在，如果出现以下任一情况，将自动停用wWebhooks:

* 网页挂接已超过5天未连接到任何方案。
* Webhook仅用于不活动情景（已处于非活动状态超过30天）。

如果已停用的Web挂接未连接到任何方案并且处于停用状态超过30天，则会自动删除和取消注册这些挂接。
