---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 Beta 3发行版活动
description: 本页介绍了2017.2 Beta 2版本在“预览”环境中提供的所有更改。 2017年5月24日，预览环境中提供了此页面上的功能。 该版本将于2017年7月底至8月初在“生产”环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9647f3c6-f287-426c-a5e7-eb33b8b22a34
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 0%

---

# 2017.2 Beta 3发行版活动

本页介绍了2017.2 Beta 2版本在“预览”环境中提供的所有更改。 2017年5月24日，预览环境中提供了此页面上的功能。 该版本将于2017年7月底至8月初在“生产”环境中提供。

>[!IMPORTANT]
>
>此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2017.2版中所做所有更改的列表，请参阅[2017.2版活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md)。

2017.2 Beta 2版本包含面向Workfront管理员和其他用户的增强功能：

管理员的&#x200B;**：**

* [正在从回收站批量还原项目](#restoring-items-in-bulk-from-the-recycle-bin)
* [用户信息从Workfront同步到ProofHQ(ProofHQ和Workfront)](#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront)

所有用户&#x200B;**：** 

* [查看订阅的用户](#view-subscribed-users)
* [配置里程碑在甘特图上的显示方式](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* 导出到PDF时[包含甘特图图例](#include-the-gantt-chart-legend-when-exporting-to-pdf)
* [在“我的工作区(Workfront)”中查看校对审批](#view-proof-approvals-in-the-my-work-area-workfront)
* [从我的工作区(Workfront)处理验证审批请求时查看用户名](#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront)
* [改进了视频校对(ProofHQ和Workfront)的校对查看器](#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront)
* [以备用分辨率(ProofHQ和Workfront)查看富媒体校样](#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront)
* 文档版本报告(Workfront)中的[新“校对创建者”对象](#new-proof-creator-object-in-document-version-report-workfront)
* [新资源池功能暂时从预览中删除](#new-resource-pool-functionality-temporarily-removed-from-preview)

## 从回收站批量恢复项目 {#restoring-items-in-bulk-from-the-recycle-bin}

您现在一次最多可以恢复10个已删除的项目、任务、问题或文档。

在此更改之前，一次只能恢复一个已删除的项目。

有关还原项目的详细信息，请参阅[还原已删除的项目](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。

## 查看订阅的用户 {#view-subscribed-users}

您现在可以通过扩展订阅链接旁边显示的订阅者数量来查看项目的订阅者。

在此增强功能之前，您不知道谁订阅了任何项目。

有关订阅项目的详细信息，请参阅[在Adobe Workfront中订阅项目](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)。 

## 配置里程碑在甘特图上的显示方式 {#configure-how-milestones-are-displayed-on-the-gantt-chart}

现在，可以使用两个选项来查看甘特图中的里程碑信息。 您可以配置以下里程碑指示器之一或两者：

* 里程碑菱形（图标）

  此图标显示在甘特图中与里程碑关联的任何任务之后。

* 里程碑线

  与里程碑关联的任何任务后面会显示一条直线，横跨甘特图中的所有任务。

在此更改之前，只有一个选项允许里程碑显示在甘特图上，称为“里程碑”。 此选项同时启用了里程碑菱形图标和里程碑线。 无法分隔这些指示器。

有关配置信息在甘特图中的显示方式的更多信息，请参阅[配置信息在甘特图中的显示方式](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)。

## 导出到PDF时包含甘特图图例 {#include-the-gantt-chart-legend-when-exporting-to-pdf}

在将甘特图导出到PDF时，现在可以选择是否同时导出图表的图例以及图表本身。 图例中包含的项目只是您已启用以便在UI的甘特图中显示的选项。 如果项目任务中存在这些选项，则它们会包含在图例中。 例如，如果启用“甘特图”中的“里程碑”显示功能，则图例也会显示它们，但前提是至少有一个任务与里程碑关联。

在此更改之前，无法从导出的PDF中排除图例，并且该图例包含甘特图的所有可能选项和标记，无论它们在UI中是已启用还是存在。

有关导出甘特图的详细信息，请参阅[将甘特图导出到PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)。

## 用户信息从Workfront同步到ProofHQ(ProofHQ和Workfront) {#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront}

现在，在Workfront中创建或更新用户时，用户信息（姓名和电子邮件）会从Workfront同步到ProofHQ。 

有关用户从Workfront同步到ProofHQ的更多信息，请参阅。

## 文档版本报告(Workfront)中的新“验证创建者”对象

{#new-proof-creator-object-in-document-version-report-workfront}

现在，创建文档版本报告时，存在新的“校样创建者”对象。 利用此对象，可报告有关创建验证的用户的信息。 

文档版本报告中的新“校样创建者”对象包含其他类型对象报告中的现有“用户”对象可用的所有字段。

>[!NOTE]
>
> 仅从首次将此功能引入相应的预览或生产环境开始，报告中才提供此信息；在引入此功能之前，报告中有关请求者对象的信息不可用。

创建文档版本报告时，您可以访问校样创建者对象，如[创建自定义报告](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)中所述。

有关文档版本对象报表的更多信息，请参阅[了解Adobe Workfront中的对象](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)中的[了解Adobe Workfront中的对象](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)部分。

## 在“我的工作区”(Workfront)中查看验证审批 {#view-proof-approvals-in-the-my-work-area-workfront}

现在，您已提交审批的所有验证审批都显示在“我的工作”区域的&#x200B;**我已提交审批的工作**&#x200B;选项卡中。

在此更改之前，我已提交审批的&#x200B;**工作**&#x200B;选项卡不包括验证审批。

仅当满足以下条件时，才会显示验证审批：

* 审批当前为未决批准
* 审批流程会分配给拥有许可的Workfront用户(不会显示分配给未获得许可的Workfront用户的审批流程)
* 在发放此功能后启动审批流程（不显示发放此功能前启动的审批流程）

有关详细信息，请参阅[查看审批](../../../../review-and-approve-work/manage-approvals/view-approvals.md)中的[查看审批](../../../../review-and-approve-work/manage-approvals/view-approvals.md)。

## 从“我的工作区”(Workfront)处理验证审批请求时查看用户名 {#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront}

现在，当从“我的工作”区域审批验证审批时，将显示请求审批的用户的名称。

有关详细信息，请参阅[批准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md)中的[批准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md)。 

## 改进了视频校样的校对查看器(ProofHQ和Workfront) {#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront}

Workfront和ProofHQ中的校对查看器正在更新，其中包含新的外观、用于提高性能的HTML5架构以及对新功能的支持。

新的校对查看器包含以下改进：

* 逐帧校对
* 视频缓冲
* 评论列表中的搜索功能
* 对注释设置的任何操作都会显示在“注释列表”的每个注释中
* 全屏模式
* 以更快或更慢的速度查看内容
* 添加评论和回复时的拼写检查器

### 预览

新的验证查看器可用于在以下预览环境中测试：

* proofhq预览环境

  有关ProofHQ预览环境的更多信息，请参阅[预览Sandbox测试环境 — Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md)。

* Workfront预览环境，当帐户已启用验证时

  有关“Workfront预览”环境的更多信息，请参阅  [Adobe Workfront预览沙盒环境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)。

在此版本中，新的校对查看器仅支持视频校对。 这意味着所有视频校样都利用新的校样查看器，而所有静态和富媒体校样都继续利用现有的校样查看器。

### 生产

在17.2版本中发布到生产环境后，管理员可以选择新验证查看器或旧验证查看器是否适合其组织中的用户。 默认情况下，将使用旧版验证查看器。

有关如何使用新的视频校对查看器的信息，请参阅  

## 以备用分辨率查看富媒体校样(ProofHQ和Workfront) {#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront}

您现在可以通过指定自定义分辨率或将图像拖动到所需分辨率来调整富媒体验证的分辨率。

在此更改之前，您可以仅使用查看内容的屏幕或设备固有的分辨率来查看校样。

您可以使用比较模式来比较不同的验证分辨率。

有关详细信息，请参阅[在桌面验证查看器中打开验证](../../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/open-proofs-in-dpv.md)。 

## 新资源池功能暂时从预览中删除 {#new-resource-pool-functionality-temporarily-removed-from-preview}

由于开发方面的挑战，我们决定删除新的“资源规划”选项卡，并将“旧版资源规划”选项卡重命名回其原始名称“资源规划”。

新的资源池功能也随此更改一起删除。 资源规划的新选项卡和资源池的功能将于2017年6月底返回到“预览沙盒”环境。
