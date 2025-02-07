---
title: 21.4项目增强功能
description: 21.4项目增强功能
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6bcd332e-bd4e-4a74-bae9-9ba507299a51
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---

# 21.4项目增强功能

本页介绍了21.4版本对“预览”环境所做的所有项目增强。 这些增强功能将在2021年10月4日当周的生产环境中提供。

有关21.4版本的所有可用更改列表，请参阅[21.4版本概述](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md)。

## 在更新中包含图像

在对象的“更新”选项卡上，您现在可以通过单击工具栏上的“图像”图标来添加图像。 您还可以将图像拖放到更新区域中。 请注意，Workfront管理员必须启用添加图像功能，您才能看到图像图标。

您可以在更新和回复中添加图像。 更新中的图像缩略图表示收件人可以在浏览器中预览或下载图像，而电子邮件和应用程序内通知显示图像已附加到更新。

以前，在Workfront中共享图像的唯一方法是将其作为文档附加到对象。 在“更新”选项卡中添加的图像仅在该选项卡上可用，在“文档”选项卡上不可用。

有关详细信息，请参阅[更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

在Workfront用户可以在更新中包含图像之前，必须首先由Adobe Workfront管理员启用此功能，如[配置用户更新的首选项](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md)中所述。

## 更新了智能分配的算法

我们改进了进行智能分配时使用的算法。 根据新的改进，Workfront会查看登录用户最近进行的30个分配，以便在他们分配任务和问题时提供建议。 建议列表最多可包含50个用户。

在此增强功能之前，Workfront在建议用户时会考虑父级任务上的分配以及与这些分配相关的其他用户属性。

有关智能分配的信息，请参阅[智能分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md)。

## 从模板创建项目时的新体验

为了让您使用Workfront与新的Workfront体验保持一致，我们重新设计了用于从模板创建项目的界面。 使用模板创建项目的功能未发生更改。 但是，这个新重新设计的界面的一些改进包括：

* 在附加模板信息之前对其进行预览
* 在项目创建过程中将模板添加到收藏夹列表

当您从项目和模板区域创建项目时，我们更新了用于创建项目的界面。

有关信息，[使用模板](../../../manage-work/projects/create-projects/create-project-from-template.md)创建项目。

## 在将模板附加到项目时的新体验

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用。

为了让您使用Workfront与新的Workfront体验保持一致，我们重新设计了用于将模板附加到项目的界面。 用于附加模板的功能未发生更改。 但是，这个新重新设计的接口有一些改进，其中包括：

* 在附加模板信息之前对其进行预览
* 在附件过程中将模板添加到收藏夹列表
* 在一个连续的页面中查看用于管理模板和项目设置的所有选项

有关信息，请参阅[将模板附加到项目](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)。

## 任务的统一持续时间和持续时间单位值

为了提供更干净和更流畅的用户体验，我们已将Duration字段的值与duration时间单位合并。 在此增强功能之前，在“持续时间”字段后面的单独下拉字段中显示的时间单位。

除了“任务详细信息”、“编辑任务”和“新建任务”框中的“持续时间”字段外，我们还将更新以下字段以匹配此体验：

* 进行高级工作时的持续时间字段
* 创建或编辑任务时均衡延迟字段
* 创建周期性任务时的频率字段（即将推出）
* 添加前置任务时的“延迟”字段（即将推出）

有关信息，请参阅[编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。

![持续时间字段](assets/duration-combined-field-350x139.png)

## 禁止在项目中添加内联问题

为确保用户通过填写问题表单向项目添加问题时提供准确的信息，我们引入了一个新设置，该设置允许您管理用户是否可以将问题添加到项目或其内联任务。 默认情况下，在编辑项目框的新问题设置区域中启用此设置。 禁用此选项会变暗项目问题部分中的添加更多问题选项，因此用户无法在列表中添加更多问题。 用户仍可以使用“问题”部分中的“新问题”选项或请求队列（如果为项目配置了请求队列）将问题添加到项目中。

>[!NOTE]
>
>此设置仅在新的Workfront Experience中可用。 使用Workfront Classic的用户仍可以向项目或其任务添加内联问题，即使新Workfront Experience中的用户已为该项目禁用此设置。

有关详细信息，请参阅[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)。

## 复选框和单选按钮的自定义字段显示改进

查看和选择自定义表单中的复选框和单选按钮选项变得更加容易 — 现在，包含许多复选框或单选按钮选项的自定义字段会显示在页面的多个列中。 以前，它们只显示在一列中，这就要求用户在填写表单时进行额外的滚动。

这取决于在自定义表单中如何放置字段 — 如果将另一个字段与复选框或单选按钮字段放在同一行，则选项可能只有足够的水平空间来在一列中显示。

有关填写自定义表单的信息，请参阅[编辑自定义表单字段中的信息](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)。

