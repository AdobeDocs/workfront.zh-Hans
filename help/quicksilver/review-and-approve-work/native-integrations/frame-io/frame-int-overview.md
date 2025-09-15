---
product-area: documents
navigation-topic: approvals
title: Frame.io集成概述
description: Frame.io集成概述
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 701f3fc2c885363b5f61fb9d77049c7d4c41963d
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---


# Frame.io集成概述

Workfront和Frame.io集成允许项目协调员在Workfront中管理项目和计划工作，而创意人员、营销人员和利益相关者可以在Frame.io中查看和批准资源。

## 构建于Adobe企业存储管理之上

此集成的核心是Adobe企业存储管理(ESM)，它是一种基于云的存储解决方案，可作为Adobe企业产品(包括Workfront和Frame.io)中资产的中央存储库。

Adobe企业存储管理的主要优势包括：

* 用于创意和工作管理资产的统一存储层
* 通过Adobe IMS集中管理权限以实现安全访问控制
* 跨Workfront、Frame.io和Creative Cloud应用程序的端到端资源可见性<!--coming soon?-->
* 满足企业需求的可扩展存储和配额管理

有关详细信息，请参阅[Adobe企业存储管理概述](help/quicksilver/review-and-approve-work/esm-overview.md)。

## 统一审查和批准

Workfront和Frame.io集成使用Workfront的统一审批功能来管理审阅和审批。 通过统一批准，您可以：

* 直接从Workfront创建和管理审阅和批准
* 实时跟踪审阅和批准状态
* 将反馈和批准集中到一个地方
* 确保所有利益相关者均有权访问最新版本的资产
* 利用AI评审员自动进行品牌合规性审查
* 等等

有关详细信息，请参阅[统一文档审批：文章索引](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md)。


### 使用Frame.io查看器

该集成还会连接到Frame.io查看器。 Frame.io查看器提供

* 标记和注释工具
* 版本历史记录和比较
* 带有时间戳的视频评论评论
* 移动访问以进行移动审阅和批准

有关详细信息，请参阅[Frame.io集成入门](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md)。

#### 视频审阅限制

<!--need to confirm these-->

#### Frame.io查看器支持的文件类型

Frame.io查看器支持所有常见视频、图像、音频、PDF和MS® Office类型。 有关支持的文件的详细列表，请参阅Frame.io[上的](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io)类型。

#### Frame.io查看器的访问和许可

Frame.io查看器适用于拥有付费许可证的所有Workfront用户。 使用Frame.io查看器审阅和批准此集成不需要其他Frame.io许可证。

如果您的组织希望利用其他Frame.io功能（如将资产直接上传到Frame.io中的项目），则可以购买Frame.io企业许可证。<!--link to Frame.io enterprise license info or who to contacT?-->

Workfront校对功能在此集成中不可用。

## Workfront中强大的项目管理

通过Workfront与Frame.io集成，项目协调员可以利用Workfront强大的项目管理功能来规划、跟踪和管理工作。

有关在Workfront中管理项目的详细信息，请参阅[项目：文章索引](/help/quicksilver/manage-work/projects/projects-toc.md)。

### 强制的结构和命名约定

由于此集成是使用ESM构建的，因此在管理项目和文档时，应注意一些强制性的结构和命名约定。

* 对象名称必须是唯一的，并且不能重复
* ESM要求层次结构树中具有相同父级的对等对象具有唯一的名称
* 如果文档属于同一项目，则不能具有相同的名称

考虑到这些限制，Workfront会根据需要自动重命名对象或文档，以防止冲突。

### Workfront中的文档管理

文档通过此集成在项目级别进行管理，目前无法上传到任务或问题。

文档访问也可在项目级别进行管理。 如果用户有权访问项目，则可以访问与该项目关联的所有文档。

<!--Documents can't be dragged as full folders.-->

### 文档体验限制

由于此集成是使用ESM构建的，因此Workfront中的原始文档体验存在一些限制：

#### 限制

以下功能将不会包含在此集成中：

* 外部文档提供程序
* 访问验证
* Workfront中的文档查看器


#### 临时限制

目前，以下功能不可用：

* 收藏的文档
* 请求文档
* 将文档发送到Adobe Experience Manager Assets
* 多阶段审批
* 在Workfront中将文档上传为评论或更新
* 将文档上传到Workfront中的任务或问题



