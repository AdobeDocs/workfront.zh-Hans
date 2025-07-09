---
content-type: release-notes
title: Adobe Workfront Planning 2025年第三季度发布活动
description: 这是Adobe Workfront计划产品2025年第三季度的发布活动。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 6761f5af-2501-4487-8114-2751f1e4fe69
source-git-commit: eaba54ebfef15c5f823c7086b809165b5cfb181b
workflow-type: tm+mt
source-wordcount: '1908'
ht-degree: 0%

---

# Adobe Workfront Planning 2025年第三季度发布活动

本文介绍了在2025年第三季度版本中为Workfront计划发布的功能。

<!--keep the sentence below for all future quarterly release pages-->

有关为Adobe Workfront Planning发布的所有功能的列表，请参阅[Adobe Workfront Planning发布活动：文章索引](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。

<!--## Auto-populate fields based on applied groupings

Preview: July 10, 2025 
Production fast release: August 14, 2025 
Production for everyone: October 16, 2025 

Now, when you have  groupings applied to a table view, adding a record to the table will auto-populate the fields associated with the groupings you add the record to.  

If you have multiple groupings applied, the system auto-populates the fields associated with all groupings only when you add the record at the end of the list inside the last grouping criteria.  

Prior to this enhancement, you had to manually update the fields associated with groupings.  

For information, see [Create records](/help/quicksilver/planning/records/create-records.md).-->

<!--## Common sharing button for views and record types

>[!NOTE]
>
>* Preview: July 9, 2025 
>* Production for everyone: July 17, 2025 

You can now share a view as well as a record type from the same button on the record type's page. Prior to this enhancement, you could only share the record type from the Share button on the record type page and a view from the view's tab.  

For more information, see the following articles: 

* [Share views](/help/quicksilver/planning/access/share-views.md)  

* [Share record types](/help/quicksilver/planning/access/share-record-types.md)
-->

<!--## Add teams as approvers on Planning request forms

>[!NOTE]
>
>* Preview: July 9, 2025 
>* Production for everyone: October 16, 20025 

To make the approval process more flexible, we've added the ability to add teams as approvers on Planning request forms. Now, you can enter and select team names when setting approvers. Any of the team members can make a decision, which counts as the approval decision for the entire team.

Previously, only individual users could be assigned as approvers. 

For more information, see [Add an approval to a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/add-approval-to-request-form.md).-->

## 共享请求表单时更新了体验

>[!NOTE]
>
>* 预览： 2025年7月9日
>* 适用于所有人的生产： 2025年7月17日

为了使在Workfront Planning中共享请求表单时体验更加安全和简单，我们进行了以下更改：

* 我们已删除继承的权限。 现在，请求表单仅与您选择的人共享。
* 我们已为您共享请求表单的用户删除了“管理”和“贡献”选项。 现在，添加的用户只能提交表单。
* 现在，仅在启用创建公共链接选项后，公共共享选项卡才会显示链接和过期日期字段。

有关详细信息，请参阅[在Adobe Workfront Planning中创建和管理申请表单](https://experienceleague.adobe.com/zh-hans/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-requests/create-request-form)。

## 展开和折叠表格视图中的所有分组

>[!NOTE]
>
>* 预览：2025年6月26日
>* 适用于所有人的生产： 2025年7月17日

现在，可以使用以下区域折叠和展开表格视图中的分组：

* 分组框，可从表格视图的工具栏访问

* 分组的标题，右键单击该标题

您可以同时折叠或展开一个分组或所有分组。

在此增强功能之前，您一次只能折叠或展开每个分组标题中的一个分组。

有关信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。

## 公式字段的新聚合功能

>[!NOTE]
>
>* 预览：2025年6月26日
>* 适用于所有人的生产： 2025年6月26日

现在，当您连接记录类型并将公式字段作为查找引入时，可以根据公式字段的格式应用聚合函数(SUM、AVERAGE、MIN、MAX等)。 例如，如果公式字段为数字，则可以使用SUM或AVG等函数；如果公式字段的格式为文本，则不会应用SUM等聚合函数。

以前，在连接记录类型并从连接的记录引入查找字段时，可以将集合函数仅应用于常规字段，而不能应用于公式字段。

有关信息，请参阅[公式字段概述](/help/quicksilver/planning/fields/formula-fields.md)。

## Workfront Planning时间线视图的自定义季度可用性

>[!NOTE]
>
>* 预览： 2025年6月12日
>* 生产快速发布： 2025年7月17日
>* 适用于所有客户的生产： 2025年7月17日

通过此更新，在“设置”的“项目首选项”区域中配置自定义季度时，自定义季度可用于Workfront Planning中的时间线视图。

在此更新之前，自定义季度仅可用于Workfront的报表功能。

有了这项改进，已购买Workfront Planning的客户将能够查看自定义季度定义的最新体验。 此更新包括以下改进：

不再接受各季度之间的差距和重叠。

您最多可以设置100个自定义季度。 在此更新之前，您只能设置8个自定义季度

对于未购买Workfront Planning的客户，其自定义季度体验没有变化。

有关详细信息，请参阅[为项目启用自定义季度](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md)。

## 同时计算所有从属公式

>[!NOTE]
>
>* 预览： 2025年6月12日
>* 生产快速发布： 2025年6月12日
>* 适用于所有客户的生产： 2025年6月12日

我们引入了一项改进，在手动更新引用的字段后，可同时更新所有相互依赖的公式字段。 与手动更改值的字段相差2、3或4个字段且相互引用的公式字段现在将自动同时更新。

在此改进之前，手动更新引用字段的值时，只更新直接相关的公式字段。

有关信息，请参阅[公式字段概述](/help/quicksilver/planning/fields/formula-fields.md)。

## 添加到公式字段的新表达式

>[!NOTE]
>
>* 预览：2025年6月6日
>* 生产快速发布： 2025年6月6日
>* 适用于所有客户的生产： 2025年6月6日

我们在公式字段中添加了以下表达式：

* ARRAYCONTAINS

* SORTASCARRAY

* SORTDESCARRAY

在此增强功能之前，这些表达式仅在Workfront计算的自定义字段中受支持。

有关信息，请参阅[公式字段概述](/help/quicksilver/planning/fields/formula-fields.md)。

## 在请求区域的Planning选项卡中添加了筛选器、列和其他字段

>[!NOTE]
>
>* 预览： 2025年5月29日
>* 生产快速发布： 2025年6月12日
>* 适用于所有客户的生产： 2025年7月17日

我们已将以下功能添加到请求区域的计划选项卡中的请求列表：

* 输入者列表示添加请求的人员
* 用于限制您在Planning选项卡上查看的请求数的过滤器。 可按以下项筛选列表：

   * 请求表单源自的Workspace
   * 与请求表单关联的记录类型
   * 请求的输入日期
   * 请求表单的名称
   * 请求的状态
   * 输入请求的人员的姓名。

* 列控制查看或隐藏Planning请求列表中的字段（或列）。

有关信息，请参阅[提交Adobe Workfront计划请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)。

## 在时间轴视图中以紧凑模式划分记录时的新体验

>[!NOTE]
>
>* 预览： 2025年5月22日
>* 生产快速发布： 2025年6月12日
>* 适用于所有客户的生产： 2025年7月17日

我们更改了在时间轴视图中划分记录时的体验，并且您应用了紧凑视图。
通过新的更新，当您在“紧凑”模式下定义划分对象并显示时间轴时，在完成划分条件的配置后，系统会提示您将视图切换为“标准”。

在此增强功能之前，在紧凑模式下显示时间轴视图时，无法定义划分条件。

在此升级中，“标准”选项是默认选项。 在此之前，默认模式为紧凑模式。

有关信息，请参阅[管理时间线视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

## 更新时间轴视图设置，以定义在使用划分选项时连接记录栏的外观

>[!NOTE]
>
>* 预览： 2025年5月15日
>* 生产快速发布： 2025年6月12日
>* 适用于所有客户的生产： 2025年7月17日

您现在可以为划分中的记录设置时间轴视图中记录栏外观的格式。 您可以更新这些记录栏的以下设置：

* 栏样式
* 颜色

在此增强功能之前，您只能格式化在时间轴视图中显示的主记录栏，并且不能格式化所连接记录的栏。\
 
有关信息，请参阅[管理时间线视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)。  

## 将表格视图导出为CSV或Excel文件 

>[!NOTE]
>
>* 预览： 2025年5月15日
>* 生产快速发布： 2025年6月12日
>* 适用于所有客户的生产： 2025年7月17日

我们为Workfront Planning添加了一项新功能，通过该功能，您可以将表视图中的可见信息导出为CSV或Excel文件。  

从表视图导出信息时，请考虑以下事项：  

* 导出的信息会考虑应用于Workfront Planning中的表格视图的筛选器、分组和排序。
* 导出的文件不支持缩略图和自定义行颜色。  
* 仅导出在Workfront界面中可见的字段。 隐藏字段不导出。  

有关详细信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。 

## 使用CSV或Excel文件导入记录时，现在支持Workfront Planning连接的字段

>[!NOTE]
>
>* 预览： 2025年5月15日
>* 生产快速发布： 2025年6月12日
>* 适用于所有客户的生产： 2025年7月17日

使用CSV或Excel文件将记录添加到记录类型时，现在可以填充已连接字段的值。  仅支持连接的Planning记录字段。 不支持显示与其他应用程序连接的字段。

导入CSV和Excel文件以创建记录类型和现有记录类型的记录时，支持此更改。

在此增强功能之前，在导入记录时无法填充连接字段。

有关信息，请参阅以下文章：

* [通过从CSV或Excel文件导入信息创建记录](/help/quicksilver/planning/records/import-file-to-create-records.md)。

* [通过从CSV或Excel文件导入信息来创建记录类型](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md)。

## 在记录的“连接的记录”页面中进行内联编辑

>[!NOTE]
>
>* 预览： 2025年4月30日
>* 生产快速发布： 2025年5月15日
>* 适用于所有客户的生产： 2025年7月17日

您现在可以在记录的“连接的记录”页面中编辑记录。 通过此更新，我们引入以下内容：

* 页面的名称已从“连接视图”更改为“连接的记录页面”。
* 此页面中显示的已连接记录可在表格视图中内联编辑。 连接的Workfront对象将继续以只读表格显示。

在此增强功能之前，对于记录连接，“连接”视图页面的表是只读的。

有关信息，请参阅[管理记录页布局](/help/quicksilver/planning/records/manage-the-record-page.md)。

## 默认情况下，Planning区域在标准许可证用户主菜单中可见

>[!NOTE]
>
>* 预览： 2025年4月30日
>* 生产快速发布： 2025年5月15日
>* 适用于所有客户的生产： 2025年7月17日

默认情况下，标准和系统管理员用户现在可以在主菜单中找到Planning区域，而无需将其分配给包含该区域的布局模板。 所有其他用户必须具有包含分配给他们的Planning区域的布局模板才能访问它。

在此增强功能之前，必须将所有许可证级别的用户分配给布局模板，修改后的布局模板必须在主菜单中包括Planning区域，才能访问此区域。

>[!NOTE]
>
>此更改将对具有系统管理员和标准许可证的所有新用户和现有用户可见。
>&#x200B;>分配到布局模板的现有用户将继续根据布局模板中定义的设置查看所有内容。

有关信息，请参阅[Adobe Workfront规划概述](/help/quicksilver/planning/access/access-overview.md)。

## 表格视图中的行级颜色格式

>[!NOTE]
>
>* 预览： 2025年4月30日
>* 生产快速发布： 2025年5月15日
>* 适用于所有客户的生产： 2025年7月17日

为了更好地显示记录的重要信息，我们为表格视图引入了行级颜色格式。 现在，您可以在定义每行的条件后，为每一行选择一种颜色。  这是一项新功能，在此更新之前不存在。

有关信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。

## 在标准时间线视图中截断长记录名称的新设置

>[!NOTE]
>
>* 预览： 2025年4月23日
>* 生产快速发布： 2025年5月15日
>* 适用于所有客户的生产： 2025年7月17日

现在，您可以在时间轴视图的“设置”框的“条形图样式”选项卡中启用设置，以在标准视图中显示较长记录名称时截断这些名称。 默认情况下，该设置处于禁用状态，仅当您在“标准”模式下显示时间轴视图时才能启用。 由于禁用此设置，默认情况下，记录栏上的信息显示为展开状态。 在此增强功能之前，默认情况下，记录栏上的信息被截断。

有关信息，请参阅[管理时间线视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

## 共享记录类型的权限


>[!NOTE]
>
>* 预览： 2025年4月17日
>* 生产快速发布： 2025年7月17日
>* 适用于所有客户的生产： 2025年7月17日

为了更好地控制谁可以查看或管理每种记录类型中的记录，并确保只有授权人员才能根据其角色和职责管理每种记录类型的信息，我们在记录类型级别引入了权限。

在此增强功能之前，您只能与他人共享工作区，并且向工作区授予的权限适用于工作区中的所有记录类型。

我们引入了以下更新：

* Workspace权限会自动与工作区中的所有记录类型共享。
* 授予工作区的权限级别显示为记录类型的继承权限。
* 您无法以高于用户在工作区中的权限级别共享记录类型。
* 您可以禁用记录类型的继承权限，使其对工作区中的所有用户都为只读。 之后，您可以添加个人、团队、组、公司或角色，并向他们授予记录类型的Contribute权限。

有关详细信息，请参阅[共享记录类型](/help/quicksilver/planning/access/share-record-types.md)。


