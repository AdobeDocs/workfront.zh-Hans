---
title: 2025年第二季度发布时间范围内的其他增强功能
description: 2025年第二季度发布时间框架内的其他增强功能
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 214f0e67-1da4-4abd-b942-09889e8bd92b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/s8T1ziXqzEOn8yipB5UdM-nShwJhYbCPNfIycC3GjYw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 335
ht-degree: 5%

---

# 2025年第二季度发布时间范围内的其他增强功能

本页介绍了在2025年第二季度版本中对“预览”环境所做的增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2025年第二季度发布周期中此时可用的所有更改列表，请参阅[&#x200B; 2025年第二季度发布概述](/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-release-overview.md)。

## 升级到具有版本升级端点的新事件订阅版本

>[!NOTE]
>
>适用于所有客户的生产： 2025年3月6日

Workfront现在提供各个版本的事件订阅。 该新版并未更改 Workfront API，而是更新了事件订阅功能。

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
