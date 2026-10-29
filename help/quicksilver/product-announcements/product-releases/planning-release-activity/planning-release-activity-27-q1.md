---
content-type: release-notes
title: Adobe Workfront Planning 2027年第一季度发布活动
description: 这是Adobe Workfront计划产品2027年第一季度的发布活动。
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 949503fecba92a7b8536b4af0b9c684e7f9e3300
workflow-type: tm+mt
source-wordcount: '1082'
ht-degree: 0%
---
# Adobe Workfront Planning 2027年第一季度发布活动

本文介绍了在2027年第一季度发行的Workfront Planning功能。

有关为Adobe Workfront Planning发布的所有功能的列表，请参阅[Adobe Workfront Planning发布活动：文章索引](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。

## 在表格视图中更好地显示快速搜索查找结果

>[!NOTE]
>
>预览： 2026年10月29日
>生产快速发布： 2026年11月12日
>适用于所有人的生产： 2027年1月21日

在表视图中使用快速搜索来查找项目时，该视图会删除与搜索不匹配的所有记录，并仅显示匹配的项目。

在此增强功能之前，将显示所有与搜索结果匹配的记录，并突出显示这些记录。

有关信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。

<!--

## Record-level permissions - restricted access to records

PLACEHOLDER: The release note field on the Workfront task points to an anchor story that no longer exists, so there is no description yet. Add the description and help link before unhiding.

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

-->

## 当跨工作区连接关闭时，允许在辅助工作区中连接连接的全局记录类型的记录

>[!NOTE]
>
>预览： 2026年10月29日
>生产快速发布： 2026年11月12日
>适用于所有人的生产： 2027年1月21日

在将两种连接的全局记录类型添加到辅助工作区时，您现在可以关闭跨工作区连接，并且仍然在本地链接记录。 每个辅助工作区只能看到其自己的两种记录类型的记录，并且可以将它们相互连接。 不再显示全局工作区和其他辅助工作区的记录。

在此增强功能之前，如果为连接的全局记录类型关闭了跨工作区连接，则辅助工作区无法将其自己的记录相互链接。 如果启用，则用户可以从全局工作区以及所有其他辅助工作区查看和链接记录。

有关详细信息，请参阅[跨工作区记录类型概述](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)。

## 查看表视图中的记录总数

>[!NOTE]
>
>预览： 2026年10月29日
>生产快速发布： 2026年11月12日
>适用于所有人的生产： 2027年1月21日

现在，表格视图会显示记录总数，并且会在您应用筛选器、搜索或更改视图时自动更新计数。 记录计数始终反映完全过滤的结果并尊重您的权限。

有关信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。

<!--

## Field aggregators available for groupings in the table view

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

Grouped records in the table views now show a summary row for each grouping, plus a grand total for the full table. Groupings and the grand total use the same summary functions, and nested groupings get their own summaries that include all child records. Aggregators update automatically as you filter, search, regroup, or edit records.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).

## Add sections to organize Planning views

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now create sections in the Workfront Planning View dropdown menu to organize related views as your list grows. You can name each section when you create it, then move views from My Views and Shared with Me into your custom sections. System views stay fixed in the System section.

For information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md).

-->

<!--

## Filters for Workfront objects connected record fields

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now filter for certain Workfront object types that meet a filter criteria when you add them as a connected field in Planning.

Only those Workfront objects that meet your filtering criteria will display as options in connected fields when editing a record.

For this feature, we added a new Record filtering rules option in the New connection tab when connecting the following Workfront object types: projects, portfolios, programs, groups, companies. Prior to this enhancement, filters were available only when connecting two record types.

For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

-->

## 查找字段数字限制

>[!NOTE]
>
>预览： 2026年10月29日
>生产快速发布： 2026年11月12日
>适用于所有人的生产： 2027年1月21日

我们将限制可以向记录类型添加的查找字段数：

* 每个记录类型最多40个查找字段
* 每个记录类型最多5个长文本查找字段。 连接的查找字段将计入其原始字段的限制中。
* 单个长文本查找单元格的值最多可包含50,000个字符。 如果查找值的组合内容超过此值，则会按连接顺序显示值，直到达到限制为止。 将忽略超出它的第一个值及其之后的所有值。 原始连接对象字段从未更改。

当您尝试创建或编辑前两个限制之外的查找字段时，会收到错误。 此更改不会影响已超过这些限制的记录类型。 您可以编辑它们，但在超出限制之前，您无法添加更多查找字段或值。

有关信息，请参阅[Adobe Workfront Planning对象限制概述](/help/quicksilver/planning/general/limitations-overview.md)。

## 新字段现在仅显示在您创建它们的视图中

>[!NOTE]
>
>预览： 2026年10月29日
>生产快速发布： 2026年11月12日
>适用于所有人的生产： 2027年1月21日

当您将新字段添加到记录类型时，它现在仅显示在您正在处理的视图中，并隐藏在所有其他现有视图中。 其他视图将按配置保留，如果需要，您可以在视图中取消隐藏新字段。

在此增强功能之前，新字段未隐藏地添加到每个视图中，有时会导致不熟悉新字段的用户混淆。

有关信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。

## 从任何视图导出记录详细信息

>[!NOTE]
>
>预览： 2026年10月29日
>生产快速发布： 2026年11月12日
>适用于所有人的生产： 2027年1月21日

您现在可以从任何详细信息视图中导出记录的详细信息，而无需切换到“所有字段”视图。

以前，导出选项仅在选择了“所有字段”视图时可用。

有关信息，请参阅[导出记录的详细信息](/help/quicksilver/planning/records/export-the-record-page.md)。

<!--

## Cancel and revert changes when editing records when business rules are violated

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

To ensure data integrity, when a business rule is violated while you edit a record, the change is blocked, the value reverts, and a toast notification explains why the edit is not allowed. The warning is visible in all areas where you are editing records, including the table view or details page.

If multiple rules are violated, each violation issues its own toast notification.

For more information, see [Configure business rules](/help/quicksilver/planning/architecture/configure-business-rules.md).

-->

## 通过在表和时间线视图中进行增量数据加载，提高了性能

<!-- NOTE FROM CSV: Must check with Lilit whether this will come to the timeline view in addition to the table (Lilit said yes; this was messaged before but pulled). The second bullet will change; check with Lilit first. -->

>[!NOTE]
>
>预览： 2026年10月29日
>生产快速发布： 2026年11月12日
>适用于所有人的生产： 2027年1月21日

为了提高大量记录的性能，我们对表和时间线视图进行了以下改进：

* 现在，该视图最初加载前500条记录，当您批量滚动500条时，会自动加载其他记录。
* 快速搜索和分组仅影响视图中当前加载的记录。

有关信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)和[管理时间线视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

<!--

## Additional permissions for users other than requestors to submitted requests

>[!NOTE]
>
>Preview: October 28, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

Workspace managers can now define what access to submitted requests users other than requestors have.

By editing the Permissions area of a request form, you can define additional access for other users to requests submitted using the form.

You can grant permissions to workspace users or any other users, groups, teams, job roles or companies in the system. Once defined in the request queue, the permissions are granted automatically when the request is submitted, and any permission changes apply only to new requests.

Prior to this enhancement, you could only grant permissions to requestors.

For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

-->

## 在时间线视图中手动重新排序分组

>[!NOTE]
>
>预览： 2026年10月29日
>生产快速发布： 2026年11月12日
>适用于所有人的生产： 2027年1月21日

您现在可以拖放分组、子分组和记录，以在时间轴视图中创建自定义顺序。 您的手动安排在各场会议中得以保留，并且随着规划需求的变化，您可以在手动订购与基于字段的排序之间无缝切换。

拖放功能适用于泳道和栈叠版本的时间线视图。

有关信息，请参阅[管理时间线视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

## 全局记录类型的业务规则

>[!NOTE]
>
>预览： 2026年10月28日
>生产快速发布： 2026年11月12日
>适用于所有人的生产： 2027年1月21日

Workspace管理员现在可以在主工作区和辅助工作区中针对全局记录类型配置业务规则。 规则适用于添加规则的所有工作区中的相同类型的所有记录。

在全局工作区中添加的业务规则在导入记录类型的辅助工作区中显示为只读。 在辅助工作区中添加的业务规则在最初创建记录类型的主工作区中显示为只读。 规则只能在创建它们的工作区中编辑。

有关信息，请参阅[配置记录类型业务规则](/help/quicksilver/planning/architecture/configure-business-rules.md)。

## 为Planning请求中的填写表单功能设置默认提示设置

>[!NOTE]
>
>预览： 2026年10月21日
>生产快速发布： 2026年11月12日
>适用于所有人的生产： 2027年1月21日

现在，您可以自定义用户在提交Planning请求时使用AI支持的填写表单功能时看到的提示。

在为Planning请求创建请求表单时，可以创建默认提示。

有关信息，请参阅[在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)。
