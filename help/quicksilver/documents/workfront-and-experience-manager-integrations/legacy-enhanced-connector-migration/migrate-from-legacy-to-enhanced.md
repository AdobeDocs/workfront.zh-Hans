---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 从旧连接器迁移到增强连接器
description: 以下流程概述了将Adobe Experience Manager旧版连接器迁移到增强型连接器以将Adobe Workfront与AEM Assets集成的最佳实践。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# 从旧连接器迁移到增强连接器

以下流程概述了将Adobe Experience Manager旧版连接器迁移到增强型连接器以将Adobe Workfront与AEM Assets集成的最佳实践。

>[!IMPORTANT]
>
>本文档仅适用于使用Adobe Experience Manager Assets内部部署或Managed Services环境的客户。


对于使用Adobe Experience Manager Assetsas a Cloud Service的客户，从旧版连接器迁移到的路径将为Workfront内部新的本机集成。 要了解有关此迁移过程的更多信息，请参阅[从旧版或增强型连接器迁移到Workfront以进行Adobe Experience Manager as a Cloud Service集成](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md)。

## 实施增强型连接器

>[!IMPORTANT]
>
>实施增强型连接器需要认证合作伙伴或Adobe Consulting服务。
>
> 对于希望对增强型连接器进行认证的合作伙伴，请查看以下文章： [用于Experience Manager增强型连接器的Workfront Expert Series](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview.html?lang=en)。

要实施增强型连接器，请参阅[为Experience Manager增强型连接器配置Workfront](https://experienceleague.adobe.com/docs/experience-manager-65/assets/integrations/workfront-connector-configure.html?lang=en)。


## 移动现有资源

配置环境后，您可以将现有的链接资源和文件夹移动到Adobe Experience Manager。 这是一个可选步骤，但将确保在卸载旧连接器后，之前通过旧连接器链接的文件夹和资产仍可访问。

有关移动资产的详细信息，请参阅[迁移链接的文件夹和文档](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md)。

## 验证所有要使用的关键用例

在卸载旧版连接器之前，必须验证所有打算通过增强型连接器使用的关键用例。

## 卸载旧版连接器

最后，您需要卸载旧版连接器。 旧式连接器不打算与增强型连接器并行运行。

要卸载，请参阅[使用Adobe Experience Manager旧版连接器卸载Workfront](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md)。
