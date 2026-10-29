---
product-area: documents
navigation-topic: approvals
title: Adobe云存储有什么不同之处
description: 了解有关Adobe云存储对象的主要差异，包括新的“文档”区域、Frame.io查看器、文档权限、对象命名规则、存储配额和Workfront Fusion。
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 120abd12533cfed2e5c7f8c2f849d34a26054dbb
workflow-type: tm+mt
source-wordcount: '1714'
ht-degree: 0%
---
# Adobe云存储有什么不同之处

使用Adobe云存储时，您的环境可以包含两种类型的对象：旧版Workfront存储上的对象（您当前拥有的对象）和使用Adobe云存储创建的对象。 新的“文档”区域、Frame.io查看器和此处描述的其他行为仅适用于使用Adobe云存储的对象。

有关移动方向，请参阅[在Adobe云存储上移动到Workfront](/help/quicksilver/review-and-approve-work/workfront-storage.md)。

## 了解旧版Workfront存储和Adobe云存储

从较高层面看，这两种存储模式在数据所在的位置、哪些Adobe产品可以看到数据以及有哪些功能可用方面有所不同：

|  | 旧版Workfront存储中的对象 | Adobe云存储上的对象 |
|---|---|---|
| 存储后端 | 仅限Workfront | Adobe 云存储 |
| 跨产品可见性 | 仅限Workfront | Workfront、Frame.io和Creative Cloud |
| 功能 | 旧版功能 | 新功能 |

默认情况下，在Adobe云存储之前创建的对象将保留在旧版Workfront存储中。 本文中描述的行为仅适用于您和您的用户在将Adobe云存储设置为默认设置后创建的Adobe云存储对象。

## 差异摘要

Adobe云存储最大的日常更改是新的“文档”区域和Frame.io查看器，支持其中的审阅和批准。 还有其他差异会影响您管理对象、文档和审阅的方式。 下表中的每个区域均链接到下面的详细部分。

| 区域 | 不同之处 | 须知事项 |
|---|---|---|
| [新文档区域](#the-new-documents-area) | 重新设计、统一的“文档”区域取代了旧的“文档”区域。 | 没有全局文档区域。 您可以从项目、项目组合、项目、任务或问题访问文档。 |
| [文档权限](#document-permissions) | 文档从链接的项目、任务或问题继承权限。 | 您无法共享或设置单个文档的权限。 您可以通过Workfront中的对象共享模式来管理所有访问权限，该模式会级联到系统生成的文档文件夹。 |
| [对象权限映射](#object-permissions-mapping) | “管理”和“贡献”权限映射到Frame.io中的“编辑”和“共享”。 查看映射到“仅注释”。 | 您可以在Workfront中管理权限。 Manage和Contribute用户都可以在Frame.io中获得外部共享功能。 |
| [审阅和批准查看者](#review-and-approval-viewer) | Frame.io查看器将取代Workfront校对查看器。 | 它包含所有Workfront用户，包括分配给审阅或审批的外部用户。 它支持标记、带有时间戳的注释、版本历史记录、移动设备、40多种格式以及最大500 GB的文件。 |
| [对象命名规则](#object-naming-rules) | 适用严格的命名规则：项目组合或项目中的唯一名称、无特殊字符、无尾随句点或空格，以及255个字符的限制。 | 出现冲突时，Workfront会自动重命名对象。 审核生成新项目名称和结构的模板。 |
| [对象可移植性](#object-portability) | 在大多数情况下，您只能在类似存储模型之间移动、复制和转换对象。 | 您可以在三个特定情况下将旧版对象转换为Adobe云存储。 在转换过程中，文档和文档文件夹不会从旧存储中移动。 |
| [功能不可用](#capabilities-not-available-on-adobe-cloud-storage-objects) | Workfront Proof、Workfront文档查看器、收藏夹文档和请求文档不在体验中。 | 旧版对象保留这些功能。 Workfront Proof将不会获得新投资，并将在未来版本中停用。 |
| [存储配额](#storage-quota) | 存储池将存放旧版Workfront项目和Adobe云存储项目，每个许可用户为60 GB，且无硬限制。 | 系统管理员可以在“设置”的“客户信息”页面上查看存储使用情况。 |
| [年度视频审核上限](#annual-video-review-cap) | 视频验证请求的组织级别上限为付费Workfront用户许可证（标准和轻量级）的10%。 | 一旦达到上限，您就无法在下一年度之前创建新的视频审核。 您会分别按80%和100%收到应用程序内通知。 上限不适用于Frame.io Enterprise客户。 |
| [Workfront Fusion](#workfront-fusion-on-adobe-cloud-storage-projects) | 现有的基于验证的Fusion场景不会自动针对Adobe云存储项目运行。 | 范围设为旧版项目的方案将继续有效。 每个受影响的方案都采用以下三个路径之一：编辑、重建或弃用。 |

## 新建文档区域

新的文档区域是为Adobe云存储设计的统一文档体验。 它简化了导航，整合了审阅和批准活动，并且是Frame.io查看器的入口点。

全局文档区域不是新Experience的一部分。 在Adobe云存储项目中，您可以访问来自项目、项目组合、项目、任务或问题的文档。

有关详细信息，请参阅[文档区域](/help/quicksilver/documents/managing-documents/documents-area.md)。

## 文档权限

文档权限在Adobe云存储项目上存在根本性差异：

* 您无法共享或设置单个文档的权限。 相反，权限将应用于包含文档的系统生成的文档文件夹。
* 系统生成的文档文件夹继承其父项目、任务或问题的权限。
* 子文件夹从系统生成的父文档文件夹继承权限。
* 子任务不从父任务继承权限。 您必须直接添加到子任务才能访问其系统生成的文档文件夹。

有关文档权限如何工作的更多信息，请参阅[Adobe云存储模型的对象权限和访问级别概述](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work)。

## 对象权限映射

权限是在Workfront中设置的，并且会沿一个方向流向Frame.io。 您不能邀请用户加入Frame.io中的Adobe云存储项目，也不能在Frame.io中修改用户权限。

>[!TIP]
>
>培训项目协调人，使他们了解Frame.io访问权限是Workfront权限的下游反映。 如果利益相关者报告他们无法访问Adobe云存储项目的审核，则修复位于Workfront中，而不是Frame.io中。

下表将Workfront对象权限映射到Frame.io权限：

| Workfront权限 | Frame.io权限 |
|---|---|
| 管理 | 编辑和共享 |
| 贡献 | 编辑和共享 |
| 视图 | 仅注释 |

在Frame.io中，管理映射和贡献映射均可编辑和共享。 在查看Adobe云存储项目的共享模式时，请考虑参与者与经理具有相同的审核端功能（包括外部共享）是否适合您的治理模式。

有关详细信息，请参阅[Adobe云存储模型的对象权限和访问级别概述](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#permission-mapping-to-frameio)。

## 审阅和批准查看者

在Adobe云存储对象上，Frame.io查看器是审核和批准界面，取代Workfront Proof。 所有Workfront用户均可免费使用Frame.io查看器，包括分配了审阅或审批的外部用户。

Frame.io查看器提供：

* 标记和注释工具，包括手绘绘图和标准形状，如圆形、箭头和正方形
* 带有时间戳的视频评论评论，具有帧精度
* 版本历史记录和版本比较
* 通过[Frame.io iOS应用程序](https://help.frame.io/en/collections/9679120-ios-app)移动访问以进行移动审阅和批准
* 支持40多种文件格式，包括所有常见的视频、图像、音频、PDF和Microsoft Office类型，原生播放专业视频格式，如ProRes、H.265和DNxHD，并支持高达500 GB的文件

## 对象命名规则

Adobe云存储强制实施严格的命名和结构规则，以使存储层在Adobe产品中保持一致。 这些规则适用于您在Adobe云存储项目上创建的对象。 现有的旧版项目会保留其当前名称。

以下规则适用于Adobe云存储项目：

| 规则 | 详细信息 |
|---|---|
| 唯一的项目和项目名称 | 如果项目和项目属于同一项目组合，则它们不能具有相同的名称。 |
| 唯一文档名称 | 如果文档属于同一项目，则不能具有相同的名称。 文档名称在文件夹层次结构的相同父级中必须是唯一的。 |
| 禁止使用的字符 | 程序、项目组合、项目、模板、任务、问题、文档文件夹和文档不能包含以下任何特殊字符：`\ / : * ? " \| < >` |
| 尾随字符 | 项目、项目组合、模板、任务、问题和文档文件夹不能包含以句点或空格结尾的名称。 |
| 名称长度限制 | 对象名称限制为255个字符。 |

如果名称与这些规则冲突，Workfront会自动重命名对象以解决冲突。

>[!TIP]
>
>如果从模板创建Adobe云存储项目，请查看现有模板，以便它们生成的项目名称和结构符合上述规则。

## 对象可移植性

在大多数情况下，您只能在类似存储模型之间移动、复制和转换Workfront对象。 例如，您可以将任务从一个Adobe云存储项目移动到另一个Adobe云存储项目。 在三种特定情况下，您可以将旧版Workfront存储对象转换为Adobe云存储。

<!--
During a group-scoped rollout, only members of the group that has Adobe cloud storage can convert an Adobe cloud storage object, such as a request, into a project. Users outside the group, including Workfront administrators, see the error "User is not eligible for this operation."

For more information, see [Plan your Adobe cloud storage rollout](/help/quicksilver/review-and-approve-work/plan-adobe-cloud-storage-rollout.md).
-->

有关详细信息，请参阅[将旧对象转换为Adobe云存储](/help/quicksilver/review-and-approve-work/convert-objects-to-adobe-cloud-storage.md)。

## Adobe云存储对象上不可用的功能

Adobe云存储对象中不包含以下功能：

* Workfront 校样
* Workfront文档查看器
* 收藏的文档
* 请求文档

旧版项目保留对Workfront Proof和上面列出的旧版文档功能的访问权限。 Workfront Proof今后将不会获得新投资，并将在未来版本中停用。

## 存储配额

存储针对旧版Workfront对象和Adobe云存储对象进行池化。 每个许可用户可接收60 GB的存储。 存储使用率没有硬性限制，但是当使用率达到配额的75% 、 90%和100%时， Workfront管理员会收到电子邮件通知。

要查看当前存储使用量和配额，请转到&#x200B;**设置** > **系统** > **客户信息**。

有关详细信息，请参阅[检查文档存储限制](/help/quicksilver/documents/managing-documents/check-document-storage.md)。

## 年度视频审查上限

视频验证请求的年度上限设置为贵组织总付费Workfront用户许可证（标准和轻量级）的10%。 此上限在组织级别应用。

* 当使用率达到上限的80%和100%时，Workfront管理员会收到应用程序内通知。
* 一旦达到上限，就必须在下一年度期间才能创建新的视频审查请求。
* 此限制不适用于Frame.io Enterprise客户。 如果贵组织定期审查大量视频内容，请联系您的Adobe客户代表，了解有关Frame.io Enterprise许可的信息。

有关详细信息，请参阅[统一审阅和批准概述](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)中的审阅和批准资源和视频常见问题解答。

## Adobe云存储项目上的Workfront Fusion

基于旧版校对构建的现有Workfront Fusion场景不会自动针对Adobe云存储项目运行。 验证特定的模块、Webhook和API端点在某些情况下具有直接等效功能，而在其他情况下具有显着变化。 覆盖到旧版项目的方案将继续像现在一样工作。

有关对常见方案类型的影响以及如何根据方案的功能将每个方案分类为“编辑”、“重新生成”或“停用”的详细信息，请参阅[更新Workfront Fusion方案以进行统一审阅和批准](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)。
