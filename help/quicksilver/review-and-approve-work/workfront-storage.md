---
product-area: documents
navigation-topic: approvals
title: 在Adobe企业存储上迁移到Workfront
description: 规划在Adobe企业存储上推出Workfront的计划。 了解Adobe企业存储对象有何变化，包括新的“文档”区域和Frame.io查看体验，并决定在您的环境中如何推出Adobe企业存储。
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 722ba7f6617e3ccc1a1dcbf51f5d539c550617ab
workflow-type: tm+mt
source-wordcount: '2360'
ht-degree: 0%

---

# 在Adobe企业存储上迁移到Workfront

Adobe企业存储上的Workfront支持完整的统一审核和批准体验：在Frame.io查看器中审核、强大的批准工作流、资产的跨产品可见性等等。

您现有的对象将继续以它们现在的方式工作。 新的“文档”区域、Frame.io查看器和其他Adobe企业存储行为仅适用于使用Adobe企业存储的对象。

本文面向准备在Workfront企业存储上推出Workfront的Adobe管理员。 它涵盖了Adobe企业存储对象上的主要差异，如何选择转出类型，以及在为用户启用Adobe企业存储之前需要考虑的事项。

>[!IMPORTANT]
>
>您的Workfront合同必须包含一个V2 Workfront SKU才能使用Frame.io查看器和Adobe企业存储。 有关详细信息，请参阅[统一审阅和批准概述](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md#getting-started-with-unified-review-and-approval)中的常见问题解答。



## 了解旧版Workfront存储和Adobe企业存储

更新合同以包括新的统一审查和批准体验后，您的环境可以包含两种类型的对象：旧版Workfront存储上的对象（您当前拥有的对象）和使用Adobe企业存储创建的对象。 从较高层面看，这两种存储模式在数据所在的位置、哪些Adobe产品可以看到数据以及有哪些功能可用方面有所不同：

|  | 旧版Workfront存储中的对象 | Adobe企业存储上的对象 |
|---|---|---|
| 存储后端 | 仅限Workfront | Adobe企业存储 |
| 跨产品可见性 | 仅限Workfront | Workfront、Frame.io和Creative Cloud |
| 功能 | 旧版功能 | 新功能 |

在设置区域中启用Adobe企业级存储之前创建的对象将保留在旧版Workfront存储中。 本文中介绍的新行为仅适用于您和您的用户在启用Adobe企业级存储后创建的Adobe企业级存储对象。

## Adobe企业存储有何不同

Adobe企业存储最大的日常更改是新的“文档”区域和Frame.io查看器，支持其中的审阅和批准。 还有其他不同会影响您管理对象、文档和审阅的方式。

下表总结了切换到Adobe企业存储时的主要差异。 表中的每个区域都链接到下面的详细部分。

| 区域 | 不同之处 | 须知事项 |
|---|---|---|
| [新文档区域](#the-new-documents-area) | 重新设计、统一的“文档”区域取代了旧的“文档”区域。 | 无全局文档区域。 从项目群、项目组合、项目、任务或问题访问文档。 |
| [文档权限](#document-permissions) | 文档从链接的项目、任务或问题继承权限。 | 您无法共享或设置单个文档的权限。 您可以通过Workfront中的对象共享模式来管理所有访问权限，该模式会级联到系统生成的文档文件夹。 |
| [对象权限映射](#object-permissions-mapping) | Workfront的“管理”和“贡献”权限映射到Frame.io中的“编辑”和“共享”。 查看映射到“仅注释”。 | 权限在Workfront中进行管理。 Manage和Contribute用户都可以在Frame.io中获得外部共享功能。 |
| [审阅和批准查看者](#review-and-approval-viewer) | Frame.io查看器将取代Workfront校对查看器。 | 包含所有拥有付费许可证的Workfront用户。 支持标记、带有时间戳的注释、版本历史记录、移动设备、40多种格式、高达500 GB的文件。 |
| [对象命名规则](#object-naming-rules) | 适用严格的命名规则：项目组合或项目中的唯一名称，无特殊字符，无尾随句点或空格，255个字符限制。 | 当出现冲突时，Workfront会自动重命名对象。 生成新项目名称和结构的审核模板。 |
| [对象可移植性](#object-portability) | 您只能在类似存储模型之间移动、复制和转换对象。 | Adobe企业存储对象无法移动到旧版项目，反之亦然。 将Adobe企业存储项目移动到旧版项目组合或项目群会将父级存储转换为Adobe企业存储。 |
| [功能不可用](#capabilities-not-available-on-adobe-enterprise-storage-objects) | Workfront Proof、Workfront文档查看器、收藏夹文档和请求文档不在体验中。 | 旧版对象保留这些功能。 Workfront Proof将不会获得新投资，并将在未来版本中停用。 |
| [存储配额](#storage-quota) | 存储被池用于旧版Workfront项目和Adobe企业项目。 每个许可用户为60 GB。 没有硬帽子。 | 系统管理员可以在“设置”的“客户信息”页面上查看存储使用情况。 |
| [年度视频审核上限](#annual-video-review-cap) | 组织级别的视频验证请求上限为付费Workfront用户许可证（标准和轻量级）的10%。 | 一旦到达，直到下一年度期间才会有新的视频审查。 80%和100%的应用程序内通知。 不适用于Frame.io Enterprise客户。 |
| [Workfront Fusion](#workfront-fusion-on-adobe-enterprise-storage-projects) | 现有的基于验证的Fusion方案不会自动针对Adobe企业存储项目运行。 | 范围设为旧版项目的方案将继续有效。 每个受影响的方案都会获得以下三个路径之一：编辑、重建或弃用。 新连接器预计将于2026年第3季度推出。 |

### 新建文档区域

新的文档区域是为Adobe企业存储设计的统一文档体验。 它简化了导航，整合了审阅和批准活动，并且是Frame.io查看器的入口点。

全局文档区域不是新Experience的一部分。 在Adobe企业存储项目中，您可以从项目、项目组合、项目、任务或问题访问文档。

有关详细信息，请参阅[文档区域](/help/quicksilver/documents/managing-documents/documents-area.md)。

### 文档权限

文档权限在Adobe企业存储项目上存在根本性差异：

* 您无法共享或设置单个文档的权限。 相反，权限将应用于包含文档的系统生成的文档文件夹。
* 系统生成的文档文件夹继承其父项目、任务或问题的权限。
* 子文件夹从系统生成的父文档文件夹继承权限。
* 子任务不从父任务继承权限。 您必须直接添加到子任务才能访问其系统生成的文档文件夹。


有关文档权限如何工作的更多信息，请参阅[Adobe企业存储模型的对象权限和访问级别概述](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work)。


### 对象权限映射

权限是在Workfront中设置的，并且会沿一个方向流向Frame.io。 您不能邀请用户加入Frame.io中的Adobe企业存储项目，也不能在Frame.io中修改用户权限。

>[!TIP]
>
>培训项目协调人，使他们了解Frame.io访问权限是Workfront权限的下游反映。 如果利益相关者报告他们无法访问Adobe企业存储项目的审核，则修复位于Workfront中，而不是Frame.io。

下表将Workfront对象权限映射到Frame.io权限：

| Workfront权限 | Frame.io权限 |
|---|---|
| 管理 | 编辑和共享 |
| 贡献 | 编辑和共享 |
| 视图 | 仅注释 |

在Frame.io中管理映射和分配映射到&#x200B;**编辑和共享**。 在查看Adobe企业存储项目的共享模式时，请考虑参与者与经理具有相同的审核端功能（包括外部共享）是否适合您的治理模式。

有关详细信息，请参阅[Adobe企业存储模型的对象权限和访问级别概述](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#permission-mapping-to-frameio)。


### 审阅和批准查看者

在Adobe企业存储对象上， Frame.io查看器是审核和批准界面，取代了Workfront Proof。 所有拥有付费许可证的Workfront用户都包含Frame.io查看器。

Frame.io查看器提供：

* 标记和注释工具，包括手绘绘图和标准形状，如圆形、箭头和正方形
* 带有时间戳的视频评论评论，具有帧精度
* 版本历史记录和版本比较
* 移动访问以进行移动审阅和批准
* 支持40多种文件格式，包括所有常见的视频、图像、音频、PDF和Microsoft Office类型，原生播放专业视频格式，如ProRes、H.265和DNxHD，并支持高达500 GB的文件


### 对象命名规则

Adobe企业存储强制实施严格的命名和结构规则，以使存储层在Adobe产品中保持一致。 这些规则适用于您在Adobe企业存储项目上创建的对象。 现有的旧版项目会保留其当前名称。

以下规则适用于Adobe企业存储项目：

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
>如果从模板创建Adobe企业存储项目，请查看现有模板，以便它们生成的项目名称和结构符合上面的规则。


### 对象可移植性

您可以在类似存储模型之间移动、复制和转换Workfront对象。 例如，您可以将任务从一个Adobe企业存储项目移动到另一个Adobe企业存储项目。 您无法将任务或问题从Adobe企业存储项目移动或复制到旧版项目，反之亦然。

现在，当您创建Adobe企业存储项目或将项目移动到旧版项目组合或项目群时，该项目组合或项目群会自动转换为Adobe企业存储对象。 在未来的版本中，系统管理员可以更好地控制自动转换的对象。

### Adobe企业存储对象上不可用的功能

Adobe企业存储对象中不包含以下功能：

* Workfront 校样
* Workfront文档查看器
* 收藏的文档
* 请求文档

旧版项目保留对Workfront Proof和上面列出的旧版文档功能的访问权限。 Workfront Proof今后将不会获得新投资，并将在未来版本中停用。

### 存储配额

存储针对旧版Workfront对象和Adobe企业级存储对象进行池。 每个许可用户可接收60 GB的存储。 存储使用率没有硬性限制，但是当使用率达到配额的75% 、 90%和100%时， Workfront管理员会收到电子邮件通知。

系统管理员可以转至&#x200B;**设置** > **系统** > **客户信息**&#x200B;查看当前存储使用量和配额。

有关详细信息，请参阅[检查文档存储限制](/help/quicksilver/documents/managing-documents/check-document-storage.md)。


### 年度视频审查上限

视频验证请求的年度上限设置为贵组织总付费Workfront用户许可证（标准和轻量级）的10%。 此上限在组织级别应用。

* 当使用率达到上限的80%和100%时，Workfront管理员会收到应用程序内通知。
* 达到上限后，直到下一年度期间才能创建新的视频审查请求。
* 此限制不适用于Frame.io Enterprise客户。 如果贵组织定期审查大量视频内容，请联系您的Adobe客户代表，了解有关Frame.io Enterprise许可的信息。

有关详细信息，请参阅[统一审阅和批准概述](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)中的审阅和批准资源和视频常见问题解答。

### Workfront Fusion on Adobe企业存储项目

基于旧版验证构建的现有Workfront Fusion方案无法自动针对Adobe企业存储项目运行。 验证特定的模块、Webhook和API端点在某些情况下具有直接等效功能，而在其他情况下具有显着变化。 覆盖到旧版项目的方案将继续像现在一样工作。

带有对统一审阅和批准的原生支持的Fusion连接器预计将在2026年第3季度提供。

有关对常见方案类型的影响以及如何根据方案的功能将每个方案分类为“编辑”、“重新生成”或“停用”的详细信息，请参阅[更新Workfront Fusion方案以进行统一审阅和批准](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)。


## 选择Adobe企业级存储的部署方式

您可以决定Adobe企业级存储对用户显示的方式。 有两种配置，一种可应用于您的整个组织或特定的Workfront组。

有关分步说明，请参阅[为您的组织启用Adobe企业存储](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)。

* **仅限Adobe企业存储**：默认情况下，新项目使用Adobe企业存储。 用户无法创建旧版项目。
* **Adobe企业级存储和旧版Workfront存储**：用户创建项目时，他们会在Adobe企业级存储（标记为“新建项目”）和旧版Workfront存储（标记为“旧版存储”）之间进行选择。

  ![选择项目类型](assets/choose-project-type.png)



>[!TIP]
>
>要先将Adobe企业存储放在较小的团队之前，请将任一配置应用于单个Workfront组。 这允许您在更广泛地推广之前运行定向试点。 我们建议从组级别推出开始，以实现受控步调，然后在试点小组验证体验后，扩展到整个组织。

现有对象会保留创建它们的存储模型。 更改默认存储首选项不会更改任何现有对象。

## 规划您的转出

每个Workfront环境都不一样。 在为用户启用Adobe企业存储之前，请花些时间规划一下您的组织成功转出的情况。 下面的建议不是清单，而是您自己的计划的起点。

**1. 选择试点组。** 通过组范围的推出，您可以先将Adobe企业存储放在更小的团队面前，收集反馈，并在更广泛的推出之前进行调整。 选择一个其工作模式具有足够代表性的组，以便及早发现您想要了解的问题。

**2. 将更改传达给最终用户。** 对于审阅人、审批人和项目所有者而言，最大的可见更改是新增的“文档”区域和Frame.io查看器，它们支持Adobe企业存储项目的审阅和审批。 规划您将如何介绍这些存储产品，以便用户了解在遇到他们的第一个Adobe企业存储项目时会有什么样的期望。 [统一审查和批准入门](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)文章是面向最终用户的材料的有用起点。

**3. 规划Workfront Fusion连接器的可用性。** 带有对统一审阅和批准的原生支持的Fusion连接器预计将在2026年第3季度提供。 现有的基于验证的Fusion方案将继续用于旧版项目。 在将依赖这些方案的团队引入Adobe企业存储试点计划之前，请决定是等待新连接器、根据当前API重建，还是使用本机统一审查和批准功能替换这些方案。

有关对常见方案类型的影响以及如何根据方案的功能将每个方案分类为“编辑”、“重新生成”或“停用”的详细信息，请参阅[更新Workfront Fusion方案以进行统一审阅和批准](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)。


## 相关文章

* [Adobe企业存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)
* [为您的组织启用Adobe企业存储](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)
* [统一审查和批准概述](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [统一审查和批准入门](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [“文档”区域](/help/quicksilver/documents/managing-documents/documents-area.md)
* [Adobe企业存储模型的对象权限和访问级别概述](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)