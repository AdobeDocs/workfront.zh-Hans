---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Adobe Workfront中的分组概述
description: 您可以添加分组以管理报表和列表中信息的布局。
author: Nolan
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# Adobe Workfront中的分组概述

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This article was supposed to be replaced by "Groupings overview", but decided to keep this here because this is linked in too many places. "Create groupings" and "Edit existing groupings" have been added also (with videos) to replace portions of the old content here.) </p>
-->

您可以添加分组以管理报表和列表中信息的布局。

您可以通过以下方式将分组添加到报表：

* 您可以通过编辑现有分组来创建分组。

   有关自定义现有分组的信息，请参阅 [编辑现有分组](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md).

* 您可以从头开始创建分组。

   有关从头开始创建分组的信息，请参阅 [在Adobe Workfront中创建分组](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

默认情况下，分组会在报表或列表中以灰色或蓝色突出显示显示。 报表或列表的结果列在其各个分组下，没有突出显示。

您最多可以在报表中添加三个分组。 通过创建矩阵报告，您最多可以按四个分组来组织信息。 有关矩阵报表的更多信息，请参阅 [创建矩阵报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

在标准分组报表中，第一个分组的颜色较深，第二个和第三个分组的颜色较浅。 不能为分组自定义高亮显示的颜色或分组名称的字体。 分组名称后的括号中的数字表示该分组下的结果数。 如果报表跨多个页面，请确保显示 *全部* 在报表或列表中生成结果，以便获取每个分组下的结果的准确计数。

![分组示例](assets/grouping-example-blue.png)

使用分组时请考虑以下事项：

* 您可以在现有分组中自定义信息。 所有能够查看分组的用户也可以查看您所做的更改。
* Workfront管理员必须授予您访问“编辑过滤器”、“视图”和“分组”的权限，才能创建分组。

   有关授予对“过滤器”、“视图”和“分组”的访问权限的信息，请参阅 [授予对过滤器、视图和分组的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* 您对分组的权限级别指示了如何保存分组。 如果最初创建了分组，则可以保存更改，否则系统会提示您保存分组的某个版本。 如果您对已与他人共享的分组进行了更改，则也会对分组产生影响。
* 仅当共享了该分组的用户授予您“管理”访问权限时，您才能自定义与您共享的分组。 有关共享分组的信息，请参阅 [共享过滤器、查看或分组](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* 不能编辑内联分组。
* 您不能按多选自定义字段（例如，复选框）或可以具有多个值的字段（例如，资源管理器）进行分组。

## 有关分组的其他信息

在使用分组时，您可以通过聚合分组行中每列的值来进一步管理报表信息，还可以按分组的字段对信息进行排序。 您还可以在不再需要分组时删除分组。

* [按分组汇总值](#aggregate-values-in-groupings)
* [按分组排序](#sort-by-a-grouping)
* [删除分组](#remove-a-grouping)

### 按分组汇总值 {#aggregate-values-in-groupings}

您可以通过汇总报表每列的值，将报表中显示的数据汇总到分组行中。 有关在分组中汇总列数据的更多信息，请参阅 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>在分组中聚合以下字段的值时，父对象（例如，父任务）会出现以下例外：
>
>* 除“实际工时”(例如“计划/实际人工成本”、“计划/实际费用成本”、“计划/实际成本”、“计划/实际工时”之外的所有“数字”和“币种”字段仅汇总子任务和独立任务的值。 它们不会聚合父任务或父代父代的值。
>* 实际小时数汇总主要父任务和独立任务的值；它们不会聚合父任务或子任务的父任务的数字。
>* 数字和货币值的自定义数据字段聚合所有任务：父母、子女、父母的父母和独立任务。


### 按分组排序 {#sort-by-a-grouping}

分组无法排序。 视图可以排序。 要按分组中捕获的值对列表进行排序，必须在视图的某一列中包含相同的值，并在视图中应用排序。 这样，列表就会间接按分组中的值排序（它会按视图中的值排序，视图中的值也会在分组中捕获）。 有关创建视图并按视图内的值排序的更多信息，请参阅 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### 删除分组 {#remove-a-grouping}

删除分组的方式取决于您最初是创建了分组，还是与您共享了分组。 不能删除默认分组。

* **如果创建了分组并将其删除**，则会从Workfront系统中删除分组。 您之前与之共享该分组的任何用户，都无法再使用该分组。
* **如果与您共享了分组，并且您将其删除**，则仅会为您删除分组。 最初创建该组的用户以及与其共享的任何其他用户仍有权访问组。

有关删除分组的信息，请参阅文章 [删除过滤器、视图和分组](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
