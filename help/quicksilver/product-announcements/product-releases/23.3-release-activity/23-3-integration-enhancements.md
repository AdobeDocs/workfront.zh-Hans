---
title: 23.3集成增强功能
description: 23.3集成增强功能
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24ddc8a-fe96-4e9b-8186-0b54ab9ab213
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 0%

---

# 23.3集成增强功能

本页介绍了随23.3版本一起进行的所有集成增强。 这些增强功能在2023年7月20日和21日发布的23.3版本的生产环境中提供。

有关23.3发行周期中此时可用的所有更改列表，请参阅 [23.3发行版概述](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

## 新的G Suite集成现已推出

Google Marketplace中现在提供了新的G Suite集成。 新的集成使用OAuth2进行身份验证，并替换以前的集成。

以前的G Suite集成现已弃用，并将自动卸载。

有关如何安装新集成的说明，请参阅 [安装 [!DNL Adobe Workfront for G Suite]](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

有关适用于G Suite的Workfront的更多信息，请参阅 [适用于G Suite的Workfront](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md).

## Adobe Creative Cloud集成现在支持多个已分配用户

当任务或问题具有多个分配用户时，Adobe Creative Cloud集成现在支持在“完成我的部分”和“完成”（或“已解决”）之间进行选择。

以前，集成允许用户将任务标记为完成，而无需指定“我的部分已完成”或“已完成”/“已解决”。

要利用此功能，请下载并安装最新的WorkfrontCreative Cloud插件。

有关该功能的更多信息，请参阅 [使用Adobe Workfront插件将工作项标记为完成](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-complete.md).

有关安装Workfront forCreative Cloud插件的信息，请参阅 [安装适用于Creative Cloud应用程序的Adobe Workfront插件](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## 从Workfront查看和管理Workfront通知以了解Creative Cloud插件

为了让您更轻松地接收所需的通知，我们让您能够在不离开Adobe Creative Cloud的情况下查看和管理Workfront通知。 现在，您可以直接从Creative Cloud应用程序的Workfront插件窗口中查看通知，以及访问与这些通知相关的工作项和注释。

以前，通知只能在Workfront中通过电子邮件提供。

要利用此功能，请下载并安装最新的WorkfrontCreative Cloud插件。

有关更多信息，请参阅 [查看和管理 [!DNL Adobe Workfront] 来自Adobe Creative Cloud的通知](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-notifications.md).

有关安装Workfront forCreative Cloud插件的信息，请参阅 [安装适用于Creative Cloud应用程序的Adobe Workfront插件](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

<!--

## Improved experience when moving a document to a linked folder with drag and drop

We've added some transparency to the process of dragging and dropping a document into a linked folder. Now, the document that you moved to a linked folder remains in the document list until it has fully moved. The document options are disabled, but you can still open the document for view while it is moving. When the document has completed the transfer, it disappears from the document list, because it is now fully located in the linked folder.

Previously, documents would immediately disappear from the document list, before they had finished moving to the linked folder.

For more information, see [Link documents from external applications](/help/quicksilver/documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

-->

## 创建项目时自动创建链接文件夹到Adobe Experience Manager Assets

借助适用于Adobe Experience Manager集成的全新创建链接文件夹工作流，您可以配置集成以及指向Adobe Experience Manager Assets文件夹的路径。 当集成添加到项目模板时，从该模板创建的任何项目都会在Experience Manager Assets的指定文件夹中自动创建链接的子文件夹。

以前，创建链接文件夹需要用户执行操作。

此功能只能与Workfront中的Adobe Experience Manager as a Cloud Service集成一起使用。 Adobe Experience Manager增强型连接器中不提供此功能。

有关更多信息，请参阅 [在Experience Manager Assets集成中使用工作流](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

## 将Workfront字段值映射到Experience Manager Assets中的标记

现在，您可以根据Workfront中的数据分类和快速查找资源。 您可以在Workfront for Experience Manager Assets集成中将此数据映射为元数据配置的一部分。

以前，将Workfront数据映射到Experience Manager Assets标记不可用。

有关Experience Manager Assetsas a Cloud Service中此功能的更多信息，请参阅 [配置 [!UICONTROL Experience Manager Assetsas a Cloud Service] 集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
有关Experience Manager Assets Essentials中此功能的更多信息，请参阅 [配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## 将Workfront字段映射到自定义Experience Manager Assets元数据字段

通过本机集成，您现在可以将本机字段和内置的Workfront字段映射到Experience Manager Assetsas a Cloud Service中的自定义元数据架构字段。

有关Experience Manager Assetsas a Cloud Service中此功能的更多信息，请参阅 [配置 [!UICONTROL Experience Manager Assetsas a Cloud Service] 集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
有关Experience Manager Assets Essentials中此功能的更多信息，请参阅 [配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## 使用用于Creative Cloud的Adobe Workfront调整自动验证工作流模板设置

您现在可以直接在Creative Cloud中调整现有的自动工作流模板设置。 选择现有的自动化工作流模板后，您可以：

* 禁用阶段
* 添加其他收件人
* 更改验证角色
* 调整截止日期
* 更新电子邮件通知
* 等等！

有关更多信息，请参阅 [使用上传文档和验证 [!DNL Adobe Workfront] 插件 [!DNL Creative Cloud] 应用程序](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-docs-proofs-toc.md).

这些增强功能适用于以下Creative Cloud应用程序：

* Photoshop
* XD
* InDesign
* Illustrator
