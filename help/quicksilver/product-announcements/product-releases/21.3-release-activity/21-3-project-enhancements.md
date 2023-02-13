---
title: 21.3项目增强功能
description: 21.3项目增强功能
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 0%

---

# 21.3项目增强功能

本页介绍了在“预览”环境中21.3版本所做的所有项目增强功能。 这些增强功能在2021年7月21日这一周的生产环境中提供。

有关21.3版本中可用的所有更改的列表，请参阅 [21.3版本概述](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## 将模板与组关联

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用。

为了帮助您简化项目创建过程，并帮助您更轻松地确定和报告哪些组拥有哪些项目模板，我们增加了将组分配给项目模板的功能。

在将组分配给项目模板时，使用该模板创建的所有项目都会自动与该模板的组关联。 有关更多信息，请参阅 [编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

此外，如果模板与您的组关联，则可以将组批准流程附加到模板及其模板任务。 有关更多信息，请参阅 [将新审批流程或现有审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 更轻松地编辑详细信息部分中的字段

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用。

通过以下改进，您可以更轻松地编辑任何对象的“详细信息”部分中的信息：

* 将鼠标悬停在字段上时，该字段周围的灰色轮廓表示该字段是可编辑的。
* 您可以通过单击一次字段来编辑它们。

在进行此增强之前，不清楚哪些字段可编辑，您必须双击才能编辑字段。

## 在计算切换日期时，请考虑跨项目前置任务

随着Adobe Workfront计算任务切换日期方式的新改进，现在考虑了跨项目依赖关系。

以前，切换日期仅基于来自同一项目的任务的先前任务来计算。

现在，为确保始终具有跨项目前置任务的准确切换日期，您必须重新计算后续任务项目的时间表。 在重新计算时间表后，计算任务的切换日期时考虑任务的跨项目依赖关系。

有关切换日期的更多信息，请参阅 [任务切换日期概述](../../../manage-work/tasks/task-information/handoff-task-date.md).

## 从Scrum展示板添加现有文章和问题

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用。

现在，您可以直接从Scrum展示板添加现有文章或问题。 这样，您就可以更轻松地将现有文章添加到当前小版本，而无需转到积压工作页面。

有关更多信息，请参阅 [添加Scrum展示板中的文章和问题](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## 从Scrum展示板添加新文章和问题

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用。

现在，您可以直接从Scrum展示板创建新文章或问题。 这样，就可以更轻松地向当前小版本快速添加新文章。

有关更多信息，请参阅 [添加Scrum展示板中的文章和问题](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## 从看板板中删除文章或问题

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用。

现在，您可以通过单击文章或发行卡上的更多图标并选择删除，直接从看板板中删除文章或发行。 删除文章或问题时，该文章或问题会移到回收站30天，并且只能由系统管理员恢复。

有关更多信息，请参阅 [从看板板中删除文章或问题](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## 敏捷卡片标题和文章板更新

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用。

在看板和看板板上，现在提供了以下增强功能：

* 文章卡片和展示板列具有固定的宽度，因此，如果您调整浏览器窗口大小，卡片大小不会发生变化。
* 文章列已重命名为父文章。
* 每张卡片顶部都有一个标签，用于将其标识为父文章、子任务（与父文章关联）、文章（与父文章不关联）或问题。
* 背景底纹以可视方式分隔列。

有关更多信息，请参阅 [迭代概述](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## 将项目、任务和问题首选项分组

正如我们之前所说，我们在2021年6月24日之前的各个阶段中针对项目、任务和问题首选项推出了组级自定义。 现在，推出已完成，可在生产中供所有客户使用。

有关更多信息，请参阅以下文章：

* [为组配置项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [为组配置任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## 允许外部用户批准文档

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用。

现在，您可以使用外部电子邮件地址将批准者分配给新Workfront体验中的文档。

以前，您只能在Workfront Classic中通过电子邮件地址添加外部用户。

有关更多信息，请参阅 [请求文档批准](../../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## 从组合或项目群的Details部分导出信息

>[!NOTE]
>
>此功能于2021年5月20日发布到预览环境。 它将于2021年6月3日发布到生产环境。

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用。

您现在可以从项目组合和项目群的Details部分导出为.pdf文件信息。 在进行此增强之前，您只能从项目、任务和问题的“详细信息”部分导出信息。

有关从对象导出自定义表单的信息，请参阅 [导出自定义表单和对象详细信息](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## 在对象标题中添加了“计划完成日期”时间戳

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用。

为了方便访问、方便和准确，我们在项目、任务或问题标题的计划完成日期中添加了选择时间戳的选项。

在进行此增强之前，当您更新对象的计划完成日期时，Workfront会选择午夜作为默认时间。 现在，您可以自定义完成日期和时间。

有关新Workfront体验中对象标题的信息，请参阅 [新对象标头](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## 将自定义表单添加到对象，而不进行编辑

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用。

我们更轻松地向对象中添加其他人将填写或稍后将填写的自定义表单。 添加表单后，表单不再自动进入编辑模式。 您只需将空表单保存到对象即可。

以前，在将自定义表单添加到对象时，页面会进入编辑模式，您必须填写表单上的任何必填字段，然后才能将其保存到对象。 当表单用于供其他用户填写，或者当您还不知道在表单上的必填字段中放置什么时，这会很麻烦。

有关将自定义表单添加到对象的信息，请参阅 [将自定义表单添加到对象](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

