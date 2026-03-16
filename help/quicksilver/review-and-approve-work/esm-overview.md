---
product-area: documents
navigation-topic: approvals
title: Adobe企业存储概述
description: Adobe企业存储概述
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
source-git-commit: 7f17ffc179914747d29c4acb08b34341c5a4b7b4
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 0%

---

# Adobe企业存储概述

Adobe企业存储是一种基于云的存储解决方案，它用作Adobe企业产品中资产的中央存储库。 Workfront和Frame.io集成构建在Adobe企业存储之上，实现了这些平台之间的无缝协作和资产管理。

此存储选项还为资产管理与其他Adobe产品（如Adobe Creative Cloud）的未来集成铺平了道路。

## 主要功能

* **统一存储层**： Adobe企业存储用作Workfront、Frame.io、Document Cloud和Creative Cloud的共享存储后端。 这实现了跨这些平台的无缝协作和资产管理。

* **内容supply chain支持**： Adobe企业存储是Adobe的Content Supply chain愿景的基础组件，它允许团队管理正在进行中的资源，而无需在各种Adobe应用程序中手动下载或重新上传。

* **集中式权限和访问**： Adobe企业存储支持企业级访问控制，并与Adobe IMS (Identity Management System)集成以获得安全且可扩展的用户权限。

* **端到端资源可见性**：存储在Adobe企业存储中的Assets可以直接在Workfront、Frame.io和Creative Cloud应用程序中显示和管理，从而提供一致的元数据、版本控制和审核跟踪。

* **与审阅和批准工作流程集成**： Adobe企业存储通过将所有资源的事实来源用作审阅和批准工作流程，来确保集中跟踪反馈和批准，从而支持创意审阅和批准工作流程。

* **可扩展的存储和配额管理**： Adobe企业级存储提供了可扩展的存储选项和跨Adobe产品的统一配额跟踪。

## 与审阅和批准工作流集成

Workfront和Frame.io集成利用Adobe企业存储以提供统一的审查和批准体验。 此集成允许项目协调员在Workfront中管理项目和计划工作，而创意人员、营销人员和利益相关者可以在Frame.io中查看和批准资源。 这可确保所有利益相关者均有权访问最新版本的资产，并将反馈集中到一处。

有关Workfront与Frame.io集成的详细信息，请参阅[Frame.io集成概述](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md)。

## Adobe企业存储与旧版Workfront存储之间的区别

现有Workfront环境具有Adobe企业级存储和旧版Workfront存储的组合。 在Adobe企业级存储发布之前创建的任何对象都使用旧版Workfront存储。

在环境中启用Adobe企业级存储后，您可以创建Adobe企业级存储和旧版Workfront存储项目。

>[!NOTE]
>
>默认情况下，新环境将启用Adobe企业级存储，并且无法选择使用旧版Workfront存储。


### 文档

#### 新建文档区域

新文档区域是为Adobe企业存储重新设计的统一文档区域。

此更新的界面简化了导航，提高了清晰度，并使团队更轻松地在一个统一的环境中管理审阅和批准。 有关详细信息，请参阅[文档区域概述](/help/quicksilver/documents/managing-documents/documents-area.md)。

#### 新建文档权限模型

>[!IMPORTANT]
>
>在Adobe企业存储中，文档权限的工作方式与旧版Workfront存储中的不同。 文档从链接的项目、任务或问题继承权限。

无法单独共享文档。 相反，系统为每个任务或问题自动生成文件夹，并继承任务或问题的权限。 上传到任务或问题的任何文档都存储在该生成的文件夹中。

有关新文档权限模型的详细信息，请参阅[Adobe企业存储模型的对象权限和访问级别概述](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)。

##### 文件夹中的链接对象

在项目级别，系统生成的文件夹显示链接对象。 自动将该文件夹的名称与其所属的任务或问题相同。 链接文件夹是系统知道该文件夹应显示在哪个任务或问题上的方式。

有关详细信息，请参阅[文档权限的工作方式](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work)。

## Workfront对象

下表比较了Adobe企业级存储和Workfront对象的旧版Workfront存储的功能。

Workfront对象包括项目组合、项目群、项目、模板、任务和问题。

| Adobe企业存储 | 旧版Workfront存储 |
|---|---|
| <ul><li>使用Adobe企业存储</li><li>与Frame.io集成</li><li>使用新的文档体验</li><li>实施严格的命名约定</li><li>直接文档共享不可用</li><li>文档在其他Adobe产品（如Frame.io和Creative Cloud）中可用</li></ul> | <ul><li>使用Workfront存储</li><li>使用校对查看器</li><li>支持单个文档共享</li></ul> |

### 移动、复制和转换对象

您可以在类似存储模型之间移动、复制和转换Workfront对象。 例如，您可以将任务从Adobe企业存储项目移动到另一个Adobe企业存储项目。 您无法将任务从Adobe企业存储项目移动到旧版Workfront存储项目。

这些操作可从任务或问题的更多菜单中获取。 每个操作都尊重文档完整性、权限继承和Adobe企业存储规则。

## 启用Adobe企业存储

现有客户可以在合同续订后在其环境中启用Adobe企业存储。 有关启用Adobe企业存储的详细信息，请参阅[为您的组织启用Adobe企业存储](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)。

>[!NOTE]
>
>新客户默认启用了Adobe企业级存储，并且不能选择使用旧版Workfront存储。



## 注意事项

* Workfront可能会与Frame.io或Creative Cloud不同步，例如某个资源在Workfornt中被删除，但仍出现在Frame.io中，请与Workfront支持人员联系重新同步环境。


