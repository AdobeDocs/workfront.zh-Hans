---
title: 22.1项目增强功能
description: 22.1项目增强功能
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24f2aae-1c3d-41ed-ad17-6276bef2cf45
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 0%

---

# 22.1项目增强功能

本页介绍了22.1版本对“预览”环境所做的所有项目增强。 这些增强功能将在“生产”环境中提供

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年1月17日这一周。

有关22.1版本的所有可用更改列表，请参阅[22.1版本概述](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md)。

## 在复制或移动任务时更改前置任务的默认选项

为了最大限度地减少复制或移动任务时的手动步骤数，我们更新了默认情况下随任务一起复制或移动的信息。 现在，默认情况下，所有前置任务都会随任务一起复制或移动，因为默认情况下会选中所有前置任务选项。

在此增强功能之前，在复制或移动任务时，默认情况下会取消选择“所有前置任务”选项。

有关更多信息，请参阅以下文章：

* [复制和复制任务](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)
* [移动任务](../../../manage-work/tasks/manage-tasks/move-tasks.md)

## 更新了仪表板列表上的工具栏和仪表板中的报告

现在，四个仪表板页面上的工具栏具有符合其他Workfront列表（如项目、任务和问题）的现代外观。 现在，此直观的工具栏可让您更轻松地添加、编辑、共享、复制和删除功能板。

具有更新的工具栏的页面包括：

* 任务报告（显示在功能板中）
* 所有报告面板列表
* 我的报告面板列表
* “共享报告面板”列表

有关详细信息，请参阅[创建和管理功能板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-and-manage-dashboards.md)。

## 添加和编辑文档的自定义表单“摘要”面板

您现在可以直接在文档摘要面板中添加和编辑自定义表单。

通过此更改，您还将在文档摘要中看到新外观。 新增了“概述”部分，其中包含图像缩略图以及文档详细信息。 您还可以在文档详情部分检入和检出文档。

以前，您必须转到文档详细信息中的自定义表单选项卡才能进行编辑或添加自定义表单。

有关详细信息，请参阅[文档概述](../../../documents/managing-documents/summary-for-documents.md)的摘要。

## 复制一个或多个任务时的新体验

为了让您使用Workfront与新的Adobe Workfront体验保持一致，我们在复制任务时重新设计了界面。 在任务级别复制任务或在列表中复制任务或多个任务时，当前可使用此功能。

其中一些改进包括：

* 复制任务之前必须更新的所有信息都会显示在一个连续的页面上。
* Workfront会检查您是否有权在选择项目后立即访问目标项目。 在此增强功能之前，确认复制后会显示一则警告消息，指示您不具有正确的访问权限，这会导致额外的步骤，并且不允许复制操作。
* 能够在不离开复制任务框的情况下请求对要复制任务的项目的访问权限。

有关详细信息，请参阅[复制和复制任务](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

## 从列表移动一个或多个任务时的新体验

为了在执行同一任务时提供一致的体验，我们现在更新了用于从列表中移动一个或多个任务的界面，以在任务级别移动任务时匹配体验。 （在以前的预览版本中，我们更新了在任务级别移动任务的体验。）

有关详细信息，请参阅[移动任务](../../../manage-work/tasks/manage-tasks/move-tasks.md)。

## 在任务级别移动任务时的新体验

为了让您使用Workfront与新的Workfront体验保持一致，我们重新设计了用于移动任务的界面。 当前在任务级别移动任务时，此功能可用。 在下一个版本中，我们将将此重新设计扩展到从列表中移动任务。

此新设计的界面的一些改进包括：

* 移动之前必须更新的所有信息都会显示在一个连续的页面上。
* Workfront将在选择目标项目后立即检查您是否可以访问该项目。 在作出此改进之前，Workfront警告您，确认移动后您不再具有正确的访问权限，这会导致额外的步骤，并且不允许移动。
* 能够在不离开“移动任务”框的情况下请求对要移动任务的项目的访问权限。

有关详细信息，请参阅[移动任务](../../../manage-work/tasks/manage-tasks/move-tasks.md)。

## 在问题级别使用模板将问题转化为项目时的新体验

>[!NOTE]
>
>此功能已于2022年3月4日从生产环境中临时删除。 该版本后来在2022年4月28日开始分阶段发布。 推广已于2022年5月5日完成。 现在，该功能在“预览”和“生产”版中可供所有客户使用。 （有关此功能发布到生产环境的最新状态更新，请参阅[22.3版本概述](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md)。）

为了让您在使用Workfront时与新的Workfront体验保持一致，我们重新设计了界面，在您从问题页面转换模板时将问题转换为项目时，使用该界面。

现在，在选择转换问题后，您可以更轻松地立即访问收藏夹列表。

重新设计的界面与我们最近更新的模板创建项目时的体验相匹配。

有关详细信息，请参阅[在Adobe Workfront中将问题转化为项目](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)。

## 使用列表、报告和报告面板中的模板将问题转化为项目

>[!NOTE]
>
>此功能已于2022年3月4日从生产环境中临时删除。 该版本后来在2022年4月28日开始分阶段发布。 推广已于2022年5月5日完成。 现在，该功能在“预览”和“生产”版中可供所有客户使用。 （有关此功能发布到生产环境的最新状态更新，请参阅[22.3版本概述](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md)。）

为了提高您的工作效率并让您更轻松地在快节奏环境中转化问题，我们添加了使用列表、报告或功能板中的模板将问题转化为项目的功能。

在此增强功能之前，仅当您从问题页面转换问题时，此功能才存在。

有关详细信息，请参阅[在Adobe Workfront中将问题转化为项目](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)。

## 在敏捷展示板上按用户列表筛选，显示分配最多的用户排在首位

>[!NOTE]
>
>此功能将不包含在22.1版本中。 已从预览环境中将其删除。

现在，过滤器先显示分配最多的用户，这样用户无需滚动列表即可更轻松地找到。

以前，Kanban和Scrum展示板上的按用户列表筛选条件按字母顺序显示。

有关更多信息，请参阅以下信息

* [在Scrum展示板上按用户筛选](../../../agile/use-scrum-in-an-agile-team/scrum-board/filter-by-user-scrum-board.md)
* [在Kanban展示板上按用户筛选](../../../agile/use-kanban-in-an-agile-team/filter-by-user.md)

## 限制向要共享的模板添加文档的功能

有时候，人们会以为自己正在将文档添加到项目中，而将文档添加到项目模板中。 现在，您可以帮助防止出现这种情况 — 当您共享具有“查看”权限的模板时，可以禁用新的高级设置“添加文档”。 这将禁用收件人向模板添加文档的能力。

有关共享模板的说明，请参阅[共享项目模板](../../../manage-work/projects/create-and-manage-templates/share-project-template.md)。

有关新的高级设置“添加文档”的信息，请参阅文章[共享模板](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)中的部分。

## 共享文档文件夹

现在，您可以从“文档”区域共享文档文件夹及其内容。 以前这样做是不可能的 — 您必须单独共享文件夹中的每个文档。

有关详细信息，请参阅[共享文档文件夹](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md)。

