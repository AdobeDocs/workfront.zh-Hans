---
title: 2026年第三季度报告增强功能
description: 2026年第三季度报告增强功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: a177e2887c2b8b281b19cda45ce59c6f8149cefb
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# 2026年第三季度报告增强功能

本页介绍了在2026年第三季度版本中对“预览”环境所做的报表增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2026年第三季度发布周期中此时可用的所有更改列表，请参阅[2026年第三季度发布概述](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)。

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
