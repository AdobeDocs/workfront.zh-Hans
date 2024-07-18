---
title: 2024年第一季度集成增强功能
description: 2024年第一季度集成增强功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0d581f3c-2aaf-4ac1-97a5-df1b01627080
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# 2024年第一季度集成增强功能

本页介绍了2024年第一季度版本与预览环境集成的所有增强功能。 这些增强功能将在2024年第一季度发行版的“生产”环境中提供。

有关2024年第一季度发布周期中此时可用的所有更改列表，请参阅[ 2024年第一季度发布概述](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md)。

## Experience Manager Assets Essentials中的映射元数据现在使用`xcm:keywords`而不是`dc:subject`

我们更新了Experience Manager Assets Essentials集成，以匹配Experience Manager Assetsas a Cloud Service集成中的体验。 现在，当在Experience Manager Assets中将多个单行文本字段映射到单个字段时，两个服务都使用`xcm:keywords`字段。

以前，这些字段将映射到Experience Manager Assets Essentials中的`dc:subject`字段。 Experience Manager Assetsas a Cloud Service功能未做更改。

当前映射到`dc:subject`的任何Experience Manager Assets Essentials元数据都必须重新映射到`xcm:keywords`。

有关将元数据映射到Experience Manager Assets Essentials的信息，请参阅[AEM关键字](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md#aem-keyword)。

## Adobe Experience Manager集成中现在提供预输入字段

为了更便于在Workfront和Adobe Experience Manager之间链接字段，我们在元数据映射中添加了对预输入字段的支持。 现在，您可以将预输入字段映射到Adobe Experience Manager中的相应字段。

如果用户为Workfront中的字段选择其他值，则此更改会立即反映在Adobe Experience Manager中。 此外，如果字段值选项发生更改（例如团队将其名称更改为新名称），则此更改也会反映在Adobe Experience Manager中。

有关Adobe Experience Manager集成中元数据映射的信息和说明，请参阅[设置元数据](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-metadata-optional)。

## 在Adobe Experience Manager中自动发布资源

我们已将另一个工作流添加到Adobe Experience Manager集成。 现在，您可以将资源设置为在发送到Adobe Experience Manager时自动发布。 可将集成配置为发布到Adobe Experience Manager发布服务或Adobe Experience Manager Brand Portal。

可在Adobe Experience Manager集成中启用和配置自动Publish工作流。 启用后，可以在项目模板或项目级别编辑工作流。

有关详细信息，请参阅[在Experience Manager Assets集成中使用工作流](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md)中的[发布资产](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#publishing-assets)。
