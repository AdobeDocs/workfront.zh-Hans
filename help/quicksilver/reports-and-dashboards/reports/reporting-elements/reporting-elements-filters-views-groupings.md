---
product-area: reporting
navigation-topic: reporting-elements
title: '报告元素：筛选器、视图和分组'
description: Workfront中每个列表和报表都必须具有的主要元素包括过滤器、视图和分组。 每个元素可在任何报表中提供不同的信息。
author: Nolan
feature: Reports and Dashboards
exl-id: 5697905e-42c0-403b-85d4-798a1a3a2e7f
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# 报表元素：筛选器、视图和分组

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>AL: Add information here about all the different kinds of FVGs: in reports, in lists, beta, etc // OR: this article should be a high-level overview of reporting elements. Then, each type of element should have:</p>
<p>- overview for Filters</p>
<p>- create a filter</p>
<p>- share a filter</p>
<p>ALL in Reporting elements but the Shared ones should be linked to Basics> Sharing; some of the articles in the Basics> Navigation> Use lists might beed to link here as well</p>
</div>
-->

有多个元素让列表或报表在Adobe Workfront中成为可能。 每个列表和报表都必须具有的主要元素包括过滤器、视图和分组。 每个元素可在任何报表中提供不同的信息。

## 有关报表元素的注意事项

使用过滤器、视图和分组时，请考虑以下事项：

* 报表元素可用作报表的构建块。 它们定义报告或列表的外观，以及报告或列表中包含的信息。
* Workfront中的报表特定于一个对象。 在构建报告之前，必须为报告定义主对象。 因此，所有报告元素都是特定于对象的。
* 您的Workfront管理员必须授予您访问级别的筛选器、视图和分组的权限，才能在列表和报告中查看或编辑它们。

  有关授予对筛选器、视图和分组的访问权限的信息，请参阅 [授予对筛选器、视图和分组的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* 您的Workfront管理员必须授予您访问级别的报告、功能板和日历的访问权限，才能查看或编辑报告。

  有关授予对报表、功能板和日历的访问权限的信息，请参阅 [授予对报告、功能板和日历的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* 如果在报表或列表上选择一个筛选器、视图或分组，则即使您注销或关闭浏览器，Workfront也会为该对象的列表保留此选择。 例如，如果为任务报告选择特定视图，则该选择将出现在其他任务列表中，例如项目上的任务列表。

## 过滤器

过滤器可控制报表中显示的结果，通常将结果从常规缩小到特定。 它的工作方式就像一个筛子，只抓取您所需的信息，并将该信息带回您的报表。

例如，如果只想查看分配给登录用户的任务，可以创建标题为“我的任务”的过滤器，定义过滤器必须满足的条件，并运行报告以仅查看分配给登录用户的任务。

筛选器的某些属性包括：

* 默认情况下，Workfront为各种对象提供了大量过滤器。
* 您可以自定义自己拥有或管理的过滤器。

  有关筛选器的更多信息，请参阅文章 [过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

![过滤器图标](assets/projects-list-with-filter-drop-down-highlighted-nwe.png)

## 视图

通过定义报表视图，您可以定义在报表中包括哪些信息。 与所有报表元素一样，视图也基于一种对象类型。\
例如，任务报告的视图可显示到期日，包括关键财务详细信息（如成本），或用于显示分配和提交日期详细信息。 视图可用于提供有关报表中数据的各种详细信息。

视图的一些属性包括：

* 您可以使用默认的Workfront视图，也可以创建自己的视图。
* 运行报表后，您可以从“视图”下拉字段中应用其他视图。
* 其他视图会暂时替换创建报告时定义的视图；但是，下次返回报告时将显示默认视图。

  有关视图的详细信息，请参阅文章 [Adobe Workfront中的视图概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## 分组

分组可控制组织数据的方式，使其更易于阅读和理解。 分组可以在整个报表中创建水平条，这些水平条显示按公共属性一起列出的结果。 您可以定义在创建分组时如何对报告结果进行分组的标准。

例如，按项目名称对跨多个项目的任务列表进行分组，会将属于该名称下的单个项目的所有相应任务整理到该名称下。

分组的某些属性包括：

* 如果您稍后要向报表中添加图表，则分组是强制性的报表元素。
* 分组在结果中显示聚合值&#x200B;。
* 分组决定图表中的轴。
* 分组可确定矩阵报表中的标题标识。\
  有关矩阵报表的更多信息，请参阅文章 [创建矩阵报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

* 分组有助于构建报告的“摘要”选项卡，提供报告的汇总值。
* 默认情况下，Workfront为不同的对象提供了大量分组。
* 您可以自定义自己拥有或管理的分组。

  有关分组的详细信息，请参阅 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## 其他报表元素

除了筛选器、视图和分组之外，您还可以将以下元素添加到报表中：

* **提示**：打开过滤器，每次运行报表时，可以通过不同的方式对其进行自定义和应用。\
  有关提示的详细信息，请参阅文章 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* **图表**：您可以通过向报表添加图表并以可视方式显示信息来增强报表。\
  有关报表中图表的详细信息，请参阅文章 [向报表中添加图表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).
