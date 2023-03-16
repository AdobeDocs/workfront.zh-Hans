---
title: 23.2灵活增强
description: 23.2灵活增强
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: 8a209bbe64b7b69b41cd9e4d2f603ff58491ba30
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# 23.2灵活增强

本页介绍在“预览”环境中23.2版本所做的所有灵活增强。 23.2版本的生产环境中将提供这些增强功能。

有关23.2发行周期中此刻可用的所有更改的列表，请参阅 [23.2版本概述](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

<!--

## Iteration functionality available in Adobe Workfront Boards

Several new features available in Workfront Boards make it possible to use agile Scrum functionality. These features include:

* Workstreams for grouping boards related to the same team, and collaborating on work
* A list of cards, or backlog of work, with the option to use sources to connect cards to Workfront tasks and issues
* Iteration planning and iteration process boards

Note that collections have been renamed to workstreams. Workstreams help you visualize data in different ways. You can display items on cards in a list, on a board, or on an iteration. Cards in a workstream can also be shared among multiple boards. You can easily facilitate workflows using cards and boards in a workstream.

For more information, see [Manage workstreams](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md), [Create an iteration](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md), and [Use the card list](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md). Second two articles will not be available in Main until I publish my branch.

## Add tasks and issues to Boards workstreams from lists and reports

You can now add existing tasks or issues to a workstream in Workfront Boards directly from a list or report view. Any items you add to the workstream are added to the card list as unplanned cards.

For more information, see [Add existing tasks or issues to a board](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).

-->

## 在主板上的连接卡上记录小时

>[!NOTE]
>
>此功能仅通过Workfront主板的早期功能选择加入来提供。

现在，您可以在连接的卡上登录数小时，这与在任务或问题上的登录方式相同。 您必须拥有正确的任务或问题权限才能记录时间。

默认情况下，时间日志记录字段不显示在连接的信息卡上。 必须启用 **小时** 在“Cards（卡片）”下的“Configure（配置）”区域。

有关更多信息，请参阅 [在主板上使用连接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## 自定义信息卡中字段的显示

>[!NOTE]
>
>此功能仅通过Workfront主板的早期功能选择加入来提供。


现在，可进行自定义，以配置在信息卡上显示的字段（在信息卡打开时的完整视图中）和展示板上的压缩信息卡视图中。 禁用字段时，这两个视图中都不显示字段。 您还可以在完整视图中启用字段，并在压缩视图中隐藏该字段。

有关更多信息，请参阅 [自定义信息卡上显示的字段](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

[观看此功能的视频演示](https://video.tv.adobe.com/v/3415710/){target=_blank}

## 为移入展示板列的信息卡定义默认状态

>[!NOTE]
>
>此功能仅通过Workfront主板的早期功能选择加入来提供。

您现在可以通过在列策略中选择自定义状态和系统状态，将默认状态设置为应用于移动到特定列中的卡。 将信息卡移入列时，Workfront会首先尝试应用自定义状态（例如，等待反馈）。 如果自定义状态不适用于该卡，则Workfront将应用系统状态（例如，暂挂）。 此外，如果连接任务或问题的状态更改为列策略中设置的自定义或系统状态，则卡会自动移至列。

以前，如果有多种状态可用，系统会提示您为移动到列中的每张信息卡选择一种状态。

有关更多信息，请参阅 [管理列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

[观看此功能的视频演示](https://video.tv.adobe.com/v/3415711/){target=_blank}

## 收藏集现在在Adobe Workfront展示板中可用

>[!NOTE]
>
>此功能仅通过Workfront主板的早期功能选择加入来提供。

您现在可以在展示板仪表板上创建收藏集。 收藏集是一组用于协作工作的委员会。 命名收藏集后，您可以使用一组提供预定义设置（如列名称）的模板将展示板添加到收藏集。 您还可以将独立展示板移入收藏集。 展示板进入某个收藏集后，即可将其移至其他收藏集，但不能成为独立的展示板。

向集合添加成员的工作方式与向展示板添加成员相同。 个人或团队必须是收藏集的成员，才能将其添加为收藏集的展示板中的成员。

有关更多信息，请参阅 [管理收藏集](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

[观看此功能的视频演示](https://video.tv.adobe.com/v/3415609/){target=_blank}

## 连接卡上的估计字段映射到Workfront对象上的“文章点”字段

>[!NOTE]
>
>此功能仅通过Workfront主板的早期功能选择加入来提供。

Workfront展示板中连接的信息卡上的“估计”字段现在映射到关联的Workfront对象的“文章点”字段。

新的“文章点”字段是一个可编辑的自由表单字段，您可以将该字段添加到列表或报表中的视图，以了解任务或问题。 它不与计划小时数或团队分配绑定。

以前，卡片估计是手动输入的，未映射到任务或问题上的任何字段。

此外，临时卡和连接卡上的“估计”字段不再具有字符限制。 以前，最大字符数为99。

有关更多信息，请参阅 [在主板上使用连接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## 进气列中的预览卡

>[!NOTE]
>
>此功能仅通过Workfront主板的早期功能选择加入来提供。

现在，您可以单击进入列中的连接卡，以查看其内容的仅查看版本。 在信息卡从进入列移出到展示板上的另一列之前，您无法编辑信息卡内容。
