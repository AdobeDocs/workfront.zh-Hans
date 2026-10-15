---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: 在Adobe云存储上迁移到Workfront
description: 规划如何在Adobe云存储上迁移到Workfront。 了解在启用您的组织后会发生什么情况、Adobe云存储对象上发生了什么变化以及如何根据您自己的时间将其推出。
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---
# 在Adobe云存储上迁移到Workfront

Adobe云存储上的Workfront提供了完整的统一审核和批准体验：Frame.io查看器中的审核、强大的批准工作流、资产的跨产品可见性等等。

本文是Workfront管理员迁移到Adobe云存储的起点。 它介绍了启用Adobe云存储时会发生的情况，向您介绍了各项更改的详细信息，并提供了指向有助于您规划和推广更改的各篇文章的链接。

## 由您决定Adobe云存储的打开时间

在Workfront管理员在&#x200B;**设置** > **系统** > **首选项**&#x200B;中启用Adobe云存储作为默认存储选项之前，Workfront环境不会发生任何变化。 在此之前，您现有的项目和创建的任何新项目将保留在旧版Workfront存储中，并保持您现在使用的审批服务。

当管理员启用Adobe云存储作为默认存储选项时：

* 新项目使用Adobe云存储
* Frame.io是默认查看器
* 统一审批是默认的审批服务

现有项目不会更改。

由于您可以控制时间，因此可以在任何人使用它之前测试体验、更新Workfront Fusion场景并规划报表更改。 有关分步说明，请参阅[为您的组织启用Adobe云存储](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)。

## 审批如何在Adobe云存储上工作

默认情况下，Adobe云存储项目使用统一批准，在Frame.io查看器中审核和批准。 保留在旧版Workfront存储中的对象会保留其已使用的任何审批服务：旧版文档审批或统一审批。

>[!NOTE]
>
>将Adobe云存储设置为默认不会更改已在您的旧版Workfront存储对象上使用的审批服务。 只有在Adobe云存储中创建的新对象，才会默认使用统一审批。

在推出Adobe云存储之前，请确保管理审批的人员知道会发生什么。 有关详细信息，请参阅[从旧文档审批移至统一审批](/help/quicksilver/review-and-approve-work/move-to-unified-approvals.md)。

## 规划您的移动

在准备时，请按顺序阅读这些文章：

* [在Adobe云存储上有什么不同之处](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md)：在Adobe云存储对象上，从新的“文档”区域和Frame.io查看器到命名规则、存储配额和Fusion，存在主要差异。
* [规划您的Adobe云存储转出](/help/quicksilver/review-and-approve-work/plan-adobe-cloud-storage-rollout.md)：如何选择转出配置、使用单个组进行试点，以及安排工作顺序，这样用户便不会感到意外。
* [为您的组织启用Adobe云存储](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)：为整个组织或特定组设置默认存储选项的步骤。
* [将旧对象转换为Adobe云存储](/help/quicksilver/review-and-approve-work/convert-objects-to-adobe-cloud-storage.md)：您可以将旧对象转换为Adobe云存储的三种情况，以及每次转换过程中将发生什么变化。


## 相关文章

* [Adobe cloud storage概述](/help/quicksilver/review-and-approve-work/esm-overview.md)
* [统一审查和批准概述](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [统一审查和批准入门](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [“文档”区域](/help/quicksilver/documents/managing-documents/documents-area.md)
* [Adobe云存储模型的对象权限和访问级别概述](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)
