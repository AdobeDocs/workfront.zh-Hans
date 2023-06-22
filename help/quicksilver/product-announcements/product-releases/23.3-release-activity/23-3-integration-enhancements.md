---
title: 23.3集成增强
description: 23.3集成增强
author: Lisa
feature: Product Announcements
source-git-commit: 3ebf408bb03a97de78600ab771834a7d7f29e2e0
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 0%

---

# 23.3集成增强

本页介绍了23.3版本对“预览”环境所做的所有集成增强。 这些增强功能将在23.3版本的生产环境中提供。

有关23.3版本周期此时可用所有更改的列表，请参阅 [23.3发行版概述](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

## Adobe Creative Cloud集成现在支持多个分配的用户

Adobe Creative Cloud集成现在支持在任务或问题有多个分配用户时选择“完成我的部分”和“完成”（或“已解决”）。

以前，集成允许用户将任务标记为完成，而无需指定“完成我的部分”或“完成”/“已解决”。

要利用此功能，请下载并安装最新的WorkfrontCreative Cloud插件。

有关该功能的更多信息，请参阅 [使用Adobe Workfront插件将工作项标记为完成](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-complete.md).

有关安装Workfront forCreative Cloud插件的信息，请参阅 [安装适用于Creative Cloud应用程序的Adobe Workfront插件](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## 从Workfront查看和管理Workfront通知以用于Creative Cloud插件

为了让您更轻松地接收所需的通知，我们让您能够在不离开Adobe Creative Cloud的情况下查看和管理Workfront通知。 现在，您可以直接从Creative Cloud应用程序的Workfront插件窗口中查看通知，以及访问与这些通知相关的工作项和注释。

以前，通知只能在Workfront中通过电子邮件提供。

要利用此功能，请下载并安装最新的WorkfrontCreative Cloud插件。

有关更多信息，请参阅 [查看和管理 [!DNL Adobe Workfront] 来自Adobe Creative Cloud的通知](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-notifications.md).

有关安装Workfront forCreative Cloud插件的信息，请参阅 [安装适用于Creative Cloud应用程序的Adobe Workfront插件](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## 改进了通过拖放操作将文档移动到链接的文件夹时的体验

我们在将文档拖放到链接文件夹中的过程中添加了一些透明度。 现在，您移动到链接文件夹的文档将保留在文档列表中，直到完全移动为止。 文档选项已禁用，但您仍然可以在移动文档时打开该文档进行查看。 文档完成传输后，它会从文档列表中消失，因为它现在完全位于链接的文件夹中。

以前，在文档完成移动到链接的文件夹之前，文档会立即从文档列表中消失。

有关更多信息，请参阅 [链接来自外部应用程序的文档](/help/quicksilver/documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## 创建项目时自动创建链接文件夹到Adobe Experience Manager Assets

借助适用于Adobe Experience Manager集成的新创建链接文件夹工作流，您可以通过Adobe Experience Manager Assets文件夹的路径来配置集成。 当集成添加到项目模板时，从该模板创建的任何项目都将自动在Experience Manager Assets的指定文件夹中创建链接的子文件夹。

以前，创建链接文件夹需要用户执行操作。

此功能仅适用于Workfront中的Adobe Experience Manager as a Cloud Service集成。 这在Adobe Experience Manager增强型连接器中不可用。

有关更多信息，请参阅 [在Experience Manager Assets集成中使用工作流](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

## 将Workfront字段值映射到Experience Manager Assets中的标记

现在，您可以根据Workfront中的数据分类并快速查找资源。 您可以在Workfront for Experience Manager Assets集成中将此数据映射为元数据配置的一部分。

以前，将Workfront数据映射到Experience Manager Assets标记不可用。

有关Experience Manager Assetsas a Cloud Service中此功能的更多信息，请参阅 [配置 [!UICONTROL Experience Manager Assetsas a Cloud Service] 集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
有关Experience Manager Assets Essentials中此功能的更多信息，请参阅 [配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## 将Workfront字段映射到自定义Experience Manager Assets元数据字段

通过本机集成，您现在可以将本机字段和内置的Workfront字段映射到Experience Manager Assetsas a Cloud Service中的自定义元数据架构字段。

有关Experience Manager Assetsas a Cloud Service中此功能的更多信息，请参阅 [配置 [!UICONTROL Experience Manager Assetsas a Cloud Service] 集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
有关Experience Manager Assets Essentials中此功能的更多信息，请参阅 [配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## 使用Adobe Workfront调整自动验证工作流模板设置以进行Creative Cloud

您现在可以直接在Creative Cloud中调整现有的自动工作流模板设置。 选择现有的自动化工作流模板后，您可以：

* 禁用暂存
* 添加其他收件人
* 更改校对角色
* 调整截止日期
* 更新电子邮件通知
* 等等！

有关更多信息，请参阅 [上传文档和验证 [!DNL Adobe Workfront] 插件 [!DNL Creative Cloud] 应用程序](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-docs-proofs-toc.md).

这些增强功能可用于以下Creative Cloud应用程序：

* Photoshop
* XD
* InDesign
* Illustrator
