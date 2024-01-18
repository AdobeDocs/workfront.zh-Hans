---
title: 21.3项目增强功能
description: 21.3项目增强功能
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 0%

---

# 21.3项目增强功能

本页介绍了21.3版本对“预览”环境所做的所有项目增强。 这些增强功能已在2021年7月21日这一周的生产环境中提供。

有关21.3版本可用的所有更改列表，请参阅 [21.3版本概述](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## 将模板与组关联

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用。

为了帮助您简化项目创建过程，并帮助您更轻松地识别和报告哪些组拥有哪些项目模板，我们增加了将组分配给项目模板的功能。

将组分配给项目模板时，从该模板创建的所有项目都会自动与模板的组相关联。 有关更多信息，请参阅 [编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

此外，如果模板与您的组相关联，则可以将组审批流程附加到模板及其模板任务。 有关更多信息，请参阅 [将新的或现有的审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 更轻松地编辑详细信息部分中的字段

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用。

通过下列改进，您可以更轻松地编辑任何对象的“详细信息”部分中的信息：

* 将鼠标悬停在字段上时，该字段周围的灰色轮廓表示该字段是可编辑的。
* 您可以通过单击字段一次来编辑它们。

在此增强功能之前，不清楚哪些字段可编辑，您必须双击才能编辑字段。

## 计算移交日期时考虑跨项目前置任务

随着Adobe Workfront计算任务移交日期的方式有了新的改进，跨项目依赖关系现在已考虑在内。

以前，仅根据同一项目中任务的前置任务计算切换日期。

现在，要确保始终为具有跨项目前置任务的任务提供准确的移交日期，必须重新计算后续任务的项目时间线。 在重新计算时间线后，任务的移交日期会在考虑任务的跨项目依赖性的情况下进行计算。

有关移交日期的详细信息，请参阅 [任务移交日期概述](../../../manage-work/tasks/task-information/handoff-task-date.md).

## 从Scrum展示板添加现有故事和问题

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用。

您现在可以直接从Scrum展示板添加现有故事或问题。 这样可以更轻松地向当前迭代添加现有故事，而无需转到积压事项页面。

有关更多信息，请参阅 [从Scrum展示板添加故事和问题](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## 从Scrum展示板添加新故事和问题

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用。

您现在可以直接从Scrum展示板创建新故事或问题。 这样可以更轻松地向当前迭代快速添加新故事。

有关更多信息，请参阅 [从Scrum展示板添加故事和问题](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## 从Kanban板中删除故事或问题

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用。

您现在可以通过单击文章或问题卡上的“更多”图标并选择删除，直接从Kanban展示板中删除文章或问题。 删除文章或问题后，该文章或问题将被移动到回收站保留30天，只有系统管理员才能恢复。

有关更多信息，请参阅 [从Kanban展示板中删除故事或问题](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## Agile信息卡页眉和故事板更新

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用。

在Kanban和Scrum展示板上，现在提供了以下增强功能：

* 故事卡和展示板列具有固定的宽度，因此，如果调整浏览器窗口大小，信息卡大小不会更改。
* “故事”列已重命名为“父故事”。
* 每个信息卡的顶部都有一个标签，用于将其标识为父故事、子任务（与父故事关联）、故事（与父故事不关联）或问题。
* 背景阴影以可视方式分隔列。

有关更多信息，请参阅 [迭代概述](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## 组项目、任务和问题偏好设置

正如我们先前所传达的，我们在截至2021年6月24日的阶段中推出了项目、任务和问题偏好设置的组级自定义。 现在推出已完成，并且可在生产环境中供所有客户使用。

有关更多信息，请参阅以下文章：

* [配置组的项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [配置组的任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## 允许外部用户审批文档

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用。

您现在可以使用外部电子邮件地址在新的Workfront Experience中将审批者分配给文档。

以前，您只能在Workfront Classic中按电子邮件地址添加外部用户。

有关更多信息，请参阅 [请求文档审批](../../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## 从项目组合或项目群的“详细信息”部分导出信息

>[!NOTE]
>
>此功能于2021年5月20日发布到“预览”环境。 该版本将于2021年6月3日发布到生产环境。

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用。

您现在可以从项目组合和程序的详细信息部分导出到.pdf文件信息。 在此增强功能之前，您只能从项目、任务和问题导出详细信息部分中的信息。

有关从对象导出自定义表单的信息，请参阅 [导出自定义表单和对象详细信息](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## 在对象标头中添加了“规划完成日期”时间戳

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用。

为了便于访问、方便且准确，我们添加了用于在项目、任务或问题标题的计划完成日期中选择时间戳的选项。

在此增强功能之前，当您更新对象的规划完成日期时，Workfront选择午夜作为默认时间。 现在，您可以自定义时间以及完成日期。

有关新Workfront Experience中对象标题的信息，请参阅 [新建对象标题](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## 将自定义表单添加到对象而不进行编辑

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用。

我们简化了将其他人将填写（或您稍后将填写）的自定义表单添加到对象的过程。 添加表单时，表单不再自动进入编辑模式。 您只需将空表单保存到对象中即可。

以前，将自定义表单添加到对象时，页面进入编辑模式，您必须先填写表单上的任何必填字段，然后才能将其保存到对象中。 当表单要由其他用户填写时，或者您不知道在表单上需要填写什么字段时，都会造成不便。

有关将自定义表单添加到对象的信息，请参阅 [向对象添加自定义表单](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

