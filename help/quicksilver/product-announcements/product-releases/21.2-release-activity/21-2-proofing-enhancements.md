---
content-type: release-notes
keywords: 注释，季度，更新，版本
navigation-topic: 2021-2-release-activity
title: 21.2校对增强功能
description: 本页介绍了21.2版本对“预览”环境所做的所有“验证”增强。 这些增强功能将在2021年5月10日这一周的“生产”环境中提供。 有关21.2版本中可用的所有更改列表，请参阅21.2版本概述。
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 1f82c397-5cb6-4adc-bb84-f5b1e1ed9d5e
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# 21.2校对增强功能

本页介绍了21.2版本对“预览”环境所做的所有“验证”增强。 这些增强功能将在2021年5月10日这一周的“生产”环境中提供。 有关21.2版本可用的所有更改列表，请参阅 [21.2发行版概述](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## 验证决策现在显示在文档列表中

>[!NOTE]
>
>仅在新的Adobe Workfront Experience中可用。

总体验证决策现在显示在默认文档列表视图中。

通过此增强功能，您可以轻松地直接在默认列表视图中查看具有总体决策的所有验证。 这样，无需导航到不同页面即可非常轻松地识别验证进度。

以前，需要转到文档详细信息和验证工作流以查看整个验证决策，这需要单击多次。

有关校对决策的详细信息，请参阅 [“文档”区域](../../../documents/managing-documents/documents-area.md).

此功能现已包含在 [管理新版Workfront Experience中的验证和版本](https://one.workfront.com/s/learningpath3/manage-proofs-and-versions-in-the-new-workfront-experience-MCPBYNLTQSS5H4NG7C27IPCVR5YA) Workfront One学习路径。

## 验证审批报告的新字段

为了帮助显示有用的验证信息，我们在验证审批报告中添加了以下字段：

* **决策日期：** 显示审批者对验证做出决定的日期。 您还可以在证明的打印摘要中找到此日期。
* **审批阶段：** 显示当前阶段信息。
* **工作流模板：** 显示附加到验证的任何工作流模板。 如果没有附加模板，则该列为空。

这些字段不是默认报表的一部分。 如果您想查看这些幻灯片，则需要添加这些幻灯片。

此功能现已包含在 [证明系统设置，第2部分：工作流管理](https://one.workfront.com/s/learningpath3/proof-system-setups-part-2-workflow-management-MCKUF6NTIJ6BGMXHBCXXX6NN53EA) Workfront One学习路径。

## 生成新版本时结转现有验证工作流

>[!NOTE]
>
>此功能于2021年3月30日从预览环境中移除，并于2021年4月1日从生产环境中移除。 它不会包含在21.1版本中。

现在，现有的校样工作流会传递到您创建的任何新版本，无论这些版本是在什么方法中生成的。

以前，验证工作流的传送方式略有不同，具体取决于您在Workfront中生成它们的位置。

有关更多信息，请参阅 [创建新版本的验证](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/create-new-proof-version.md).
