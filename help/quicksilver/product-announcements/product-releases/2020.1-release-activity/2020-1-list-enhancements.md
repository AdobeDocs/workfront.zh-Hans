---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1列表增强功能
description: 本页介绍了2020.1版本对Lists的所有增强功能。 这些增强功能目前在“预览”环境中提供，并将于2020年3月底或4月初在“生产”环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: efe05da7-ec25-4fbd-a7f9-645364d3e2a8
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 0%

---

# 2020.1列表增强功能

本页介绍了2020.1版本对Lists的所有增强功能。 这些增强功能目前在“预览”环境中提供，并将于2020年3月底或4月初在“生产”环境中提供。

有关2020.1版本可用的所有更改列表，请参阅[2020.1版本概述](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md)。

## 在任务列表中进行更改时的新保存模式：时间线计划模式

根据项目的大小和复杂性，更新任务列表（尤其是日期和持续时间）可能需要比预期更长的时间。 为了加快编辑速度，我们在名为“时间线计划”模式的列表中编辑任务时引入了一个新的保存选项。 在此模式之前，您可以使用自动保存自动保存保存保存对任务列表所做的更改，或者在禁用自动保存移动时手动保存所做的更改。

使用“时间线计划”模式将更改保存到任务列表时，请考虑以下优点：

* Workfront应用新视图，任务列表字段更少。 这可确保您能够专注于可能影响项目时间线的最重要的字段。
* 提交每个更改比使用自动或手动保存模式更快。
* 您可以在保存更改之前撤消更改。

有关将更改保存到任务列表的详细信息，请参阅[编辑列表中的任务](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)一文中的“使用时间线规划设置编辑任务”一节。

## 更新了新列表的外观

>[!NOTE]
>
>当这些功能最初发布到“预览”中时，它们可用于所有报告和列表，但“设置”和“报告”区域中的列表除外。 这些功能现在仅适用于项目、任务和小时列表。

项目、任务和小时列表现在具有更新的外观。

有关查看列表中的项的信息，请参阅[Adobe Workfront中的列表入门](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)。

其中一些更新包括：

* 用于快速查找列表中项目的快速筛选器
* 更干净的网格设计
* 更新了颜色和字体
* 列标题更易于阅读
* 内联编辑体验更易于阅读

## 改进了所有新列表的导航，具有明确的分组区分

现在，您可以更清楚地看到采用新配色方案的列表中若干层分组之间的区别。 在单独的框架中，还更清楚地概述了分组结果。 此更改已应用于所有新列表。

有关创建和自定义分组的信息，请参阅Adobe Workfront中的[分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。

## 使用快速筛选器时突出显示列表中的匹配项目

现在，在列表中查找项目速度更快：使用快速过滤器搜索项目时，匹配字段在结果中以黄色突出显示，以便您清楚地看到哪个字段值与您的关键字匹配。 在独立字段、共享列和复杂字段中，这些字段以黄色突出显示。 复杂字段的一些示例包括“分配”、“分配和状态”、“完成百分比”、“前置任务”、“审批者和状态”、“资源管理器”、“类别”、“条件”、“条件更新”等。

有关使用快速筛选器的信息，请参阅[Adobe Workfront中的列表入门](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)。

## 限制用户编辑列表和报告上的筛选器、视图和分组控件的能力

现在，您可以使用访问级别来限制用户编辑列表和报告上的筛选器、视图和分组控件的能力。 如果您希望自定义字段仅对特定访问级别的用户可见，则此功能非常有用。

有关详细信息，请参阅[授予对筛选器、视图和分组的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)。

## 在更新区域新增更多菜单

使用更新中的更多菜单可以：

* 复制更新的正文文本
* 将直接链接复制到更新线程或单个更新
* 删除更新

有关详细信息，请参阅[更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

## 更新区域的新进度条

更新区域中的完成百分比进度条具有新外观。 单击并拖动以更新百分比，或双击以手动输入数字。

有关详细信息，请参阅[更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

## 以句子大小写显示列表和报告的列标题

在以前的版本中，我们进行了一项更改，即在查看列表或报表时以所有大写字母显示所有列标题。 根据我们收到的反馈，我们现在将还原此更改。 经过此更改后，所有列标题现在均以句子大小写形式显示。

## 用于指示如何在列表中显示分组结果的新选项

>[!NOTE]
>
>此选项已从Workfront Classic预览环境中删除，不会包含在2020.1版本中。

为了让您更好地控制列表结果的显示方式，您现在可以指示在显示列表或报告时，是否默认展开或折叠分组中的结果。 此选项在列表或报表的分组生成器中可用。

默认情况下，结果显示在分组下的展开列表中。

在此更改之前，结果始终显示在折叠的列表中。

有关创建分组的信息，请参阅Adobe Workfront中的[分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。
