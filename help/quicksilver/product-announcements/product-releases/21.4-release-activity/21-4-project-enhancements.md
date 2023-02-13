---
title: 21.4项目增强功能
description: 21.4项目增强功能
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 6bcd332e-bd4e-4a74-bae9-9ba507299a51
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# 21.4项目增强功能

本页介绍了在“预览”环境中21.4版本所做的所有项目增强功能。 这些增强功能将于2021年10月4日这一周的生产环境中提供。

有关21.4版本中可用的所有更改的列表，请参阅 [21.4版本概述](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## 在更新中包含图像

在对象的更新选项卡中，您现在可以通过单击工具栏中的图像图标来添加图像。 您还可以将图像拖放到更新区域中。 请注意，您的Workfront管理员必须先启用添加图像，然后才能看到图像图标。

您可以在更新和回复中添加图像。 更新中的图像缩略图表示收件人可以在浏览器中预览或下载图像，而电子邮件和应用程序内通知则显示图像已附加到更新中。

以前，在Workfront中共享图像的唯一方法是将图像作为文档附加到对象。 在“更新”选项卡中添加的图像仅在该选项卡上可用，而不在“文档”选项卡上可用。

有关更多信息，请参阅 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

在Workfront用户可以在更新中包含图像之前，此功能必须首先由Adobe Workfront管理员启用，如 [配置用户更新的首选项](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

## 更新了智能分配的算法

我们改进了智能分配时使用的算法。 通过新的改进，Workfront将检查登录用户在分配任务和问题时所做的30项最新分配，以提出建议。 建议列表最多可包含50个用户。

在进行此增强之前，Workfront在建议用户时会考虑父任务上的分配以及与这些分配相关的其他用户属性。

有关智能分配的信息，请参阅 [智能分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## 从模板创建项目时的新体验

为了让您使用Workfront与新的Workfront体验保持一致，我们重新设计了用于从模板创建项目的界面。 使用模板创建项目的功能没有更改。 但是，这个新重新设计的界面的一些改进包括：

* 在附加模板信息之前预览模板信息
* 在项目创建过程中向收藏列表添加模板

在从“项目”和“模板”区域创建项目时，我们都更新了用于创建项目的界面。

有关信息， [使用模板创建项目](../../../manage-work/projects/create-projects/create-project-from-template.md).

## 将模板附加到项目时的新体验

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用。

为了让您使用Workfront与新的Workfront体验保持一致，我们重新设计了用于将模板附加到项目的界面。 附加模板的功能未发生更改。 但是，这个新重新设计的界面有一些改进，包括：

* 在附加模板信息之前预览模板信息
* 在附件过程中向收藏列表添加模板
* 在一个连续的页面中查看用于管理模板和项目设置的所有选项

有关信息，请参阅 [将模板附加到项目](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## 任务的统一持续时间和持续时间单位值

为了获得更简洁、更简单的用户体验，我们已将“持续时间”字段的值与持续时间单位进行了合并。 在进行此增强之前，时间单位会显示在“持续时间”字段后面的单独下拉字段中。

除了任务详细信息、编辑任务和新任务框中的持续时间字段之外，我们还要更新以下字段以匹配此体验：

* 进行高级分配时的持续时间字段
* 在创建或编辑任务时调平延迟字段
* 创建定期任务时的频度字段（即将提供）
* 添加前置任务时的延迟字段（即将提供）

有关信息，请参阅 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

![](assets/duration-combined-field-350x139.png)

## 禁用在项目中添加内联问题

为确保用户在填写问题表单向项目添加问题时提供准确信息，我们引入了新设置，以便您管理他们是否可以在项目中添加问题，还是可以在内联执行任务。 默认情况下，在“编辑项目”框的新“问题设置”区域中启用此设置。 禁用此选项会导致项目“问题”部分中的“添加更多问题”选项变为不可用，因此用户无法在列表中添加任何其他问题。 用户仍可以使用“问题”部分中的“新问题”选项或使用请求队列（如果为项目配置了请求队列），向项目添加问题。

>[!NOTE]
>
>此设置仅在新的Workfront体验中可用。 在Workfront Classic中工作的用户仍可以在项目或其任务中添加内嵌问题，即使在新Workfront体验中工作的用户为项目禁用了此设置的情况下也是如此。

有关更多信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

## 对复选框和单选按钮的自定义字段显示改进

在自定义表单中查看和选择复选框和单选按钮选项变得更轻松了 — 现在，具有许多复选框或单选按钮选项的自定义字段会显示在页面的多个列中。 以前，它们会显示在一列中，这要求用户在填写表单时需要额外滚动。

这取决于您在自定义表单中放置字段的方式 — 如果将另一个字段与复选框或单选按钮字段放在同一行，则选项可能只有足够的水平空间在单列中显示。

有关填写自定义表单的信息，请参阅 [编辑自定义表单字段中的信息](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

有关在自定义表单中创建复选框或单选按钮字段的信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) 和 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#configur) 在文章中 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

