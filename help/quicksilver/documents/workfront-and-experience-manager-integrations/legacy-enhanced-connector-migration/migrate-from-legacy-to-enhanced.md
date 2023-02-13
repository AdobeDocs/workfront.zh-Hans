---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 从旧版连接器迁移到增强型连接器
description: 以下流程概述了将Adobe Experience Manager旧版连接器移至用于将Adobe Workfront与AEM Assets集成的增强型连接器的最佳实践。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 从旧版连接器迁移到增强型连接器

以下流程概述了将Adobe Experience Manager旧版连接器移至用于将Adobe Workfront与AEM Assets集成的增强型连接器的最佳实践。

>[!IMPORTANT]
>
>本文档仅适用于使用Adobe Experience Manager Assets本地或Managed Services环境的客户。


对于Adobe Experience Manager Assetsas a Cloud Service的客户，从旧版连接器迁移到Workfront内的新本机集成的路径。 要详细了解此迁移过程，请参阅 [从旧版或增强型连接器迁移到Workfront for Adobe Experience Manager as a Cloud Service集成](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md).

## 实施增强的连接器

>[!IMPORTANT]
>
>实施增强型连接器需要经认证的合作伙伴或Adobe咨询服务。
>
> 对于希望验证增强型连接器的合作伙伴，请查看以下文章： [Workfront for Experience Manager增强型连接器专家系列](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview.html?lang=en).

要实施增强的连接器，请参阅 [为Experience Manager增强的连接器配置Workfront](https://experienceleague.adobe.com/docs/experience-manager-65/assets/integrations/workfront-connector-configure.html?lang=en).


## 移动现有资产

配置环境后，您可以将现有关联的资产和文件夹移到Adobe Experience Manager。 这是一个可选步骤，但将确保卸载旧版连接器后，仍可以通过旧版连接器访问之前链接的文件夹和资产。

有关移动资产的更多信息，请参阅 [迁移链接的文件夹和文档](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## 验证所有要使用的关键用例

在卸载旧版连接器之前，务必验证打算通过增强型连接器使用的所有关键用例。

## 卸载旧版连接器

最后，您需要卸载旧版连接器。 旧版连接器不能与增强型连接器并行运行。

要卸载，请参阅 [使用Adobe Experience Manager旧版连接器卸载Workfront](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
