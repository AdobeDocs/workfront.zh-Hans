---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 从旧版或增强型连接器迁移到Workfront以进行Adobe Experience Manager as a Cloud Service集成
description: 此页面上的信息介绍了从Workfront for Experience Cloud增强型连接器或旧版连接器迁移到连接Workfront和Adobe Experience Manager Assets as a Cloud Service的最新本机集成的最佳实践。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
TQID: 'https://experienceleague.adobe.com/0pAHfS7cDqv1tV4TBdx9WqvJA1-zySGsPHVXI8EG7Hc'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: e7123179a59cd7ed9c76f4718b3b8019854cbfe1
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%
---
# 从旧版或增强型连接器迁移到Workfront以进行Adobe Experience Manager as a Cloud Service集成

此页面上的信息介绍了从Workfront for Experience Cloud增强型连接器或旧版连接器迁移到连接Workfront和Adobe Experience Manager Assets as a Cloud Service的最新本机集成的最佳实践。

>[!IMPORTANT]
>
>此信息不适用于使用Adobe Experience Manager Assets内部部署或Managed Services环境的客户。

<!--

## Move your Workfront instance to the Admin Console

Customers that intend to use the new native integration between Workfront and Adobe Experience Manager Assets as a Cloud Service must ensure their Workfront environment is tied to an Adobe Admin Console. For existing Workfront environments, this will likely require a migration of the environment to a connected Adobe Admin Console. For more details regarding this migration and the associated checklist, see [Prepare to onboard your organization to the Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md). 

 Adobe must help carry out this migration. To request help, do one of the following:

* If you have Workfront Hub access, submit your request to the [Workfront Migration to Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=629674d500054a38133cf26e01d06a97&path=).
* If you do not have Workfront Hub access, you can submit your request to the [Workfront to Adobe Admin Console Early Migration Request Queue](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

-->

## 为Adobe Experience Manager assets as a Cloud Service集成配置新的Workfront

将Workfront环境迁移到Adobe Admin Console后，Workfront管理员可以配置新的本机集成。 有关配置帮助，请参阅[配置Experience Manager Assets as a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)。

## 将现有资源移至Workfront以进行Adobe Experience Manager资源as a Cloud Service集成

配置环境后，您可以将现有的链接资源和文件夹移动到Adobe Experience Manager。 这是一个可选步骤，但将确保卸载以前通过旧版或增强型连接器链接的文件夹和资产后，这些连接器仍可访问。

有关移动资产的详细信息，请参阅[迁移链接的文件夹和文档](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md)。

## 验证所有要使用的关键用例

在卸载旧版或增强型连接器之前，请务必验证拟通过本机集成使用的所有关键用例。

## 卸载旧版或增强型连接器

最后，您需要卸载旧版或增强型连接器。 本机集成不打算与任一连接器并行运行。

要卸载，请参阅

* 旧版连接器卸载说明： [使用Adobe Experience Manager旧版连接器卸载Workfront](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md)。
* 增强型连接器卸载说明： [使用Adobe Experience Manager增强型连接器卸载Workfront](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md)。
