---
product-area: documents
navigation-topic: approvals
title: Adobe cloud storage概述
description: Adobe cloud storage概述
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YOO4BspMzbMr8iPoXRBKK65IbU5yfpiJndNuYvYF5SM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: c2fe0c6afbc9b536186bd473e95b3f82f144b06c
workflow-type: tm+mt
source-wordcount: 1061
ht-degree: 0%

---

# Adobe cloud storage概述

Adobe云存储是一个基于云的存储解决方案，它充当Adobe企业产品中资产的中央存储库。 Workfront和Frame.io集成构建在Adobe云存储之上，实现了这些平台之间的无缝协作和资源管理。

此存储选项还为资产管理与其他Adobe产品（如Adobe Creative Cloud）的未来集成铺平了道路。

## 主要功能

* **统一存储层**： Adobe云存储用作Workfront、Frame.io、Document Cloud和Creative Cloud的共享存储后端。 这实现了跨这些平台的无缝协作和资产管理。

* **内容supply chain支持**： Adobe云存储是Adobe的Content Supply chain愿景的基础组件，允许团队管理正在进行中的资源，而无需在各种Adobe应用程序中手动下载或重新上传。

* **集中式权限和访问**： Adobe Cloud Storage支持企业级访问控制，并与Adobe IMS (Identity Management System)集成以获得安全且可扩展的用户权限。

* **端到端资源可见性**：存储在Adobe云存储中的Assets可以直接在Workfront、Frame.io和Creative Cloud应用程序中显示和管理，从而提供一致的元数据、版本控制和审核跟踪。

* **与审阅和批准工作流程集成**： Adobe Cloud Storage支持创意审阅和批准工作流程，充当所有资源的事实来源，确保集中跟踪反馈和批准。

* **可扩展存储和配额管理**： Adobe云存储提供了可扩展的存储选项和跨Adobe产品的统一配额跟踪。

## 与审阅和批准工作流集成

Workfront和Frame.io集成利用Adobe云存储提供统一的审查和批准体验。 此集成允许项目协调员在Workfront中管理项目和计划工作，而创意人员、营销人员和利益相关者可以在Frame.io中查看和批准资源。 这可确保所有利益相关者均有权访问最新版本的资产，并将反馈集中到一处。

有关Workfront与Frame.io集成的详细信息，请参阅[统一审阅和批准概述](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)。

## Adobe云存储与旧版Workfront存储之间的区别

现有Workfront环境具有Adobe云存储和旧版Workfront存储的组合。 在发布Adobe Cloud Storage之前创建的任何对象都使用旧版Workfront Storage。

在环境中启用Adobe云存储后，您可以创建Adobe云存储和旧版Workfront存储项目。

>[!NOTE]
>
>默认情况下，新环境将启用Adobe云存储，并且无法选择使用旧版Workfront存储。


### 文档

#### 新建文档区域

新的文档区域是为Adobe云存储重新设计的统一文档区域。

此更新的界面简化了导航，提高了清晰度，并使团队更轻松地在一个统一的环境中管理审阅和批准。 有关详细信息，请参阅[文档区域概述](/help/quicksilver/documents/managing-documents/documents-area.md)。

#### 新建文档权限模型

>[!IMPORTANT]
>
>在Adobe云存储中，文档权限的工作方式与旧版Workfront存储中的不同。 文档从链接的项目、任务或问题继承权限。

无法单独共享文档。 相反，系统为每个任务或问题自动生成文件夹，并继承任务或问题的权限。 上传到任务或问题的任何文档都存储在该生成的文件夹中。

有关新文档权限模型的详细信息，请参阅[Adobe云存储模型的对象权限和访问级别概述](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)。

##### 文件夹中的链接对象

在项目级别，系统生成的文件夹显示链接对象。 自动将该文件夹的名称与其所属的任务或问题相同。 链接文件夹是系统知道该文件夹应显示在哪个任务或问题上的方式。

有关详细信息，请参阅[文档权限的工作方式](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work)。

#### Adobe云通道

Adobe Cloud Drive是一款桌面应用程序，可将您的Adobe云存储项目作为驱动器装载到Mac或Windows计算机上。 您可以在Adobe Cloud Drive中打开、编辑和保存任何应用程序中的文件，同时让您的工作与Adobe Cloud Storage保持同步。 有关详细信息，请参阅[Adobe Cloud Drive概述](/help/quicksilver/documents/adobe-cloud-drive/adobe-cloud-drive-overview.md)。

## Workfront对象

下表比较了Adobe云存储和Workfront对象的旧版Workfront存储的功能。

Workfront对象包括项目组合、项目群、项目、模板、任务和问题。

| Adobe 云存储 | 旧版 Workfront 存储 |
|---|---|
| <ul><li>使用Adobe云存储</li><li>与Frame.io集成</li><li>使用新的文档体验</li><li>实施严格的命名约定</li><li>直接文档共享不可用</li><li>文档在其他Adobe产品（如Frame.io和Creative Cloud）中可用</li></ul> | <ul><li>使用Workfront存储</li><li>使用校对查看器</li><li>支持单个文档共享</li></ul> |

### 移动、复制和转换对象

在大多数情况下，您可以在类似存储模型之间移动、复制和转换Workfront对象。 例如，您可以将任务从一个Adobe云存储项目移动到另一个Adobe云存储项目。

在以下三个特定用例中，您可以将旧版Workfront存储对象转换为Adobe云存储：

* 将旧版Workfront存储任务转换为Adobe云存储项目。
* 将旧版Workfront存储产品组合转换为Adobe云存储产品组合。
* 从旧版Adobe存储模板创建一个Workfront云存储项目。

在任何这些转换期间，文档和文档文件夹都不会从旧版Workfront存储移动到Adobe云存储。

有关详细信息，请参阅[在Adobe云存储上移动到Workfront](/help/quicksilver/review-and-approve-work/workfront-storage.md)中的[对象可移植性](/help/quicksilver/review-and-approve-work/workfront-storage.md#object-portability)。

## 启用Adobe云存储

您必须使用支持Adobe云存储的Workfront版本。 如果贵组织尚未使用支持的版本，请联系您的Adobe客户代表。

有关在环境中启用Adobe云存储的信息，请参阅[为您的组织启用Adobe云存储](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)。

>[!NOTE]
>
>新客户默认启用了Adobe云存储，并且无法选择使用旧版Workfront存储。



## 沙盒环境中的Adobe云存储

Adobe云存储在[!DNL Workfront]沙盒环境中可用，因此您可以在生产环境中启用它之前对其进行测试。 但是，Frame.io查看器在沙盒中不可用，因此必须在生产环境中验证完整的统一审阅和批准体验。

如果您有自定义刷新沙盒，则必须在升级到支持Adobe云存储的Workfront版本后刷新它，才能在沙盒中访问Adobe云存储功能。 有关详细信息，请参阅[自定义刷新沙盒环境 [!DNL Adobe Workfront] &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)。

## 注意事项

* Workfront可能会与Frame.io或Creative Cloud不同步，例如某个资产在Workfront中被删除但仍出现在Frame.io中，请与Workfront支持人员联系以重新同步环境。


