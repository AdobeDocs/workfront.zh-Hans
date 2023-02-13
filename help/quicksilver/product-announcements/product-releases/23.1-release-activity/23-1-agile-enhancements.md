---
title: 23.1灵活增强
description: 23.1灵活增强
author: Courtney
draft: Probably
feature: Product Announcements
exl-id: 4bd041a5-a6e3-4fe3-ae23-45980701e904
source-git-commit: f0e21f9b2846c5665474903a2910ce9f41cdf810
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# 23.1灵活增强

本页介绍了在“预览”环境中23.1版本所做的所有敏捷增强。 这些增强功能将于2023年1月16日这一周的生产环境中提供。

有关23.1版本中可用的所有更改的列表，请参阅 [23.1版本概述](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

## 为Workfront展示板进行规划

Adobe Workfront展示板中新增的Scrum规划功能提供了灵活的选项来管理您的灵活流程。 使用这些工具，您可以：

* 跟踪小版本或短划分中的工作
* 使用velocity指导团队承诺
* 跟踪燃耗和完成率

在23.1版本发布后，Scrum规划功能将是“快速跟进”的功能。

## 卡片上的到期日期映射到Workfront对象上的计划完成日期

>[!NOTE]
>
>此功能仅通过Workfront主板的早期功能选择加入来提供。

Workfront展示板中连接的信息卡的到期日期现在映射到关联的Workfront对象的计划完成日期。 如果您在信息卡上更新到期日期，则计划完成日期会在任务或问题上更新。 更改计划完成日期也会更改卡片上的到期日期。 以前，卡到期日期是手动输入的，且未映射到任务或问题的任何日期。

日期映射还适用于与子任务同步的连接的核对清单项目。

连接的卡和临时卡上的到期日期现在也包含一个时间字段。

有关更多信息，请参阅 [在主板上使用连接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[观看此功能的视频演示](https://video.tv.adobe.com/v/3411952/){target=_blank}

## 展示板核对清单项目和Workfront子任务现已关联

>[!NOTE]
>
>此功能仅通过Workfront主板的早期功能选择加入来提供。

将连接的信息卡添加到Workfront任务的展示板后，任何子任务都会作为核对清单项目导入该信息卡。 此外，在连接的卡上创建检查列表项时，子任务会添加到Workfront任务中。 与问题有关的核对清单项未与任何Workfront对象关联。

以前，核对清单项目和子任务未关联。 如果您希望在展示板上包含子任务，可以将其导入为单独连接的信息卡，或手动将核对清单项添加到信息卡。

有关更多信息，请参阅 [在主板上使用连接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) 和 [管理信息卡上的核对清单项目](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md).

[观看此功能的视频演示](https://video.tv.adobe.com/v/3411951/){target=_blank}

## 展示板列上的卡计数器

>[!NOTE]
>
>此功能仅通过Workfront主板的早期功能选择加入来提供。

可使用新的配置设置来打开展示板上所有列的卡片计数器。 如果对列使用WIP限制，则不会添加单独的卡片计数器。

有关更多信息，请参阅 [管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

## 在展示板仪表板上搜索和排序

>[!NOTE]
>
>此功能仅通过Workfront主板的早期功能选择加入来提供。

您现在可以按展示板名称或日期对展示板功能板进行排序，并在列表中搜索特定的展示板。

有关更多信息，请参阅 [使用展示板仪表板](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md).

## 状态显示在卡片上

>[!NOTE]
>
>此功能仅通过Workfront主板的早期功能选择加入来提供。

如果展示板上的信息卡被分配了状态，则状态现在会显示在信息卡上，这样您就不必打开信息卡即可查看状态。 此增强功能适用于临时卡和连接的卡。

有关更多信息，请参阅 [在主板上使用连接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) 和 [向展示板添加临时信息卡](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

![卡片状态](/help/quicksilver/product-announcements/product-releases/assets/boards-connected-card-details-110922.png)

## 可链接卡片现在可在展示板上使用

>[!NOTE]
>
>此功能仅通过Workfront主板的早期功能选择加入来提供。

您现在可以向其他展示板用户发送指向特定信息卡的链接。 用户必须有权查看展示板，然后才能打开链接。

在展示板上打开信息卡时，浏览器URL如下所示：

```
https://<Workfront-URL>/boards/<board-id>/card/<card-id>. 
```

您可以复制完整的URL并将其发送给其他人。 访问链接时，他们将直接转到打开的卡。

以前，链接可用于展示板，但不可用于特定信息卡。

有关信息卡的信息，请参阅 [向展示板添加临时信息卡](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) 和 [在主板上使用连接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## 在展示板上按连接过滤

>[!NOTE]
>
>此功能仅通过Workfront主板的早期功能选择加入来提供。

展示板上的过滤器列表现在包含按连接过滤的选项，该选项可显示特定项目的所有连接卡。 您还可以按未连接的卡进行过滤。

有关更多信息，请参阅 [在展示板中筛选和搜索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[观看此功能的视频演示](https://video.tv.adobe.com/v/3412381/){target=_blank}

## 按计划从展示板存档信息卡

>[!NOTE]
>
>此功能仅通过Workfront主板的早期功能选择加入来提供。

您可以配置展示板，以便按计划存档信息卡或“从展示板上流失”。 选项可用于设置特定列中的信息卡，以在特定天或周内进行存档。 例如，您可以定义衰减，以便“完成”列中的信息卡在列中处于两周后进行存档。

如果要在信息卡从展示板上掉下来后再次显示信息卡，可以设置展示板筛选器以显示已存档的信息卡。

有关更多信息，请参阅 [配置卡片衰减](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).

[观看此功能的视频演示](https://video.tv.adobe.com/v/3412323/){target=_blank}
