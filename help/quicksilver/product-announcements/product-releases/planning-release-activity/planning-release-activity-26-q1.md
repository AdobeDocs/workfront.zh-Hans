---
content-type: release-notes
title: Adobe Workfront Planning 2026年第一季度发布活动
description: 这是Adobe Workfront计划产品2026年第一季度的发布活动。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 34e6f4386c768b94c3835d4a4d7e7deadc3fecda
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 0%

---

# Adobe Workfront Planning 2026年第一季度发布活动

本文介绍了在2026年第一季度发行的Workfront Planning功能。

<!--keep the sentence below for all future quarterly release pages-->

有关为Adobe Workfront Planning发布的所有功能的列表，请参阅[Adobe Workfront Planning发布活动：文章索引](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。

## 在辅助工作区中删除了全局记录类型上的视图的公共共享


>[!NOTE]
>
>预览： 2025年12月3日
>生产快速发布： 2025年12月4日
>适用于所有人的生产： 2026年1月15日


在辅助工作区中共享全局记录的视图时，我们删除了“公共共享”选项卡。 不能通过从现有全局记录类型添加到另一个工作区的全局记录类型公开共享视图。 您可以从全局记录类型视图的原始工作区公开共享该视图。

有关信息，请参阅[共享视图](/help/quicksilver/planning/access/share-views.md)。


## 将GenStudio for Performance Marketing Brands与Workfront Planning记录类型联系起来

>[!NOTE]
>
>预览： 2025年11月13日
>生产快速发布： 2025年11月13日
>适用于所有人的生产： 2025年11月13日

您现在可以将Workfront Planning记录类型与Adobe GenStudio for Performance Marketing中的品牌联系起来。 您的组织必须同时具有Workfront Planning和Adobe GenStudio for Performance Marketing。

有关详细信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。


## Planning视图中的筛选器、字段和行颜色图标中的新字段搜索框

>[!NOTE]
>
>预览： 2025年11月6日
>生产快速发布： 2025年12月11日
>适用于所有人的生产： 2026年1月15日

在记录类型视图中构建视图元素时，您现在可以搜索特定字段。 当您构建过滤器、排序、分组或配置字段或行颜色时，我们添加了搜索框。 在此增强功能之前，您只需滚动浏览可用字段列表即可。

此改进适用于所有记录类型视图。

有关信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。


## 全局记录类型以及将它们作为现有记录类型添加到其他工作区的功能

>[!NOTE]
>
>预览： 2025年10月16日
>生产快速发布： 2025年11月13日
>适用于所有人的生产： 2026年1月15日

在使用通用工作流为多团队组织实施Workfront Planning时，您可能需要为关键记录类型（如营销活动或交付项）定义一个凝聚结构和元数据，这些记录类型可以添加到每个团队的工作区中以捕获和管理其工作。

此外，您可能需要每个团队的工作汇总到一个中心级别。

在此类工作流中，您可以确保团队以一致的方式捕获他们的工作，同时解锁跨团队的可见性，而无需将组织中的每个人添加到每个工作区。 您可以使用全局记录类型来实现这一点。

现在，您可以将记录类型指定为全局记录类型，并可在多个工作区中使用该记录类型。 用户可以使用已在中央工作区中配置的相同字段结构和连接。

有关更多信息，请参阅以下文章：

* [跨工作区记录类型概述](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

* [配置记录类型跨工作区功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)

* [从另一个工作区添加现有记录类型](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## 对一种记录类型的连接字段的新限制

>[!NOTE]
>
>预览： 2025年10月16日
>生产快速发布： 2025年11月13日
>适用于所有人的生产： 2026年1月15日

我们引入了每个记录类型30个连接字段的限制。

注意：如果贵组织当前有一个记录类型的连接字段超过30个，则可以保留超过30个限制的其他字段。 但是，不能向超过限制的记录类型添加更多连接字段。 今后，将强制执行30个连接字段的新限制。

有关详细信息，请参阅[连接的记录类型概述](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。

## 为选择类型字段选项设置用户友好型值

>[!NOTE]
>
>预览： 2025年10月16日
>生产快速发布： 2025年11月13日
>适用于所有人的生产： 2026年1月15日

向单选或多选字段添加字段选项时，Workfront现在将为每个选项分配唯一的用户友好型值。 在此改进之前，Workfront生成了一个字母数字ID，在API调用和其他集成中难以理解和使用。

进行此改进时请考虑以下事项：

* 新值将添加到新字段选项中。 现有字段选项将保留其字母数字ID。

* 一个字段的选项值是唯一的，但可以在不同字段之间重复。

* 重命名选项不会更新其原始值。

* 选择值以小写显示，在多词选择的情况下使用下划线分隔。 如果您使用已用作同一字段的另一个选择名称的标签，Workfront会向该值添加一个序列号。

有关信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。