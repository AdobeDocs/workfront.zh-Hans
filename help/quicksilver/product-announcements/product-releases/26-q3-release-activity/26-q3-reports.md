---
title: 2026年第三季度报告增强功能
description: 2026年第三季度报告增强功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: f465ac03e0ff91216d1ef934a1696127796645ba
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---

# 2026年第三季度报告增强功能

本页介绍了在2026年第三季度版本中对“预览”环境所做的报表增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2026年第三季度发布周期中此时可用的所有更改列表，请参阅[2026年第三季度发布概述](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)。

## 画布功能板提示默认值和用户首选项持久性

>[!NOTE]
>
>预览： 2026年6月25日>生产快速发布： 2026年7月15日>适用于所有人的生产： 2026年7月16日

为了通过保留用户的工作筛选器状态来提高用户在功能板和记录之间移动的效率，功能板管理员现在可以为Canvas功能板定义默认提示值。 这些默认值将自动应用于所有仪表板查看器。

当用户更新提示时，他们的选择会在刷新、重新打开或导航到记录并返回后保存和恢复。

管理员可随时重置仪表板的默认状态。 用户还可以通过三个圆点菜单快速恢复到默认值。

在此增强功能之前，仪表板提示不具有提示状态的可配置默认设置或已保存的用户偏好设置。

有关信息，请参阅[筛选画布功能板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/filter-canvas-dashboard.md)。

## 一次性将多个Power BI IP地址范围添加到Data Connect

>[!NOTE]
>
>预览：不适用>生产快速发布： 2026年6月11日>适用于所有人的生产： 2026年7月16日

Workfront管理员将Microsoft Power BI连接到Workfront Data Connect后，现在只需一步即可将整个区域的Azure IP地址范围集添加到。 在&#x200B;**Data Connect**&#x200B;中的&#x200B;**IP**&#x200B;选项卡上，**新IP地址**&#x200B;按钮现在包含一个&#x200B;**添加Power BI IP地址块**&#x200B;选项，该选项将打开一个对话框，您可以通过该对话框粘贴Microsoft发布的Power BI IP范围和服务标签JSON文件中的Azure服务标签条目。

这取代了之前每次添加一个Power BI CIDR块的工作流程，对于发布大量地址前缀的区域而言，此工作流非常耗时。

有关详细信息，请参阅[建立与Workfront Data Connect的连接](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)。


## 对画布功能板列表进行排序

>[!NOTE]
>
>预览： 2026年6月11日>生产快速发布： 2026年7月15日>适用于所有人的生产： 2026年7月16日
>
>Canvas功能板当前处于Beta版。

您现在可以按以下任意列对画布功能板列表进行排序：**名称**、**描述**、**创建者**&#x200B;或&#x200B;**创建日期**。 单击列标题可按该列对列表进行排序，然后再次单击同一标题可反转排序方向。 默认情况下，该列表按&#x200B;**名称**&#x200B;从A到Z排序。在“画布功能板”列表中的选项卡之间切换时，将保留您的排序顺序。

有关详细信息，请参阅[使用画布功能板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md)。

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

