---
title: 23.2 Agile增强
description: 23.2 Agile增强
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: d9fa1c876f2b789c3c387387964ba749c5453a1e
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 0%

---

# 23.2 Agile增强

本页介绍了23.2版本对“预览”环境做出的所有Agile增强。 这些增强功能将在23.2版本的生产环境中提供。

有关23.2版本周期此时可用所有更改的列表，请参阅 [23.2发行版概述](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## 从列表和报告将任务和问题添加到Workfront讨论区

您现在可以直接从列表或报告视图将现有任务或问题添加到Workfront展示板。 您添加到展示板的任何项目都将成为连接的卡片。

此外，面板字段现在可用于添加到任务或问题的列表和报告。 此字段显示任务或问题已添加到的所有讨论区。

有关更多信息，请参阅 [将现有任务或问题添加到讨论区](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).

## 在展示板上记录已连接信息卡上的小时数

>[!NOTE]
>
>此功能只能通过Workfront展示板的早期功能选择加入来使用。

您现在可以在已连接的信息卡上记录小时数，就像在任务或问题上一样。 您必须对任务或问题具有正确的权限才能记录时间。

默认情况下，时间记录字段不会显示在连接的卡片上。 您必须启用 **小时** 在“信息卡”下的“配置”区域中。

有关更多信息，请参阅 [在展示板上使用连接的信息卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## 自定义信息卡上的字段显示

>[!NOTE]
>
>此功能只能通过Workfront展示板的早期功能选择加入来使用。


自定义功能现在可用于配置信息卡上显示的字段，包括信息卡打开时的完整视图以及展示板上的压缩信息卡视图。 禁用时，字段不会显示在任一视图中。 您还可以在全视图中启用某个字段并在压缩视图中隐藏该字段。

有关更多信息，请参阅 [自定义信息卡上显示的字段](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

[观看此功能的视频演示](https://video.tv.adobe.com/v/3415710/){target=_blank}

## 为移动到展示板列中的信息卡定义默认状态

>[!NOTE]
>
>此功能只能通过Workfront展示板的早期功能选择加入来使用。

现在，通过在列策略中选择自定义状态和系统状态，可设置默认状态以应用于移动到特定列的卡片。 将信息卡移动到列中时，Workfront会首先尝试应用自定义状态（例如，等待反馈）。 如果该信息卡的自定义状态不可用，Workfront将改为应用系统状态（例如，已搁置）。 此外，如果所连接任务或问题的状态更改为列策略中设置的自定义或系统状态，信息卡会自动移动到列。

以前，如果存在多个状态，系统会提示您为移动到列中的每张卡片选择一个状态。

有关更多信息，请参阅 [管理列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

[观看此功能的视频演示](https://video.tv.adobe.com/v/3415711/){target=_blank}

## 收藏集现在可在Adobe Workfront展示板中使用

>[!NOTE]
>
>此功能只能通过Workfront展示板的早期功能选择加入来使用。

您现在可以在展示板功能板上创建收藏集。 收藏集是一组用于协作完成工作的展示板。 为收藏集命名后，您可以使用一组提供预定义设置（如列名称）的模板将展示板添加到收藏集。 也可以将独立展示板移动到收藏集中。 展示板放入收藏集后，可以将其移动到其他收藏集，但不能成为独立展示板。

将成员添加到收藏集的工作方式与将成员添加到展示板的工作方式相同。 人员或团队必须是收藏集的成员，然后才能添加为收藏集中展示板的成员。

有关更多信息，请参阅 [管理收藏集](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

[观看此功能的视频演示](https://video.tv.adobe.com/v/3415609/){target=_blank}

## 已连接信息卡上的估计字段映射到Workfront对象上的故事点字段

>[!NOTE]
>
>此功能只能通过Workfront展示板的早期功能选择加入来使用。

Workfront展示板中已连接信息卡上的“估计”字段现在映射到关联Workfront对象的“故事点”字段。

新的“故事点”字段是可编辑的自由表单字段，可添加到列表或报告中任务或问题。 它与计划小时数或团队分配无关。

以前，信息卡估算是手动输入，未映射到任务或问题上的任何字段。

此外，临时信息卡和已连接信息卡上的“估计”字段不再有字符限制。 以前，最大字符数为99。

有关更多信息，请参阅 [在展示板上使用连接的信息卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## 在摄取列中预览卡片

>[!NOTE]
>
>此功能只能通过Workfront展示板的早期功能选择加入来使用。

现在，您可以单击引入列中的已连接信息卡，以查看其内容的仅查看版本。 在将信息卡从摄取列移动到展示板上的另一列之前，无法编辑信息卡内容。
