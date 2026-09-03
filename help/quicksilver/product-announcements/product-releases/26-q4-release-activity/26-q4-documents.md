---
title: 2026年第四季度文档增强
description: 2026年第四季度文档增强
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: ee1fceee828c97db535ccc03c8b428940d6f7eed
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 0%

---

# 2026年第四季度文档增强

本页介绍了在2026年第四季度发行版中对“预览”环境所做的文档增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2026年第四季度发布周期中此时可用的所有更改列表，请参阅[2026年第四季度发布概述](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)。

<!--

## Frame comment visibility in Workfront

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

When an approval workflow is created for a document, users can leave comments and make annotations in the Frame.io viewer. These comments are not displayed in the Workfront Comments panel, but you can view them in the Frame.io viewer.

Now, the Comments panel in Workfront displays a message letting you know when new comments are available in Frame.io.

For more information, see [Add an update to a document](/help/quicksilver/documents/managing-documents/add-update-documents.md).

-->

## 通过审批电子邮件链接直接验证访问

>[!NOTE]
>
>预览：不适用
>生产快速发布： 2026年9月17日
>适用于所有人的生产： 2026年10月15日

当文档附加了验证时，审批电子邮件中的“前往审阅”链接现在直接打开验证查看器，因此审阅者和审批者可以立即开始审阅。 如果文档没有验证，则链接将继续打开文档的审批部分，就像之前一样。

<!--

## Add teams to approvals for objects using Adobe cloud storage

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

You can now add a Workfront Team as an approver or reviewer on a document approval or approval template, instead of adding each person individually:

* Objects on Adobe cloud storage: Workfront adds each active team member individually, so the approver list always reflects who's currently on the team.
* Objects using legacy Workfront storage: The team is added as a single participant by default, but you can now choose to add each team member as an individual participant.
* In approval templates, Workfront stores a reference to the team and expands it into active members when you apply the template to a document, not when you save the template.

For more information, see:

* [Create an approval workflow in the new Documents area](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-new-documents-area)
* [Create an approval workflow in the legacy documents area](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-in-the-legacy-documents-area)
* [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

-->

## 在项目模板上设置Frame.io工作区

>[!NOTE]
>
>预览： 2026年9月3日
>生产快速发布： 2026年9月17日
>适用于所有人的生产： 2026年10月15日

如果贵组织使用Adobe云存储，并且您拥有Frame.io企业许可证，则现在可以在项目模板的项目详细信息中选择Frame.io工作区。 从模板创建的项目会自动使用模板上设置的工作区，因此项目会被路由到所需的Frame.io工作区，而无需在创建项目时执行额外的操作。

新字段列出了您有权为其分配项目的Frame.io工作区。 该字段在模板上随时保持可编辑状态；更改仅适用于更新后创建的项目，因此现有项目会保留其原始工作区。

从模板创建项目后，其Frame.io工作区字段为只读，并且链接到Frame.io中的工作区。

如果您没有Frame.io Enterprise许可证，则项目将继续转到Workfront的默认工作区。

有关详细信息，请参阅[编辑项目模板](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md)和[管理项目概述区域中的信息](/help/quicksilver/manage-work/projects/manage-projects/understand-project-overview-area.md)。

<!--

## Consistent review and approval buttons across documents

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

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

## 电子邮件主题行中的自定义消息

>[!NOTE]
>
>预览：不适用
>生产快速发布： 2026年9月17日
>适用于所有人的生产： 2026年10月15日

现在，当您为文档审批设置自定义消息时，该消息也会显示在审批请求电子邮件的主题行中，在设置该消息时以截止日期为开头。 这样，查看者无需打开电子邮件，即可直接从其收件箱中查看需要注意的事项和方式。

有关详细信息，请参阅[创建文档审批工作流](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。

<!--

## Redesigned Versions panel in the new documents area

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

If your organization uses Adobe cloud storage, the Versions panel in the new Documents area has a new design:

* Versions are labeled V1, V2, and so on to drive consistency with Frame.io.
* Each version shows its approval status, such as "Approved" or "Withdrawn", directly in the list.
* The panel now lists only Version history — there's no longer a separate "latest file" entry at the top.

Previously, versions were timestamped instead of numbered.

For more information, see [Manage document versions](/help/quicksilver/documents/managing-documents/manage-document-versions.md).

## Redesigned Approvals panel in the new documents area

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

If your organization uses Adobe cloud storage, the Approvals panel in the new Documents area now shows approval history across versions:

* The panel lists the approval workflow for every version that has one, not just the current version.
* Withdrawn workflows stay in the list, so you can still review their prior decisions.
* Expand any version to see its stages, approver decisions, decision rule, and due dates without leaving the panel.

Previously, the Approvals panel only showed the current version's workflow.

For more information, see [Create a document approval workflow](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

-->

## 将图像附加到对Adobe云存储对象的注释中

>[!NOTE]
>
>预览： 2026年7月30日
>生产快速发布： 2026年7月30日
>适用于所有人的生产： 2026年7月30日
>[!BADGE 超出计划]{type=Neutral}

作为统一审阅和批准的一部分使用Adobe云存储的组织现在可以将图像文件直接附加到注释中，将反馈、上下文和支持可视化一起保留在单个可跟踪的注释线程中。 这弥补了之前的空白：只有旧版Workfront存储中的组织才能将图像附加到评论。

Adobe云存储组织现在支持所有媒体类型图像格式。 （旧版对象注释仍仅支持.jpg、.gif和.png文件。） 旧版或Adobe云存储对象的注释不支持非图像文件。

有关详细信息，请参阅[更新工作](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

## 将Experience Manager Assets中的资源与Adobe云存储关联

>[!NOTE]
>
>预览： 2026年7月30日
>生产快速发布： 2026年8月13日
>适用于所有人的生产： 2026年10月15日

如果您的组织使用Adobe云存储，则可以将Experience Manager Assets中的单个资源链接到支持文档的任何Workfront对象。 链接的内容会自动保持同步：在Experience Manager Assets中所做的更改会显示在Workfront中，并且您无需离开Workfront即可引入新的资源版本。

链接功能由内容审查工具提供支持，因此，您还可以在选择内容时获得AI 搜索、智能建议、营销活动简短分析等。

有关详细信息，请参阅[将Experience Manager Assets中的内容与Adobe云存储关联](/help/quicksilver/review-and-approve-work/native-integrations/link-aem-assets-cloud-storage.md)。
