---
product-area: reporting
navigation-topic: text-mode-reporting
title: 文本模式的常见用途概述
description: 文本模式的常见用途概述
author: Nolan
feature: Reports and Dashboards
exl-id: 81512837-1ec4-4dbc-ace4-bdf08fe667ce
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 0%

---

# 文本模式的常见用途概述

<!-- Audited: 1/2025 -->

<!--(NOTE: Alina: ***This is linked to Understanding Text Mode (article), and the TOC article for examples of various reporting elements)</p>-->

您可以使用报表和报表元素中的文本模式来扩展报表功能。 您还可以使用某个版本的文本模式来构建更复杂的计算自定义字段。 有关文本模式的详细信息，请参阅[文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

本文仅概述几个常见示例，您最可能需要在其中使用文本模式来扩展Adobe Workfront中的报表或计算自定义字段功能。 有关更全面的示例列表，请参阅：

* [自定义视图、筛选器和分组示例：文章索引](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
* [报表中计算的自定义数据](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md)

有关使用文本模式创建报告（包括类、视频和教程）的更多信息，请参阅Adobe Experience League网站上的“学习”部分。

## 可以在列表和报告中使用文本模式的实例

我们建议您使用报表和列表生成器来构建视图、筛选器和分组。 但是，在某些情况下，您可以使用文本模式来增强报告和列表。

当您希望在Workfront中实现以下目标时，可以使用文本模式：

* 在自定义表单中构建自定义计算自定义字段。\
  有关计算自定义字段的更多信息，请参阅本文中的[在计算自定义字段中使用文本模式](#use-text-mode-in-calculated-custom-fields)部分。
* 在Report Builder中可提供的范围之外增强筛选器、视图和分组。 有关对筛选器、视图和分组使用文本模式的信息，请参阅本文中的以下部分：

   * [在视图中使用文本模式](#use-text-mode-in-views)
   * [在筛选器中使用文本模式](#use-text-mode-in-filters)
   * [在分组中使用文本模式](#use-text-mode-in-groupings)

* 创建自定义提示。 您只能使用文本模式创建自定义提示。

  有关生成自定义提示的信息，请参阅[向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)。

## 在计算自定义字段中使用文本模式 {#use-text-mode-in-calculated-custom-fields}

您可以使用文本模式将计算的自定义字段添加到自定义表单。

有关将计算自定义字段添加到自定义表单的详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

有关在文本模式下创建计算自定义字段的详细信息，请参阅[将计算字段添加到表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。

例如，您可以添加计算自定义字段，以显示项目被标记为“进行中”时的时间和日期戳。 您可以将此计算用于其他状态。

有关信息，请参阅[计算自定义字段示例：在自定义表单中显示状态时间戳](../../../reports-and-dashboards/reports/calc-cstm-data-reports/example-status-timestamp-in-calculated-field.md)。

## 在视图中使用文本模式 {#use-text-mode-in-views}

您可以使用视图中的文本模式来展开可在视图中显示的字段和对象。

有关在视图中使用文本模式的最常见原因的示例，请参阅以下文章：

* [视图：显示未包含在标准界面中的对象](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-objects-not-in-standard-interface.md)
* [视图：显示列](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculation-between-two-fields.md)中两个字段之间的计算结果
* [视图：永久编辑列的宽度](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md)
* [视图：合并来自一个共享列中多个列的信息](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)
* [视图：删除列](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-remove-link-to-object.md)中对象的链接
* [引用报告中的收藏集](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)
* [视图：隐藏列](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-hide-column-content.md)的内容
* [视图：在列](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-image-in-view.md)中显示图像而不是字符串
* [视图：在任务列表中显示任务缩进](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-task-identations.md)
* [查看：计算时间和日期差异](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculate-time-and-date-differences.md)

## 在筛选器中使用文本模式 {#use-text-mode-in-filters}

构建过滤器时，您可以使用文本模式来展开可过滤的字段和对象。

有关在过滤器中使用文本模式的最常见原因的示例，请参阅以下文章：

* [筛选器：创建引用同一字段（“AND”语句）的多个筛选器规则](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-refrence-the-same-field-multiple-times.md)
* [筛选器：仅显示处于批准状态的项目](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-for-items-in-approval-status.md)
* [筛选器：当状态与不同的组相关联时，按同名状态显示项目](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-same-name-statuses-from-different-groups.md)
* [筛选器：通过比较两个字段](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-items-by-comparing-two-fields.md)来消除列表中的项
* [使用EXISTS语句创建复杂文本模式筛选器](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)文章中的部分[跨对象层次结构中多个级别的文本模式筛选器示例](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#examples)
* [&#128279;](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#missing-object-filters)部分[使用EXISTS语句创建复杂文本模式筛选器](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)中的缺失对象创建复杂文本模式筛选器

## 在分组中使用文本模式 {#use-text-mode-in-groupings}

在构建分组时，可以使用文本模式展开可在列表和报告中作为分组依据的字段和对象。

有关在分组中使用文本模式的最常见原因的示例，请参阅以下文章：

* [分组：按分组中所有对象通用的计算值组织列表结果](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-by-calculated-common-values.md)
* [分组：向列表添加第四个分组](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-add-fourth-grouping.md)
* [分组：编辑分组中的显示名称](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-rename-grouping.md)
* [分组：指示应使用文本模式折叠或展开分组的结果](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-collapsed-or-expanded-results.md)
