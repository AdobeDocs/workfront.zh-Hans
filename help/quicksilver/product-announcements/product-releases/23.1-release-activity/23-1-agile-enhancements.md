---
title: 23.1 Agile增强功能
description: 23.1 Agile增强功能
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bd041a5-a6e3-4fe3-ae23-45980701e904
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

# 23.1 Agile增强功能

本页介绍了23.1版本对“预览”环境所做的所有Agile增强。 这些增强功能将在2023年1月16日这一周的“生产”环境中提供。

有关23.1版本的所有可用更改列表，请参阅[23.1版本概述](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md)。

## Workfront展示板的Scrum规划

Adobe Workfront展示板中的新Scrum规划功能提供了灵活的选项来管理您的敏捷流程。 使用这些工具，您可以：

* 跟踪迭代或冲刺中的工作
* 使用Velocity指导团队承诺
* 跟踪燃尽和完成率

Scrum规划功能在23.1版本之后将成为“快速跟进”。

## 卡片上的到期日期映射到Workfront对象上的计划完成日期

>[!NOTE]
>
>此功能只能通过Workfront展示板的早期功能选择加入来使用。

Workfront展示板中已连接信息卡的到期日期现在映射到关联Workfront对象上的计划完成日期。 如果您更新信息卡上的到期日期，则任务或问题上的计划完成日期将更新。 更改规划完成日期也会更改信息卡上的到期日期。 以前，信息卡到期日期是手动输入的，不会映射到任务或问题的任何日期。

日期映射也适用于同步到子任务的已连接清单项目。

现在，所连接信息卡和临时信息卡上的到期日期也包含时间字段。

有关详细信息，请参阅[在展示板上使用连接的卡片](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)。

[观看此功能的视频演示](https://video.tv.adobe.com/v/3411952/){target=_blank}

## 讨论区清单项目和Workfront子任务现在已链接

>[!NOTE]
>
>此功能只能通过Workfront展示板的早期功能选择加入来使用。

在为Workfront任务将连接的信息卡添加到展示板时，任何子任务都会作为信息卡上的清单项目导入。 此外，在连接的信息卡上创建清单项目时，子任务会添加到Workfront任务中。 问题的清单项目未连接到任何Workfront对象。

以前，清单项目和子任务未关联。 如果您想在展示板上包括子任务，则可以将其导入为单独的已连接信息卡，或手动将清单项目添加到信息卡。

有关详细信息，请参阅[在展示板上使用连接的展示卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)和[管理展示卡上的清单项目](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md)。

[观看此功能的视频演示](https://video.tv.adobe.com/v/3411951/){target=_blank}

## 板列上的卡计数器

>[!NOTE]
>
>此功能只能通过Workfront展示板的早期功能选择加入来使用。

新的配置设置可用于为展示板上的所有列打开卡片计数器。 如果对列使用WIP限制，则不会添加单独的卡计数器。

有关详细信息，请参阅[管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)。

## 在展示板仪表板中搜索和排序

>[!NOTE]
>
>此功能只能通过Workfront展示板的早期功能选择加入来使用。

您现在可以按展示板名称或日期对展示板仪表板进行排序，并在列表中搜索特定展示板。

有关详细信息，请参阅[使用讨论区功能板](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md)。

## 状态显示在信息卡上

>[!NOTE]
>
>此功能只能通过Workfront展示板的早期功能选择加入来使用。

如果展示板上的信息卡被分配了状态，则状态现在将显示在信息卡上，因此您不必打开信息卡即可查看状态。 此增强功能同时适用于ad hoc卡和连接的卡。

有关详细信息，请参阅[在展示板上使用连接的信息卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)和[向展示板添加临时信息卡](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md)。

信息卡上的![状态](/help/quicksilver/product-announcements/product-releases/assets/boards-connected-card-details-110922.png)

## 可链接卡现在可在展示板上使用

>[!NOTE]
>
>此功能只能通过Workfront展示板的早期功能选择加入来使用。

您现在可以将指向特定卡片的链接发送给其他展示板用户。 用户必须具有查看展示板的权限，然后才能打开链接。

当您在展示板上打开信息卡时，浏览器URL将如下所示：

```
https://<Workfront-URL>/boards/<board-id>/card/<card-id>. 
```

您可以复制完整的URL并将其发送给其他人。 访问链接时，用户将直接转到打开的卡。

以前，链接适用于展示板，但不适用于特定信息卡。

有关信息卡的信息，请参阅[向展示板添加临时信息卡](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md)和[在展示板上使用连接的信息卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)。

## 按展示板上的连接过滤

>[!NOTE]
>
>此功能只能通过Workfront展示板的早期功能选择加入来使用。

展示板上的过滤器列表现在包含按连接过滤的选项，该选项显示特定项目的所有连接信息卡。 您还可以按未连接的信息卡进行过滤。

有关详细信息，请参阅[在讨论区中筛选和搜索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md)。

[观看此功能的视频演示](https://video.tv.adobe.com/v/3412381/){target=_blank}

## 按计划存档展示板中的卡片

>[!NOTE]
>
>此功能只能通过Workfront展示板的早期功能选择加入来使用。

您可以配置展示板，以便按计划存档信息卡，或使信息卡“从展示板中流失”。 可使用以下选项：设置特定列中的卡片，以将其存档在特定天数或周数内。 例如，您可以定义流失，以便完成列中的信息卡在列中保留两周后进行存档。

如果您要在卡片从展示板跌落后再次显示卡，您可以将展示板过滤器设置为显示已存档的卡。

有关详细信息，请参阅[配置卡片减量](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md)。

[观看此功能的视频演示](https://video.tv.adobe.com/v/3412323/){target=_blank}
