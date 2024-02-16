---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1项目增强功能
description: 本页介绍了2020.1版本中对项目的所有增强。 这些增强功能目前在“预览”环境中提供，并将于2020年3月底或4月初在“生产”环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 13b6dd9e-52b9-4c5f-b727-bf32fbb94e8c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# 2020.1项目增强功能

本页介绍了2020.1版本中对项目的所有增强。 这些增强功能目前在“预览”环境中提供，并将于2020年3月底或4月初在“生产”环境中提供。

有关2020.1版本可用的所有更改列表，请参阅 [2020.1版概述](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## 更轻松地查看在更新中标记的人员

现在，查看哪些用户在更新中被标记更加容易。 已标记的用户名以蓝色显示，并链接到用户配置文件。

已标记的用户也会列在注释框下。

在此增强功能之前，之前标记的用户未出现在“通知”框中。

有关更多信息，请参阅 [为其他人标记更新](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## 在更新注释或回复中包括并标识引用文本

键入注释时，可以将注释的一部分标记为带引号的文本，以便将其与自己的注释区分开来。 使用HTML编辑器中的“块引用”按钮。

有关更多信息，请参阅 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


## 在更新评论或回复中引用以前的评论

在更新跟帖中注释时，可以快速将先前注释中的文本包含到跟帖中。 在要报价的备注旁边的“更多”菜单中查找“报价回复”选项。

有关更多信息，请参阅 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## 其他风险信息

为了帮助您更好地了解项目的风险，您现在可以看到在项目上输入了风险的人和时间以及更新风险的时间。 您可以在风险视图中通过公共Workfront API访问此信息。 这些字段将在API版本11中可用，该版本随2020.1生产版一起发布。

有关Workfront中的风险的信息，请参阅 [创建和编辑项目风险](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

## 添加到基线和基线任务的其他字段

为了帮助您更好地了解项目的财务进度，您现在可以在基准或基准任务报告中包括额外的成本和收入信息。 附加的财务信息不会添加到当前保存的基线中，而是会为新的基线而添加。

有关可从基线和基线任务对象访问的项目和任务财务字段的信息，请参阅 [项目基线中包含的项目财务](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## 处于“已关闭 — 未决批准”状态的问题被视为未完成

Workfront处理“完成 — 未决批准”状态问题的方式已更改。 现在，这些问题会被视为未解决，在解决审批之前，无法将项目标记为完成。

在此更改之前，处于“已关闭 — 未决批准”状态的问题被视为已关闭。

在此更改之前所有处于“已关闭 — 未决批准”状态的问题都将与之前的行为相同，即视为已完成，同时允许项目完成。 进行此更改后处于此状态的所有问题都将被视为未完成。

有关项目状态的信息，请参阅 [访问系统项目状态的列表](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).

