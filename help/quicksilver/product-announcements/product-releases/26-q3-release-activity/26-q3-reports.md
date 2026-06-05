---
title: 2026年第三季度报告增强功能
description: 2026年第三季度报告增强功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b9c63e1ca4b2b301ee104ee84151a2d0148a8cea
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# 2026年第三季度报告增强功能

本页介绍了在2026年第三季度版本中对“预览”环境所做的报表增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2026年第三季度发布周期中此时可用的所有更改列表，请参阅[2026年第三季度发布概述](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)。

## 对自定义公式中实际小时数的更改

>[!NOTE]
>
>预览： 2026年6月1日>生产快速发布： 2026年6月1日>适用于所有人的生产： 2026年6月1日

2025年，新的Actual Hours字段作为`actualWorkRequiredDouble`添加到Workfront数据库中，现有的Actual Hours字段（数据库中的`actualWorkRequired`）已重命名Legacy Actual Hours。 有关详细信息，请参阅[发行说明](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-project-enhancements.md)。

2026年6月，使用`actualWorkRequired`（旧版实际小时数）的现有自定义公式已迁移为使用`actualWorkRequiredDouble`（实际小时数）。 `actualWorkRequired`不能再用于计算和公式中。

此外，强烈建议在所有报表中使用`actualWorkRequiredDouble`。

替换字段时，请注意，`actualWorkRequired`以分钟为单位存储值，而`actualWorkRequiredDouble`以小数精度以小时为单位存储值。

有关实际小时数的详细信息，请参阅[查看实际小时数](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md)。

## 画布功能板报表中的自定义货币数据字段

>[!NOTE]
>
>预览： 2026年5月28日>生产快速发布： 2026年6月11日>适用于所有人的生产： 2026年7月16日

画布仪表板报表现在支持自定义货币数据字段，如列、筛选器、分组和聚合，包括在系统设置中配置多个汇率时。 当自定义货币数据字段显示为列或聚合时，除非该字段在报表级别被锁定，否则值将转换为在功能板的汇率切换中选择的货币。

以前在添加第二个汇率货币后失败并显示“受限字段”消息的报表现在会呈现。 定义了多个汇率时，计划货币字段仍受限制。

有关详细信息，请参阅[在画布功能板中使用货币字段](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md)。

## 提高了画布功能板报表中的数据准确性

>[!NOTE]
>
>预览： 2026年5月14日>生产快速发布： 2026年6月11日>适用于所有人的生产： 2026年7月16日
>
>Canvas功能板当前处于Beta版。

画布功能板现在可构建报表查询，以防止过滤器或字段交叉相关记录时显示重复行，这样计数、总和和其他聚合即可返回准确值。

以前，相关记录之间的连接可以为每个相关记录重复一次父记录。 例如，在筛选为分配给特定用户的任务的项目报告中，每个项目都会为每个匹配任务重复一次。 汇总项目预算的KPI可以显示6,000美元，而不是正确的1,250美元。

对画布功能板界面没有更改。 在此版本之后，现有报表会自动返回准确的数据。