---
content-type: release-notes
title: Adobe Workfront Planning 2026年第一季度发布活动
description: 这是Adobe Workfront计划产品2026年第一季度的发布活动。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 46f3be50925d2e830c572ce9bbad0d3b320f6a95
workflow-type: tm+mt
source-wordcount: '1501'
ht-degree: 0%

---

# Adobe Workfront Planning 2026年第一季度发布活动

本文介绍了在2026年第一季度发行的Workfront Planning功能。

<!--keep the sentence below for all future quarterly release pages-->

有关为Adobe Workfront Planning发布的所有功能的列表，请参阅[Adobe Workfront Planning发布活动：文章索引](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。

## 改进了“连接的记录”页面

>[!NOTE]
>
>预览： 2025年12月19日
>快速生产： 2026年1月14日
>全部生产： 2026年1月15日

为了让您在处理连接的记录页面时拥有更大的灵活性，我们增强了Workfront Planning此区域中的视图功能。 以下是对记录的已连接记录页面的改进：

* 您现在可以将时间轴和日历视图添加到记录的“连接的记录”页面。
* 您现在可以从连接的记录页面共享所有视图。 在Workfront Planning的任何其他区域中，与您共享这些页面的用户可以在系统范围内查看这些页面的共享视图。 在Planning的任何其他区域共享的所有视图也会在与其共享这些视图的相同用户的已连接记录页面中可见。
* 我们添加了限制，每个记录或对象类型仅允许一个连接的记录页面。 在此增强功能之前，您可以为同一记录或对象类型添加多个页面。 现在，您可以在一个连接的记录页面中为同一记录类型使用多个视图。
* 我们在表视图底部添加了&#x200B;**新行**&#x200B;链接，并在连接的记录页面的右上角区域添加了&#x200B;**连接记录**&#x200B;按钮。 在此增强功能之前，**新行**&#x200B;链接和&#x200B;**连接记录**&#x200B;按钮仅存在于连接的项目页面上。

有关信息，请参阅[将“连接的记录”页面添加到记录](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)。

## 在“连接的项目”记录页面中共享视图

>[!NOTE]
>
>预览： 2025年12月18日
>生产快速发布： 2026年1月14日\
>适用于所有人的生产： 2026年1月15日

为了更便于确保查看您需要的信息，我们添加了将视图共享到“连接的项目”记录页面的功能。 现在，您可以与其他用户、团队或组共享视图。

有关信息，请参阅[将“连接的记录”页面添加到记录](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)。

## 项目连接视图筛选器中现在提供当前用户通配符

>[!NOTE]
>
>预览： 2025年12月18日
>生产快速发布： 2026年1月14日\
>适用于所有人的生产： 2026年1月15日

为了更便于筛选适用于您的项目连接，我们创建了一个当前用户通配符。 现在，在筛选时，您可以选择“我（已登录用户）”。 该过滤器随后将应用于正在查看请求列表的用户。

当向多个用户将使用的视图添加过滤器时，这会很方便。 每个用户都将看到适用于他们的筛选结果。

通配符在值为用户的字段中可用。

有关配置项目连接视图（包括筛选器）的详细信息，请参阅[将连接的记录页添加到记录](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)。

<!--

## Create record type hierarchies in workspaces

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production all: January 15, 2026 

You can now define flexible but structured hierarchies between record or object types.  

Hierarchies are connections between record types. You can have up to 4 record and object types connected in one hierarchy, and you can have multiple hierarchies in one workspace. The first record type in the hierarchy is a parent, and all the other record or object types are its children objects.  

You can use hierarchies to organize work in a way that reflects how your teams actually plan, operate, and deliver and to visualize how strategy flows into execution. 

Consider the following when building hierarchies: 

* You can have multiple hierarchies in a workspace 
* You can connect only Planning record types from one workspace and Workfront projects in a hierarchy.  
* A record type or a project can only have one parent in the same workspace. 
* A record type can be the parent in multiple hierarchies 
* Connectable record types cannot be used in hierarchies in other workspaces than their own. 
* Global record types can be used in hierarchies only in the workspaces that they were created in or have been added to.  

When you create hierarchies between record types, they generate breadcrumbs for records that belong to those record types. 

For more information, see [Hierarchy and breadcrumb overview](help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

-->

<!--

## New unified breadcrumbs added to records' pages

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production for all: January 15, 2026 

We have added breadcrumbs to a record's page to reflect its spot in a hierarchy. After you create hierarchies, you can see a record's breadcrumb at the top of its page, indicating what other parent or children objects are connected to it. Hierarchies are consistent across Workfront and Planning.  

For example, you can view a project's Planning hierarchy when it's connected to Planning record types in its Planning breadcrumb, and its Workfront hierarchy when it's connected to Workfront object types, like Portfolios or Programs, in Workfront.  

For information, see [Hierarchy and breadcrumb overview](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

-->

## Workspace主页改进

>[!NOTE]
>
>预览： 2025年12月18日
>快速生产： 2026年1月14日
>全部生产： 2026年1月15日

我们对Workfront Planning中的Workspaces主页进行了以下改进：

* 更快、更动态的滚动体验。 如果您的组织拥有大量工作区并且是系统管理员可以看到的情况，则这一点尤为明显。

* 我们添加了一个搜索框，现在可让您按名称搜索特定工作区。

* **其他工作区**&#x200B;选项卡已重命名为&#x200B;**所有工作区**，并且其中包含您至少拥有查看权限的所有工作区，包括您创建的那些工作区。

有关信息，请参阅[编辑工作区](/help/quicksilver/planning/architecture/edit-workspaces.md)。



## 在GenStudio工作区中，默认将Brand Connection字段添加到“产品和角色”

>[!NOTE]
>
>预览： 2025年12月11日
>生产快速发布： 2025年12月11日
>适用于所有人的生产： 2025年12月11日
>[!BADGE 超出计划]{type=Neutral}

现在，与GenStudio for Performance Marketing品牌的连接字段默认添加到Workfront Planning的GenStudio工作区中的“产品”和“角色”记录类型。

您的组织必须同时具有Workfront Planning和Adobe GenStudio for Performance Marketing。

在此增强功能之前，您只能手动将Brand Connection字段添加到任何记录类型，包括Products和Personas。 您仍然可以在Workfront Planning中手动将Brand GenStudio记录类型连接到其他记录类型。

有关信息，请参阅[Adobe Workfront Planning与Adobe GenStudio for Performance Marketing集成入门](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)。

## 限制从Planning中删除GenStudio for Performance Marketing用户的权限

>[!NOTE]
>
>预览： 2025年12月11日
>生产快速发布： 2025年12月11日
>适用于所有人的生产： 2025年12月11日
>[!BADGE 超出计划]{type=Neutral}

我们添加了护栏，用于防止从Workfront Planning对象中删除GenStudio for Performance Marketing用户的权限。 经过这项改进后，您无法再从Planning的GenStudio工作区中移除GenStudio用户，也无法在GenStudio工作区中禁用记录类型的继承权限(如果这些权限包括GenStudio用户)。 在此改进之前，当您从Planning的GenStudio工作区中删除这些用户时，他们也将失去在GenStudio中记录类型的权限。

您的组织必须同时具有Workfront Planning和Adobe GenStudio for Performance Marketing。

有关信息，请参阅[Adobe Workfront规划和Adobe GenStudio for Performance Marketing集成入门](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)。


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






