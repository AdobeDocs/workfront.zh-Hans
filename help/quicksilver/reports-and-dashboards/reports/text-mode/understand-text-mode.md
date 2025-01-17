---
product-area: reporting
navigation-topic: text-mode-reporting
title: 文本模式概述
description: 在创建构成报告或列表的元素时，可以使用标准或文本模式界面在Adobe Workfront中构建报告或列表。
author: Nolan
feature: Reports and Dashboards
exl-id: 8be8cbd0-da1b-4e90-a52e-dc352f646d18
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# 文本模式概述

<!-- Audited: 1/2025 -->

<!--(NOTE: Linked to the UI (for the areas mentioned in the comments below and the new NWE filters as well))-->

<!--(NOTE: Alina: ***Linked to other articles. Do not move, rename or change url.Linked to the product, in the report builder, when using a field that is not recognized in standard mode.)-->

<!--(NOTE: This will be linked to the Ninja feature about adding a filter to the User typeahead field (which originally is open only for text mode filters). Update the Context Sensitive sheet at release time)-->

在创建构成报告或列表的元素时，可以使用标准或文本模式界面在Adobe Workfront中构建报告或列表。

标准界面允许您引用Workfront界面中随时可用的字段及其属性。

使用文本模式，您可以引用在标准模式下可能不可用，但在Workfront数据库中可用的字段和属性。

有关使用文本模式创建报告（包括类、视频和教程）的更多信息，请参阅Adobe Experience League网站上的“学习”部分。

## 使用文本模式之前的注意事项

>[!TIP]
>
>您还可以通过使用自定义字段的文本模式版本来扩展计算自定义字段的功能。 用于创建计算自定义字段的语法和规则与您在报表和列表中使用的语法和规则不同。 有关添加计算自定义字段的信息，请参阅[将计算字段添加到表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。

* 在报表中开始使用文本模式之前，我们强烈建议您先参加有关高级报表的课程，以便更深入地了解我们的文本模式语言。
* 我们建议您使用标准模式，以确保在Workfront软件更新时您创建的报表保持不变。 虽然文本模式使您能够创建更复杂的视图、筛选器和分组，但维护起来也更加复杂，并且在Workfront软件更新时无法保证这一点。
* 我们建议您始终尝试在标准界面中构建所有报表元素，并仅在进行少量调整时切换到文本模式生成器。

  >[!TIP]
  >
  >使用标准生成器会为您提供重要的构建块和代码模式，您可以在文本模式下修改代码时使用这些构建块和模式。

* 要以文本模式成功构建报表和列表，您必须使用一组规则和唯一语法。 在开始之前，请确保您熟悉文本模式的Workfront语法。

  有关使用文本模式的语法和规则的信息，请参阅[文本模式语法概述](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)。

* 在文本模式下自定义报表元素后，可能无法切换回标准模式（在视图中），或者您创建的元素的代码可能会被删除（在筛选器和分组中）。 这是因为标准模式并非支持文本模式中支持的所有字段。

## 标准模式界面

标准模式界面显示字段，以映射要在报表或列表中显示的应用程序元素。 标准模式界面是一组下拉菜单，您可以从中选择要在报告或列表中显示的字段。

有关标准模式界面的详细信息以及了解如何创建报告或列表，请参阅：

* [创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
* [报表元素：筛选器、视图和分组](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)

## 文本模式界面

文本模式允许您使用标准模式界面中不可用的字段，从而创建更复杂的视图、筛选器、分组和提示。 在Workfront文本模式下，是编码语句的集合，用于指示您希望在报表或列表中显示的对象。

有关所有可报告字段的完整列表，请参阅[API资源管理器](../../../wf-api/general/api-explorer.md)。

>[!NOTE]
>
>并非所有通过API可用的字段都可通过文本模式界面使用。 如果您在文本模式代码中使用了正确的字段，并且没有显示预期的结果，则该字段可能只能通过API报告。

## 访问报表元素并编辑文本模式 {#access-reporting-elements-and-edit-text-mode}

从报表或列表访问视图、分组和筛选器时，访问文本模式界面的方式与此类似。

有关在视图、筛选器和分组中使用文本模式的信息，请参阅：

* [使用文本模式编辑视图](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
* [使用文本模式编辑筛选器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
* [使用文本模式编辑分组](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

自定义提示只能在文本模式下编辑。 您只能从报表访问提示。

有关访问自定义提示的文本模式界面的信息，请参阅[向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)。

## 使用文本模式的常见原因 {#common-reasons-to-use-text-mode}

除了创建只能使用文本模式配置的自定义提示之外，我们建议您使用Report Builder构建视图、筛选器和分组。 但是，在某些情况下，您可以使用文本模式来增强报告和列表。

有关文本模式的常见用法的详细信息，请参阅[文本模式的常见用法概述](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)。
