---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 从旧版或增强型连接器迁移到Workfront for Adobe Experience Manager as a Cloud Service集成
description: 本页面上的信息介绍了从Workfront for Experience Cloud enhanced或旧版连接器移动到连接Workfront和Adobe Experience Manager Assets的最新本机集成的最佳as a Cloud Service。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# 从旧版或增强型连接器迁移到Workfront for Adobe Experience Manager as a Cloud Service集成

本页面上的信息介绍了从Workfront for Experience Cloud enhanced或旧版连接器移动到连接Workfront和Adobe Experience Manager Assets的最新本机集成的最佳as a Cloud Service。

>[!IMPORTANT]
>
>此信息不适用于使用Adobe Experience Manager Assets本地或Managed Services环境的客户。

## 将Workfront实例移到Admin Console

如果客户打算使用Workfront与Adobe Experience Manager Assets之间的新本机集成，则必须确保其Workfront环境已绑定到Adobe Admin Console。 对于现有的Workfront环境，这可能需要将环境迁移到连接的Adobe Admin Console。 有关此迁移及相关检查列表的更多详细信息，请参阅 [准备将您的组织载入Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

Adobe必须帮助执行此迁移。 要请求帮助，请执行以下操作之一：

* 如果您有Workfront中心访问权限，请将请求提交到 [Workfront迁移到Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&amp;projectID=629674d500054a38133cf26e01d06a97&amp;path=).
* 如果您没有Workfront中心访问权限，则可以将请求提交到 [Workfront到Adobe Admin Console的抢先迁移请求队列](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

## 为Adobe Experience Manager资产配置新的Workfrontas a Cloud Service集成

将Workfront环境迁移到Adobe Admin Console后，Workfront管理员可以配置新的本机集成。 有关配置帮助，请参阅 [配置Experience Manager Assetsas a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## 将现有资产移动到Workfront以实现Adobe Experience Manager资产as a Cloud Service集成

配置环境后，您可以将现有关联的资产和文件夹移到Adobe Experience Manager。 这是一个可选步骤，但将确保卸载这些连接器后，仍可以通过旧版或增强型连接器访问之前链接的文件夹和资产。

有关移动资产的更多信息，请参阅 [迁移链接的文件夹和文档](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## 验证所有要使用的关键用例

在卸载旧版或增强型连接器之前，务必要验证打算通过本机集成使用的所有关键用例。

## 卸载旧版或增强型连接器

最后，您需要卸载旧版或增强型连接器。 本机集成不打算与任一连接器并行运行。

要卸载，请参阅

* 旧版连接器卸载说明： [使用Adobe Experience Manager旧版连接器卸载Workfront](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* 增强的连接器卸载说明： [使用Adobe Experience Manager增强连接器卸载Workfront](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
