---
title: 2025年第二季度发布时间范围内的其他增强功能
description: 2025年第二季度发布时间框架内的其他增强功能
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 214f0e67-1da4-4abd-b942-09889e8bd92b
source-git-commit: d603edee0099b6ce3e4f8d3414d1b31f94209196
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# 2025年第二季度发布时间范围内的其他增强功能

本页介绍了在2025年第二季度版本中对“预览”环境所做的增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2025年第二季度发布周期中此时可用的所有更改列表，请参阅[ 2025年第二季度发布概述](/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-release-overview.md)。

## 升级到具有版本升级端点的新事件订阅版本

>[!NOTE]
>
>适用于所有客户的生产： 2025年3月6日

Workfront现在提供各个版本的事件订阅。 新版本不是对Workfront API的更改，而是对事件订阅功能的更改。

升级或降级事件订阅的功能确保在对事件结构做出更改时，现有订阅不会中断，从而允许您测试和升级到新版本，而不会在事件订阅中出现间隙。

有关两个版本之间差异的更多信息，请参阅文章[事件订阅版本控制](/help/quicksilver/wf-api/general/event-subs-versioning.md)。

有关用于在版本之间升级或降级事件订阅的端点的信息，请参阅事件订阅API一文中的[事件订阅版本控制](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning)部分。

## 在Workfront更新信息源中将Adobe Admin Console用户更改表示为“系统”

>[!NOTE]
>
>预览版本： 2025年1月23日；用于快速发布的生产：用于25.2版（2025年2月13日）；用于季度发布的生产：用于25.4版（2025年4月）

现在，当Adobe Admin Console管理员更改Workfront用户的用户信息时，Workfront将这一更改记录在用户更新区域的System activity （系统活动）选项卡中，并归入“System”（系统）。 此联系人为Adobe Admin Console管理员。

在此更新之前，Admin Console管理员对用户所做的更改将记录为Workfront主要系统管理员所做的更改。

有关在Adobe Admin Console中管理用户的信息，请参阅[在Adobe Admin Console中管理用户](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)
