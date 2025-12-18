---
title: 2026年第一季度报告增强功能
description: 2026年第一季度报告增强功能
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: bed931281d7d0b3184914ed7649d9cb889bcf39a
workflow-type: tm+mt
source-wordcount: '871'
ht-degree: 0%

---

# 2026年第一季度报告增强功能

本页介绍了在2026年第一季度发布中对“预览”环境所做的报表增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2026年第一季度发布周期中此时可用的所有更改列表，请参阅[ 2026年第一季度发布概述](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md)。

<!--

## Currency updates in Canvas Dashboards

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast release: January 14, 2026 
>Production for everyone: January 15, 2026 

We have made the following updates for currency fields:

* When multiple currencies are defined in Workfront, you can now choose a default currency for the dashboard during creation. 

* When creating a report, you can lock a currency field. This ensures that the dashboard-level currency preference does not affect the display of these values.

* When viewing a dashboard, users can toggle between any defined currencies in Workfront. These changes apply to the entire dashboard with the exception of locked currency fields.

-->

<!--

## Quick search table results in Canvas Dashboards

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast release: January 14, 2026 
>Production for everyone: January 15, 2026 

We have added a quick search to Table reports. This search works across all pages, so you can find data even if it's not currently visible.

-->

## 饼图的新显示总计选项

>[!NOTE]
>
>预览： 2025年12月18日
>生产快速发布： 2026年1月14日
>适用于所有人的生产： 2026年1月15日

我们引入了一个新的“显示总计”选项，该选项可将饼图转换为圆环图。 此功能允许用户显示一个中心值，代表图表中所有区段的总数。

* 对于计数聚合类型，显示的中心值是图表所有区段的计数。
* 对于总和聚合类型，显示的中心值是数值或货币值的聚合总计。
* 对于average、max和min聚合类型，中心值将相应地显示平均值、最大值或最小值。

用户还可以选择显示或隐藏总计的标签，并提供自定义标签值。

有关详细信息，请参阅[在画布仪表板中生成图表报告](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md)。

## 画布仪表板中饼图的新配置选项

>[!NOTE]
>
>预览： 2025年12月18日
>生产快速发布： 2026年1月14日
>适用于所有人的生产： 2026年1月15日

我们为饼图引入了两个新的配置选项：

* 隐藏区段标签：现在，您可以选择在饼图上隐藏区段标签（如果区段标签太长并影响图表可读性）。
* 隐藏和重新定位图表图例：您现在可以选择隐藏饼图图例。 您还可以将图例的位置设置为图表的右侧（默认）、左侧、顶部或底部。

有关详细信息，请参阅[在画布仪表板中生成图表报告](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md)。

## 画布功能板分组计数改进

>[!NOTE]
>
>预览： 2025年12月18日
>生产快速发布： 2026年1月14日
>适用于所有人的生产： 2026年1月15日

我们更新了画布仪表板中的分组栏，以显示当前页面的记录计数以及跨所有页面的分组的整体记录计数。

例如，分组栏将显示“第3个（共7个）”或“第83个(共21032个)”，以清楚地了解分组中的数据分布。

以前，分组栏不提供此详细的计数信息，这使得在导航多个页面时了解分组中的记录总数变得困难。

## Canvas功能板中的报告新增了参考线功能

>[!NOTE]
>
>预览： 2025年12月18日
>生产快速发布： 2026年1月14日
>适用于所有人的生产： 2026年1月15日

现在，您可以在条形图、柱形图和折线图中定义参考线，以设置基于系列报表的目标或阈值。

注意：参照线不是动态的，不能应用多条参照线。 我们正在探索未来的增强功能，但目前还没有制定任何计划。

有关详细信息，请参阅[在画布仪表板中生成图表报告](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md)。

## 自定义画布仪表板中图表报表的轴标签

>[!NOTE]
>
>预览： 2025年12月18日
>生产快速发布： 2026年1月14日
>适用于所有人的生产： 2026年1月15日

您现在可以自定义图表报表上的轴标签。 此新功能允许您输入要显示的替换轴标签，而不是默认对象和字段路径。 此外，您可以选择完全隐藏轴标签。

有关详细信息，请参阅[在画布仪表板中生成图表报告](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md)。

## 在画布功能板中复制报告

>[!NOTE]
>
>预览版本： 2025年10月23日
>适用于所有客户的生产： 2025年10月23日
>[!BADGE 超出计划]{type=Neutral}

现在，您可以在创建KPI、表或图表报表后，将其复制到画布仪表板中。 复制后，您可以在保存之前根据需要编辑报表。

## 从报告筛选器中删除字段选项

>[!NOTE]
>
>预览： 2025年11月6日
>生产快速发布： 2025年11月13日
>适用于所有人的生产： 2026年1月15日

我们删除了以下之前在将过滤器应用于报表时可用的字段选项：

* 其他组ID
* 其他角色ID
* 其他团队ID

由于与“不等于”和“为空”运算符相关的问题，已删除这些参数。 如果您现有的过滤器使用其中一个字段，则该过滤器将继续按预期工作。 或者，您可以在<code>文本模式下继续使用这些字段</code>，但建议在这样做时避免使用“不等于”或“为空”运算符。

以下字段选项可用作替代项：

* 其他组： ID
* 其他角色： ID
* 其他团队： ID

## 改进了画布功能板中分组计数的显示

>[!NOTE]
>
>预览： 2025年11月6日
>生产快速发布： 2025年11月13日
>适用于所有人的生产： 2026年1月15日

当表报告有多个结果页并且表配置了分组时，该表现在显示当前页的记录数量和所有页的总记录计数。 例如，如果表报表分为7个分组，且第一页显示为3个，则表将显示第3页（共7页）。


## 新护栏可缩短Canvas仪表板中的加载时间

>[!NOTE]
>
>预览： 2025年11月6日
>生产快速发布： 2025年11月13日
>适用于所有人的生产： 2026年1月15日

为了避免加载时间延迟并提高画布仪表板中的整体性能，我们对可以向仪表板添加多少仪表板组件施加了限制：

* 每个仪表板的报表数：25个限制
* 表视图上的分组：5个限制
* 与报表的基本对象的距离：10限制
* 表格视图中的列：25个限制
* 仪表板级别筛选器提示： 10次限制




