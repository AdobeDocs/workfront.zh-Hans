---
title: 2027年第一季度文档增强
description: 2027年第一季度文档增强
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 86dd87865046a4f2dc75e13feb370e338bbf4c92
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%
---

# 2027年第一季度文档增强

本页介绍了在2027年第一季度发布中对“预览”环境所做的文档增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2027年第一季度发布周期中此时可用的所有更改列表，请参阅[ 2027年第一季度发布概述](/help/quicksilver/product-announcements/product-releases/27-q1-release-activity/27-q1-release-overview.md)。

## Adobe Cloud Drive v1.2.0中的新增功能

>[!NOTE]
>
>预览： 2026年11月25日
>生产快速发布： 2026年11月25日
>适用于所有人的生产： 2026年11月25日
>[!BADGE 并发释放]{type=Neutral}
>[!BADGE 工作流程Ultimate]{type=Informative}

Adobe Cloud Drive v1.2.0中引入了上传文件、管理同步和使用云内容的新方法：

* **上传到云（直接上传）：**&#x200B;在Finder或文件资源管理器中右键单击某个文件以将其直接上传到Adobe云存储中的项目，而无需先将其复制到Adobe云驱动器文件夹中。 在同步活动的“直接上传”部分中监视进度。
* **暂停并继续同步：**&#x200B;在慢速连接或按流量计费的连接上暂停Adobe Cloud Drive，然后在准备就绪后继续。
* **版本历史记录：**&#x200B;浏览文件的已保存云版本，编辑版本名称和描述，并还原到早期版本。
* **管理本地存储：**&#x200B;监视本地磁盘使用情况、设置存储限制并查看此设备上标记为“始终”的文件。
* **同步活动：**&#x200B;查看最近的上传、下载和更改，并识别无法同步的项目。
* **在Workfront中打开：**&#x200B;直接从Finder、文件资源管理器或同步活动中打开项目的Workfront位置。

有关详细信息，请参阅[使用Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md)和[Adobe Cloud Drive疑难解答](/help/quicksilver/documents/adobe-cloud-drive/troubleshoot-adobe-cloud-drive.md)。

<!--

## Delegate unified document approvals

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now delegate your unified document approvals to another user, who can approve, reject, or mark reviews complete on your behalf during the delegation period. Delegated decisions show both names in the approval workflow, so it's clear who made each decision.

Legacy document and proof approvals remain unsupported.

For more information, see [Delegate approval request](/help/quicksilver/review-and-approve-work/manage-approvals/delegate-approval-requests.md).

-->

<!--

## Consistent review and approval buttons across documents

>[!NOTE]
>
>Preview: November 5, 2026
>Production fast release: December 17, 2026
>Production for everyone: January 21, 2027

Review and approval buttons now look and work the same everywhere you review documents: My approvals widget in Home, Document summary panel, the Document Details page, and the document preview page.

In addition to a new look and feel, some buttons have new names:

| Previous name | New name |
| --- | --- |
| Open proof | Open viewer |
| Review and approve | Make decision |
| Complete my review | Complete review |
| Open in Frame.io | Open viewer |

For more information, see [Review and approve documents](/help/quicksilver/documents/review-and-approve-documents.md).

-->

<!--

## Turn the Approved with changes decision on or off

>[!NOTE]
>
>Preview: November 5, 2026
>Production fast release: December 17, 2026
>Production for everyone: January 21, 2027

If your organization uses Adobe cloud storage, System Administrators can now turn the "Approved with changes" decision on or off for document approvals. When it's on, reviewers see three decisions (Approved, Approved with changes, and Needs Work) in both the Workfront approval interface and the Frame.io viewer. When it's off, reviewers see only Approved and Needs Work.

The setting lives on the Approval Settings page in Setup, and a live preview on that page shows exactly which decisions reviewers currently see.

For more information, see [Configure the Approved with changes decision](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/configure-approved-with-changes.md).

-->

## 配置统一的审核和批准电子邮件通知


>[!NOTE]
>
>预览： 2026年11月5日
>生产快速发布： 2026年11月12日
>适用于所有人的生产： 2027年1月21日

您现在可以配置统一的审核和批准电子邮件通知。 Workfront始终会发送这些电子邮件，但您现在无法配置它们。 现在有18个通知被分组为统一审批并默认处于活动状态。 Workfront管理员可以在“设置”中为每个人激活或取消激活这些受众，用户可以在他们的配置文件中管理这些受众。

作为此更新的一部分，这些通知的电子邮件主题行略有变化。 主题行现在以结果开头，例如“在{Document}上需要您的批准”。 有关批准总体结果的通知以“最终决定”开头，因此您可以将其与单个批准者的决定区分开来。

有关详细信息，请参阅[为系统中的每个人配置事件通知](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。
