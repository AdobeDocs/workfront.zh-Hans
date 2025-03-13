---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Adobe Workfront中的分组概述
description: 您可以添加分组来管理报告和列表中的信息布局。
author: Nolan
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
source-git-commit: 69dec186cdb8a6d29853703edb41073282cdd447
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# Adobe Workfront中的分组概述

<!-- Audited: 11/2024 -->

<!--(NOTE: This article was supposed to be replaced by "Groupings overview", but decided to keep this here because this is linked in too many places. "Create groupings" and "Edit existing groupings" have been added also (with videos) to replace portions of the old content here.)-->

您可以添加分组来管理报告和列表中的信息布局。

您可以通过以下方式将分组添加到报表：

* 您可以通过编辑现有分组来创建分组。

  有关自定义现有分组的信息，请参阅[编辑现有分组](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md)。

* 您可以从头开始创建分组。

  有关从头开始创建分组的信息，请参阅[在Adobe Workfront中创建分组](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)。

默认情况下，分组在报表或列表中以灰色高亮显示。 报告或列表的结果会列在其各个分组下，不会突出显示。

![分组示例](assets/grouping-example-blue.png)

您最多可以向一个报表中添加三个分组。 通过创建矩阵报告，您最多可以将信息分为四组。 有关矩阵报表的详细信息，请参阅[创建矩阵报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)。

分组名称后括号中的数字表示该分组下的结果数。 如果您的报表跨越多个页面，请确保在报表或列表中显示&#x200B;*全部*&#x200B;个结果，以便准确计算每个分组下的结果。

使用分组时，请考虑以下事项：

* 您可以自定义现有分组中的信息。 所有可以查看分组的用户也可以看到您所做的更改。
* 您的Workfront管理员必须授予您编辑筛选器、视图和分组的权限才能创建分组。

  有关授予对筛选器、视图和组的访问权限的信息，请参阅[授予对筛选器、视图和组的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)。

* 您对分组的权限级别决定了分组的保存方式。 如果最初创建分组，则可以保存更改，否则系统会提示您保存分组的版本。 如果您对与其他人共享的分组进行更改，则也会影响这些更改。
* 仅当与您共享的分组用户授予了您管理访问权限时，您才可以自定义与您共享的分组。 有关共享分组的信息，请参阅[共享筛选器、视图或分组](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md)。
* 无法编辑内联分组。
* 不能按多选自定义字段（例如，复选框）或可有多个值的字段（例如，资源管理器）进行分组。

## 有关分组的其他信息

在使用“分组”时，您可以进一步管理报表信息，方法是聚合“分组”行上每列中的值，以及按“分组”字段对信息进行排序。 您还可以在不再需要某个分组时将其删除。

* [分组中的聚合值](#aggregate-values-in-groupings)
* [按分组排序](#sort-by-a-grouping)
* [删除分组](#remove-a-grouping)

### 分组中的聚合值 {#aggregate-values-in-groupings}

您可以通过汇总报告每列中的值来汇总分组行中报告显示的数据。 有关汇总分组中列数据的更多信息，请参阅Adobe Workfront中的[视图概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。


>[!NOTE]
>
>在分组中聚合以下字段的值时，以下例外适用于父对象（例如，父任务）：
>
>* 除“实际小时数”之外的所有数字、货币和日期字段，仅聚合子任务和独立任务的值。 它们不会聚合父任务的值或父任务的父值。 在仅包含父任务的列表中对数字、货币和日期字段进行聚合时，不会在分组栏中显示聚合值。
>
>* 实际小时数聚合主父任务和独立任务的值；它们不会聚合子任务的数量或父任务的父任务的数量。<!--Examples of Actual hours include Planned/Actual Labor Cost, Planned/Actual Expense Cost, Planned/Actual Cost, and Planned Hours.-->
>
>* 数字和货币值的自定义数据字段汇总所有任务：父任务、子任务、父任务的父任务和独立任务。


### 按分组排序 {#sort-by-a-grouping}

无法对分组进行排序。 可对视图进行排序。 要按分组中捕获的值对列表进行排序，您必须在视图的某列中包含相同的值，并在视图中应用排序。 这样，列表间接地按分组中的值排序（它按视图中同样在分组中捕获的值排序）。 有关在视图内创建视图并按值排序的详细信息，请参阅Adobe Workfront中的[视图概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

### 删除分组 {#remove-a-grouping}

删除分组的方式取决于您最初是创建该分组，还是与您共享该分组。 不能删除默认分组。

* **如果您创建了分组并将其删除**，则该分组将从Workfront系统中删除。 该分组不再适用于您之前与其共享的任何用户。
* **如果分组已与您共享并且您将其删除**，则仅为您删除该分组。 最初创建该分组的用户及其共享的任何其他用户仍有权访问该分组。

有关删除分组的信息，请参阅文章[删除筛选器、视图和分组](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md)。


<!--Original note

The following exceptions apply for parent objects (for example, parent tasks) when you are aggregating values for the following fields in groupings:
All the number and currency fields except Actual Hours (for example, Planned/ Actual Labor Cost, Planned/ Actual Expense Cost, Planned/ Actual Cost, Planned Hours) aggregate only the values for the children tasks, and standalone tasks. They do not aggregate the values for the parent tasks or parents of parents.
Actual Hours aggregate the values for the main parent and the standalone tasks; they do not aggregate the numbers for the parents of parent tasks or the children tasks.
Custom data fields for number and currency values aggregate all tasks: parents, children, parents of parents, and standalone tasks.

-->