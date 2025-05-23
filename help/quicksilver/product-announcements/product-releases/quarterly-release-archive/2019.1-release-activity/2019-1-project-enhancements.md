---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1项目增强功能
description: 本页介绍了2019.1版本中包含的所有项目增强功能。 该功能当前在“预览”环境中可用。 它将在的生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7b39082a-ab96-4e54-8f28-96629760715a
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 1%

---

# 2019.1项目增强功能

本页介绍了2019.1版本中包含的所有项目增强功能。 该功能当前在“预览”环境中可用。 它将在的生产环境中提供。

>[!IMPORTANT]
>
>此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2019.1版中所做所有更改的列表，请参阅“2019.1版活动概述”。

管理员的&#x200B;**&#x200B;**

* [从回收站还原模板](#restore-templates-from-the-recycle-bin)
* [显示主页中日期字段的时间戳](#show-timestamps-for-date-fields-in-home)
* [项目偏好设置下可用的所有持续时间类型](#all-duration-types-available-under-project-preferences)

所有用户&#x200B;**&#x200B;**

* [Agile改进](#agile-improvements)
* [将任务和问题从列表添加到迭代](#add-tasks-and-issues-from-a-list-to-an-iteration)
* [甘特图导出的新纸张大小](#new-paper-sizes-for-gantt-chart-export)
* [在编辑模式下删除了对甘特图对话框的访问权限](#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode)
* [在程序或Portfolio的项目列表甘特图中查看任务信息](#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio)
* [访问模板上的任务列表甘特图](#access-the-task-list-gantt-chart-on-templates)
* [重命名甘特图上的项目视图](#renamed-the-project-view-on-the-gantt-chart)
* [任务列表甘特图中的假设分析方案](#what-if-scenarios-in-the-task-list-gantt-chart)
* [任务列表改进](#task-list-improvements)
* [全屏显示列表](#display-lists-in-full-screen)
* [其他区域的新列表](#new-lists-in-additional-areas)
* [以XLSX格式发送传递的报告](#send-a-delivered-report-in-xlsx-format)
* [导出审核日志](#export-audit-logs)

## 从回收站恢复模板 {#restore-templates-from-the-recycle-bin}

Workfront管理员现在可以从回收站恢复模板。 与其他已删除的项目一样，您最多可以在删除模板后的30天内恢复该模板。

有关详细信息，请参阅“恢复已删除的项目”。

## 在主页中显示日期字段的时间戳 {#show-timestamps-for-date-fields-in-home}

作为Workfront管理员，您现在可以选择使用布局模板在工作列表和日历中显示或隐藏到期日期的时间戳。 默认情况下，时间戳对模板用户和非模板用户均可见。

有关更多信息，请参阅创建和管理布局模板一文中的“自定义主页区域”。

## 项目偏好设置下可用的所有持续时间类型 {#all-duration-types-available-under-project-preferences}

在设置>项目偏好设置中设置默认任务和问题持续时间类型时，您可以使用以下任一选项：

简单

投入比导向

计算的分配量

计算的工作量

以前，如果将“简单”或“投入比导向”设置为默认持续时间类型，则无法选择“计算的分配”和“计算的工时”。

有关设置任务和问题持续时间类型默认值的详细信息，请参阅“任务和问题首选项”

## Agile改进 {#agile-improvements}

Agile工具中现在提供了以下改进：

Kanban

从任何任务列表或报告将任务和问题添加到Kanban板。

以前，您只能从积压工作将任务添加到Kanban展示板。 无法添加问题。

按团队中的个人用户筛选Kanban展示板。

有关更多信息，请参阅使用Kanban板。

查看和管理Kanban积压中的问题。

有关更多信息，请参阅使用Kanban板。

以前，无法在Kanban展示板上添加或管理问题。

Scrum

按团队中的个人用户筛选迭代故事板。

有关更多信息，请参阅“使用Scrum敏捷故事板”。

以前，无法在Kanban或Scrum展示板上按用户筛选。

## 将任务和问题从列表添加到开发周期 {#add-tasks-and-issues-from-a-list-to-an-iteration}

您现在可以使用任务或问题列表、报告或仪表板将故事添加到开发周期。 还可在一个迭代中为多个团队分配故事。

以前，您只能从任务或问题详细信息页面将故事添加到开发周期，并且只能将故事添加到团队创建的开发周期。

有关更多信息，请参阅创建和管理Agile迭代。

## 以XLSX格式发送已传送的报表 {#send-a-delivered-report-in-xlsx-format}

除了当前的所有其他格式外，您现在还可以安排报表以MS Excel (.xlsx)格式传送。

以前，您只能通过以下格式提交报表：

HTML

PDF

MS Excel (.xls)

TSV

有关计划报表提交的信息，请参阅设置报表提交。

## 任务列表改进 {#task-list-improvements}

[更新已从]中删除的18.3 Beta 4

新重新设计的任务列表在18.3 Beta 4版本中短暂删除后已重新启用。 我们还向任务列表引入了以下附加功能，这些功能不在原始版本中：

内联编辑一项任务时，将右键单击菜单替换为更多图标。

现在，内联编辑多个任务时右键单击菜单中可用的选项已移至任务列表顶部显示的图标。

默认情况下，任务列表显示2000个任务。

当Workfront重新计算时间表时，日期正在更新的任务旁边的问号已替换为灰色区域。

有关编辑内联任务的信息，请参阅复制和复制任务以及通过链接任务创建前置任务关系。

有关重新计算项目时间线的信息，请参阅“重新计算项目的时间线”。

## 全屏显示列表 {#display-lists-in-full-screen}

当项目或任务列表大于屏幕大小时，该列表现在会在您滚动时自动显示在整个浏览器窗口中。 这会增加您一次查看的信息量，并使列表更易于管理。

您可以全屏显示以下列表：

以下选项卡和子选项卡中的项目列表：

我在处理的项目

我拥有的项目

所有项目

Portfolio中的“项目”选项卡

项目群中的“项目”选项卡

以下选项卡中的任务列表：

项目中的“任务”选项卡

任务中的“子任务”选项卡

有关在列表中显示对象的信息，请参阅查看列表中的项目。

## 其他区域的新列表 {#new-lists-in-additional-areas}

在以下方面，我们提高了性能并改善了项目和任务列表的外观：

“项目”区域中的“Portfolio”和“项目群”选项卡

任务级别的“子任务”选项卡

在此增强功能之前，新列表仅在以下区域可用：

“项目”区域中的“项目”选项卡

项目级别的“任务”选项卡

有关在列表中显示对象的信息，请参阅查看列表中的项目。

## 在项目列表甘特图中查看项目或Portfolio中的任务信息 {#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio}

您现在可以在项目列表甘特图中的项目或Portfolio中查看有关项目任务的信息。

以前，您只能在项目选项卡的项目列表甘特图中查看有关任务的信息。

有关详细信息，请参阅查看甘特图中的信息。

## 任务列表甘特图中的假设分析方案 {#what-if-scenarios-in-the-task-list-gantt-chart}

当项目中的任务以甘特图的编辑模式显示时，您现在可以对它们执行以下操作：

添加任务

删除任务

内联编辑任务

重复任务

重新排列任务

修改子任务

尽管您可以看到所做的更改对项目时间线的影响，但是它们不会立即保存。 您可以保存它们以永久更新项目时间线，也可以取消它们。

以前，您无法预览甘特图中的任务列表更改。

有关在甘特图中编辑任务的信息，请参阅“更新任务列表甘特图中的信息”。

## 访问模板上的任务列表甘特图 {#access-the-task-list-gantt-chart-on-templates}

您现在可以访问项目模板中的任务列表甘特图。

以前，您无法查看模板内任务列表上的甘特图。

有关详细信息，请参阅“甘特图快速入门”。

## 用于导出甘特图的新纸张大小 {#new-paper-sizes-for-gantt-chart-export}

您现在可以在A1和A2纸张大小上打印甘特图。

以前，您只能导出到Letter、Legal、Ledger、A3（仅适用于某些语言）和A4。

有关详细信息，请参阅将甘特图导出到PDF。

## 重命名了甘特图上的项目视图 {#renamed-the-project-view-on-the-gantt-chart}

我们将甘特图上的“项目”视图选项重命名为“适合所有”。 视图选项仍像以前一样工作。 新名称旨在让您在选择选项时，能更好地描述所查看的内容。

有关详细信息，请参阅查看甘特图中的信息。

## 在编辑模式下删除了对甘特图中对话框的访问权限 {#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode}

当甘特图处于编辑模式时，您无法再访问“高级分配”对话框。 在任务列表甘特图处于编辑模式时，只能进行内联编辑。

以前，您可以在甘特图处于编辑模式时访问“高级分配”对话框，但它保存了甘特图中所做的更改并关闭了编辑模式。

有关编辑任务列表甘特图的更多信息，请参阅“更新任务列表甘特图中的信息”。

## 导出审核日志 {#export-audit-logs}

您现在可以将审核日志条目导出到CSV文件。 一次最多可以将50,000个审核日志条目导出到CSV文件。

有关更多信息，请参阅管理审核日志。
