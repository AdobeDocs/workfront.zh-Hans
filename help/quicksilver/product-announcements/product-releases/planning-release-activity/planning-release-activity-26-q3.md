---
content-type: release-notes
title: Adobe Workfront Planning 2026年第三季度发布活动
description: 这是Adobe Workfront计划产品2026年第三季度的发布活动。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: c3131cb38ac6f71cdd98149c8d49177d59b7accf
workflow-type: tm+mt
source-wordcount: '2826'
ht-degree: 0%

---

# Adobe Workfront Planning 2026年第三季度发布活动

<!--
take the next sentence out when we start listing features
-->

<!--
There are no features released during the Third Quarter Release for 2026. When features are released for this quarter, we will document them in this article. 
-->

<!--keep the sentence below for all future quarterly release pages-->

本文介绍了在2026年第三季度版本中为Workfront计划发布的功能。

有关为Adobe Workfront Planning发布的所有功能的列表，请参阅[Adobe Workfront Planning发布活动：文章索引](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。

## Snowflake中Workfront Planning的自动访问控制

>[!IMPORTANT]
>
>面向所有客户的预览和生产： 2026年7月16日超出计划]{type=Neutral}


此发行版本引入了对Snowflake中Workfront Planning数据的自动授权驱动访问管理，作为Workfront Data Connect的一部分。

首先，将安全视图生成扩展到Planning表，为下游访问控制奠定必要的基础，并使基于权利的授权成为可能。

以此为基础，读取器帐户设置现在在创建时检查TMS权限，并自动应用或保留对Planning数据库的授权，确保正确无误。

在此增强功能之前，这仅适用于Workfront。

此更新包括以下功能：

* 自动的每日作业可检测现有客户的授权更改
* 新作业根据权限授予、撤销或保留访问权限
* 覆盖整个生命周期的资源调配、帐户创建以及持续的授权更改。

[Workfront Data Connect数据字典](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md)文章将在发布日期后更新。


## 设置记录的默认权限

>[!NOTE]
>
>预览：2026年7月7日生产快速发布： 2026年7月15日适用于所有人的生产： 2026年7月16日

Workspace管理员现在可以为每种记录类型设置默认权限规则（“打开”或“受限”），因此新创建的记录无需任何手动步骤即可自动受到保护。

选择“受限”时，只有记录创建者和任何特别选择的用户、组、团队、角色或公司可以编辑记录，而其他所有人将保留仅查看权限。

此规则自动应用于新记录，而不管该记录的创建方式如何（新记录按钮、请求表单、API、使用Fusion自动化或AI助手）。 对规则的更改只会影响以后创建的记录，而不会影响现有的记录。

创建记录后，仍可以独立更新其权限，而不会影响未来记录的默认规则。

有关信息，请参阅[设置记录的默认权限](/help/quicksilver/planning/access/set-default-record-permissions.md)。

## 时间轴视图的泳道分组布局

>[!NOTE]
>
>预览：2026年7月7日生产快速发布： 2026年7月15日适用于所有人的生产： 2026年7月16日

分组的时间轴视图现在支持泳道布局，其中分组呈现为冻结的左标题列而不是滚动的水平条带。 此分组类型是当前栈叠分组的附加类型。

嵌套的分组级别显示为缩进的子列，并且每个车道中的记录都保持子栈叠状态并排序。

您可以在分组视图中拖放记录，以顺利更新其信息和日期。

所有查看视图的用户都可以看到应用的分组。

有关信息，请参阅[管理时间线视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)。


## 支持画布仪表板中的货币计划字段

>[!NOTE]
>
>预览：2026年6月25日生产快速发布： 2026年7月15日适用于所有人的生产： 2026年7月16日

现在，您可以在画布功能板中的表格、KPI和图表报表中包含货币计划字段。

在此增强功能之前，画布功能板不支持货币字段。

有关信息，请参阅[在画布功能板中使用货币字段](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md)。

## 行颜色控件界面改进

>[!NOTE]
>
>预览：2026年6月22日生产快速发布： 2026年7月15日适用于所有人的生产： 2026年7月16日

我们更新了表格视图中“行颜色”控件的外观。

有关详细信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。

## 为选定和人员类型字段添加默认选项

>[!NOTE]
>
>预览：2026年6月18日生产快速发布： 2026年7月15日适用于所有人的生产： 2026年7月16日

在创建单选、多选字段或“人员”类型字段时，您现在可以指定这些字段的默认值。 当字段在记录中可见时，将始终应用默认值。

保存字段后，您可以更改该字段的默认设置。 处理记录时，可以替换字段的默认值。

有关信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。

## 改进了表格视图中的界面

>[!NOTE]
>
>预览：2026年6月11日生产快速发布： 2026年7月15日适用于所有人的生产： 2026年7月16日

我们更新了Workfront Planning中以下领域的表格视图的外观：

* 所有记录类型页面

* 所有连接的记录类型页面，项目除外

除了一些导航更改和设计改进之外，此更新中的某些改进包括：

* 在表底部添加汇总行，该汇总行使用以下汇总器汇总数字、货币、百分比和一些公式字段：SUM、AVG、MAX、MIN。

* 添加日期字段时使用更简单的日期格式，格式类型更少。

* 添加日期字段时，能够选择所有用户可见的时区，无论其用户档案的时区如何。

* 删除了行编号，使外观更干净

* 持久行选择框，而不是仅在悬停在行上时可见

* 持久化列分隔符行以提高可读性

* 从列标题排序时更简单的排序体验

有关详细信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。


## GenStudio for Performance Marketing品牌现在可以添加到Planning请求表单中

>[!NOTE]
>
>适用于所有客户的预览和生产： 2026年6月5日仅适用于也拥有Adobe GenStudio for Performance Marketing的Adobe Workfront Planning客户。超出计划]{type=Neutral}


要允许从提交请求开始将品牌添加到营销活动，现在可将“连接的品牌”记录字段添加到“计划”请求表单。

当Planning记录类型与GenStudio Brands记录类型连接时，您可以将Brands connected字段添加到与Planning记录类型关联的Planning请求表单。

有关信息，请参阅[Adobe Workfront Planning与Adobe GenStudio for Performance Marketing集成入门](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)。


## Planning登陆页面中新增了示例工作区选项卡

>[!NOTE]
>
>预览：2026年6月1日生产快速发布： 2026年6月11日适用于所有人的生产： 2026年7月16日


我们在Planning登录区域中添加了Sample workspaces选项卡，您可以在其中查看最佳实践工作区示例。 工作区不可编辑。 Workspace管理员可以修改示例工作区中的视图。 该选项卡对标准和系统管理员用户可见。

我们建议您查看示例工作区作为示例，并使用多工作区模板包来创建、编辑和共享因使用该模板而产生的工作区。  模板捆绑包含的工作区与“示例工作区”选项卡相同。

有关信息，请参阅[工作区概述](/help/quicksilver/planning/architecture/workspaces-overview.md)。

>[!NOTE]
>
>仅工作流Prime或Ultimate包中的组织可使用模板包创建工作区。

## Workfront计划API版本2

>[!NOTE]
>
>所有客户均可用： 2026年5月28日超出计划]{type=Neutral}

Workfront Planning API版本2现已可用，它显着扩展了版本1的功能。

版本2中包含以下增强功能：

* 以编程方式创建、更新和删除工作区、记录类型和字段。

* 完全管理记录。
* 改进了URL结构、错误处理、分页、筛选和权限。
* 包括通过PATCH进行的部分更新
* 包括批量记录操作。

版本1仍然可用，但我们建议您转为使用版本2。

>[!NOTE]
>
>Workfront Planning connector for Fusion尚未更新到API版本2，在进一步通知之前，它将继续使用版本1。

有关信息，请参阅[Adobe Workfront规划API基础知识](/help/quicksilver/planning/general/planning-api-basics.md)。

有关Workfront计划API规范，请参阅[Workfront计划API](https://developer.adobe.com/wf-planning/)开发人员文档。

## 向记录授予权限

>[!NOTE]
>
>预览： 2026年5月28日生产快速发布： 2026年6月11日适用于所有人的生产： 2026年7月16日


您现在可以调整单个记录权限，以控制谁可以在记录类型中管理它们。

默认情况下，用户从工作区和记录类型继承记录权限。 您现在可以覆盖特定记录的继承权限，以授予一部分用户的查看或管理访问权限。 权限覆盖可应用于单个记录，也可以跨多个记录批量更新。

<!-- 
Laurel asked for this to be replaced with the above: 

Users inherit record permissions from the workspace and record type by default. To give only select users with record type permissions Manage permissions to only certain records, you can disable inherited permissions on select records and grant only those users Manage access to those records. You can adjust permissions for one record, or for multiple records at the same time, in bulk.

You can give users the following permissions levels: 

* View 
* Manage 
-->

>[!NOTE]
>
>* 用户的记录级别权限不能超过其记录类型权限。 例如，对记录类型具有“查看”权限的用户不能被授予对该类型的单个记录的“管理”权限。
>* 此时无法从记录中删除用户的权限。 至少具有该记录类型查看权限的任何用户都可以查看该类型的所有记录。

有关信息，请参阅[共享记录](/help/quicksilver/planning/access/share-records.md)。

## 简化的全局记录类型添加

>[!NOTE]
>
>预览： 2026年5月28日生产快速发布： 2026年6月11日适用于所有人的生产： 2026年7月16日

为了减少点击次数并帮助您快速找到所需的记录类型，我们增强了添加记录的体验，以便您在将全局记录类型添加到另一个工作区时更快、更直观。

现在，当您选择从现有记录类型添加记录时，您将立即看到所有可用全局记录类型的列表。

您可以直接从此屏幕同时选择并添加一个或多个全局记录类型。

有关信息，请参阅[从另一个工作区添加现有记录类型](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)。

## Beta中现在提供所有Designer Planning客户的Planning Workfront

>[!NOTE]
>
>预览： 2026年5月28日生产快速发布： 2026年6月11日适用于所有人的生产： 2026年7月16日在Beta]{type=Neutral}中

您现在可以使用由AI提供支持的Adobe Planning Designer来轻松配置工作区和数据结构。 Planning Designer支持从创建和配置工作区到定义字段和公式、管理记录、查看更改历史记录和构建自定义视图的所有功能。

无论直接使用还是通过AI Assistant，Planning Designer都为构建和维护结构化、关联的信息提供了一个灵活、强大的环境。

Workfront管理员可以从“设置”的系统首选项区域管理Planning Designer的可用性。

有关信息，请参阅[Adobe Workfront规划Designer入门](/help/quicksilver/planning/general/planning-ai-designer.md)。


## 将元数据从Planning同步到AEM Assets

>[!NOTE]
>
>适用于所有人的预览和生产： 2026年5月28日仅适用于同时拥有Adobe GenStudio for Performance Marketing和Adobe Experience Manager的Adobe Workfront Planning客户。超出计划]{type=Neutral}

为了提高数据完整性，当GenStudio for Performance Marketing链接到Workfront Planning中的AEM Assets记录类型时，我们已发布AEM Assets记录类型与GenStudio之间的无缝元数据同步。

以下GenStudio for Performance Marketing记录类型可以连接到AEM Assets：营销活动、产品、角色、地区和渠道。

添加到Workfront Planning中GenStudio记录类型的信息显示在AEM中AEM资源的单独Campaign选项卡中。 该营销活动的产品、角色、区域和渠道的相关信息也会以只读模式显示在该选项卡上。

在此版本中，关键元数据在两个平台上都是一致的，并近乎实时地反映了更新，从而减少了手动协调。

有关信息，请参阅[在Adobe Workfront规划中管理GenStudio工作区](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)。

## 将元数据从Planning同步到AEM内容片段

>[!NOTE]
>
>适用于所有人的预览和生产： 2026年5月28日仅适用于同时拥有Adobe GenStudio for Performance Marketing和Adobe Experience Manager的Adobe Workfront Planning客户。超出计划]{type=Neutral}

为了提高数据完整性，当内容片段链接到AEM营销活动时，我们已发布了GenStudio工作区中的Planning记录类型与GenStudio for Performance Marketing内容片段之间的无缝元数据同步。

GenStudio促销活动信息现在显示在AEM中内容片段的“元数据”选项卡中。  该营销活动的产品、角色、区域和渠道的相关信息也会以只读模式显示在该选项卡上。

在此版本中，关键元数据在两个平台上都是一致的，并近乎实时地反映了更新，从而减少了手动协调。

有关信息，请参阅[在Adobe Workfront规划中管理GenStudio工作区](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)。


## 列表视图更新

>[!NOTE]
>
>预览： 2026年5月27日生产快速发布： 2026年6月11日适用于所有人的生产： 2026年7月16日

列表视图上的多个字段类型已更新，包括键盘导航和其他增强功能。

现在，多选、单选和代理人字段在列表视图中提供键盘导航：

* 使用键盘上的上下箭头在人员列表中移动。

* 按空格键以选择人员或删除所选人员。

在列表视图中的单选和多选字段上：

* 在未找到结果时，可以直接从编辑器中添加新选项。 请注意，此功能可能并非在所有列表中都可用。

* 字段交互现在可使用键盘。 这包括使用向上和向下箭头在标记、搜索选项和列表之间导航。 按空格键选择项目或删除选定项目。

引用字段（如预输入字段和外部查找字段）已收到一些界面增强。

此外，在提供时，还以可视方式改善了列的拖放体验。

有关详细信息，请参阅[在Adobe Workfront规划中管理列表视图](/help/quicksilver/planning/views/manage-the-list-view.md)。

## Workfront引用字段作为Planning连接的查找字段启用

>[!NOTE]
>
>预览： 2026年5月27日生产快速发布： 2026年6月11日\
>适用于所有人的生产： 2026年7月16日

将Workfront记录类型与Workfront对象类型连接时，您现在可以将Planning引用字段添加为查找字段。

例如，您可以将“项目”对象中的“Portfolio”、“项目”、“组”或“公司”信息添加到Planning中促销活动的项目连接字段。

有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。

## 时间轴视图划分功能的新筛选器

>[!NOTE]
>
>预览： 2026年5月27日生产快速发布： 2026年6月11日适用于所有人的生产： 2026年7月16日

您现在可以根据条件筛选时间轴视图中的信息，这些条件与记录划分中包含的对象匹配。

在此增强功能之前，您只能为时间线视图中的主记录应用过滤器。

有关信息，请参阅[管理时间线视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

## 新指示已编辑和删除字段会影响请求表单

>[!NOTE]
>
>预览： 2026年5月27日生产快速发布： 2026年6月11日适用于所有人的生产： 2026年7月16日

我们添加了提醒，提醒您编辑或删除的记录字段可能会影响包含这些字段的请求表单。 现在，您将有机会查看受影响的表单，并确保要对字段进行的更改不会影响现有信息。

有关信息，请参阅[编辑字段设置](/help/quicksilver/planning/fields/edit-fields.md)。

## 编辑提交的规划请求

>[!NOTE]
>
>预览： 2026年5月27日生产快速发布： 2026年6月11日适用于所有人的生产： 2026年7月16日

现在，您可以在提交Planning请求之后、根据请求创建记录之前对其进行编辑。

以下用户可以编辑提交的请求：

* 请求创建者
* 提交请求的工作区的Workspace管理器
* 系统管理员

在此增强功能之前，您无法编辑提交的请求。

有关详细信息，请参阅[提交Adobe Workfront计划请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)。

## AEM内容片段的新预览窗口

>[!NOTE]
>
>面向所有客户的预览和生产： 2026年5月14日超出计划]{type=Neutral}

为了在使用连接到AEM Planning记录的Workfront内容片段时提高可见性，我们添加了一个预览窗口，用于在Workfront Planning中显示有关片段的信息。

此功能以前可用于AEM资源，现在我们将其添加到内容片段。

有关信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。

## Workfront Planning中现在提供AEM内容片段的查找字段

>[!NOTE]
>
>面向所有客户的预览和生产： 2026年5月14日仅适用于也拥有Adobe Experience Manager的Adobe Workfront Planning客户。超出计划]{type=Neutral}

现在，在将Planning记录类型连接到AEM内容片段时，可以添加以下查找字段：

* 创建者
* 创建于
* 修改者
* 修改时间

在此增强功能之前，查找字段仅可用于AEM资源和文件夹。

有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。



## 记录详细信息页面的自定义视图

>[!NOTE]
>
>预览： 2026年5月14日生产快速发布： 2026年6月11日适用于所有人的生产： 2026年7月16日

为了在记录的详细信息页面中更加灵活地可视化您的信息，我们引入了为此页面创建自定义视图的功能。

除了添加两个已构建的详细信息页面视图（包含所有记录字段或仅包含表格视图中可见的字段）之外，您现在还可以为记录的详细信息页面创建自定义视图。 您创建的视图对可以访问该记录的每个人都可见。

此更新将删除&#x200B;**显示所有字段**&#x200B;设置，并将其替换为自定义详细信息视图。

有关信息，请参阅[管理记录页](/help/quicksilver/planning/records/manage-the-record-page.md)。

## 向“连接的项目”记录页面添加分组

>[!NOTE]
>
>预览： 2026年5月14日\
>快速生产：2026年6月11日适用于所有人的生产： 2026年7月16日

您现在可以在Workfront Planning中记录的“连接的项目”记录页面中对您的信息进行分组。 在此增强功能之前，此区域中不存在此功能。

有关信息，请参阅[管理列表视图](/help/quicksilver/planning/views/manage-the-list-view.md)。

