---
content-type: release-notes
title: Adobe Workfront Planning 2026年第三季度发布活动
description: 这是Adobe Workfront计划产品2026年第三季度的发布活动。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: ab1ac1363d6531352e905536218618196651c3b9
workflow-type: tm+mt
source-wordcount: '1448'
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



<!--

## Planning Designer now available in Beta for all Workfront Planning customers

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 
>[!BADGE In Beta]{type=Neutral}

You can now use the Adobe Planning Designer powered by AI to configure your workspaces and data structures with ease. The Planning Designer supports everything from creating and configuring workspaces to defining fields and formulas, managing records, reviewing change history and building custom views.  

Whether used directly or through the AI Assistant, the Planning Designer provides a flexible, powerful environment for building and maintaining structured, connected information. 

A Workfront administrator can manage the availability of the Planning Designer from the System Preferences area in Setup.   

For information, see [Get started with the Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).

## New Sample workspaces tab added to the Planning landing page

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

We have added the Sample workspaces tab in the Planning landing area where you can view example of best-practice workspaces. The workspaces are not editable and we recommend that you use them as examples to create your own.  

We also recommend that you use the multi-workspace template to create, and edit and share workspaces that result as a use of that template.  The template contains the same workspaces as the Sample workspaces tab.   

Workspace managers can modify views in sample workspaces.     

For information, see Workspaces overview (/help/quicksilver/planning/architecture/workspaces-overview.md). 

-->

## Workfront计划API版本2

>[!NOTE]
>
>适用于所有客户： 2026年5月28日>[!BADGE 不按计划]{type=Neutral}

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
>预览： 2026年5月28日>生产快速发布： 2026年6月11日>适用于所有人的生产： 2026年7月16日

您现在可以调整单个记录权限，以控制谁可以在记录类型中管理它们。

默认情况下，用户从工作区和记录类型继承记录权限。 要仅向具有记录类型权限的select用户授予仅管理某些记录的权限，您可以禁用对选定记录的继承权限，并仅向这些用户授予对这些记录的“管理”访问权限。 您可以批量调整一个记录的权限，或同时调整多个记录的权限。

您可以授予用户以下权限级别：

* 视图
* 管理

>[!NOTE]
>
>* 用户的记录级别权限不能超过其记录类型权限。 例如，对记录类型具有“查看”权限的用户不能被授予对该类型的单个记录的“管理”权限。
>* 此时无法从记录中删除用户的权限。 至少具有该记录类型查看权限的任何用户都可以查看该类型的所有记录。

有关信息，请参阅[共享记录](/help/quicksilver/planning/access/share-records.md)。

## 简化的全局记录类型添加

>[!NOTE]
>
>预览： 2026年5月28日>生产快速发布： 2026年6月11日>适用于所有人的生产： 2026年7月16日

为了减少点击次数并帮助您快速找到所需的记录类型，我们增强了添加记录的体验，以便您在将全局记录类型添加到另一个工作区时更快、更直观。

现在，当您选择从现有记录类型添加记录时，您将立即看到所有可用全局记录类型的列表。

您可以直接从此屏幕同时选择并添加一个或多个全局记录类型。

有关信息，请参阅[从另一个工作区添加现有记录类型](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)。


## 将元数据从Planning同步到AEM Assets

>[!NOTE]
>
>预览： 2026年5月28日>生产快速发布： 2026年5月28日>适用于所有人的生产： 2026年5月28日>[!BADGE 取消计划]{type=Neutral}

为了提高数据完整性，当GenStudio for Performance Marketing链接到Workfront Planning中的AEM Assets记录类型时，我们已发布AEM Assets记录类型与GenStudio之间的无缝元数据同步。

以下GenStudio for Performance Marketing记录类型可以连接到AEM Assets：营销活动、产品、角色、地区和渠道。

添加到Workfront Planning中GenStudio记录类型的信息显示在AEM中AEM资源的单独Campaign选项卡中。 该营销活动的产品、角色、区域和渠道的相关信息也会以只读模式显示在该选项卡上。

在此版本中，关键元数据在两个平台上都是一致的，并近乎实时地反映了更新，从而减少了手动协调。

有关信息，请参阅[在Adobe Workfront规划中管理GenStudio工作区](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)。

## 将元数据从Planning同步到AEM内容片段

>[!NOTE]
>
>预览： 2026年5月28日>生产快速发布： 2026年5月28日>适用于所有人的生产： 2026年5月28日>[!BADGE 取消计划]{type=Neutral}

为了提高数据完整性，当内容片段链接到AEM营销活动时，我们已发布了GenStudio工作区中的Planning记录类型与GenStudio for Performance Marketing内容片段之间的无缝元数据同步。

GenStudio促销活动信息现在显示在AEM中内容片段的“元数据”选项卡中。  该营销活动的产品、角色、区域和渠道的相关信息也会以只读模式显示在该选项卡上。

在此版本中，关键元数据在两个平台上都是一致的，并近乎实时地反映了更新，从而减少了手动协调。

有关信息，请参阅[在Adobe Workfront规划中管理GenStudio工作区](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)。


## 列表视图更新

>[!NOTE]
>
>预览： 2026年5月27日>生产快速发布： 2026年6月11日>适用于所有人的生产： 2026年7月16日

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
>预览： 2026年5月27日>生产快速发布： 2026年6月11日\
>适用于所有人的生产： 2026年7月16日

将Workfront记录类型与Workfront对象类型连接时，您现在可以将Planning引用字段添加为查找字段。

例如，您可以将“项目”对象中的“Portfolio”、“项目”、“组”或“公司”信息添加到Planning中促销活动的项目连接字段。

有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。

## 时间轴视图划分功能的新筛选器

>[!NOTE]
>
>预览： 2026年5月27日>生产快速发布： 2026年6月11日>适用于所有人的生产： 2026年7月16日

您现在可以根据条件筛选时间轴视图中的信息，这些条件与记录划分中包含的对象匹配。

在此增强功能之前，您只能为时间线视图中的主记录应用过滤器。

有关信息，请参阅[管理时间线视图](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

## 新指示已编辑和删除字段会影响请求表单

>[!NOTE]
>
>预览： 2026年5月27日>生产快速发布： 2026年6月11日>适用于所有人的生产： 2026年7月16日

我们添加了提醒，提醒您编辑或删除的记录字段可能会影响包含这些字段的请求表单。 现在，您将有机会查看受影响的表单，并确保要对字段进行的更改不会影响现有信息。

有关信息，请参阅[编辑字段设置](/help/quicksilver/planning/fields/edit-fields.md)。

## 编辑提交的规划请求

>[!NOTE]
>
>预览： 2026年5月27日>生产快速发布： 2026年6月11日>适用于所有人的生产： 2026年7月16日

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
>预览： 2026年5月14日>生产快速发布： 2026年5月14日>适用于所有人的生产： 2026年5月14日>[!BADGE 取消计划]{type=Neutral}

为了在使用连接到AEM Planning记录的Workfront内容片段时提高可见性，我们添加了一个预览窗口，用于在Workfront Planning中显示有关片段的信息。

此功能以前可用于AEM资源，现在我们将其添加到内容片段。

有关信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。

## Workfront Planning中现在提供AEM内容片段的查找字段

>[!NOTE]
>
>预览： 2026年5月14日>生产快速发布： 2026年5月14日>适用于所有人的生产： 2026年5月14日>[!BADGE 取消计划]{type=Neutral}

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
>预览： 2026年5月14日>生产快速发布： 2026年6月11日>适用于所有人的生产： 2026年7月16日

为了在记录的详细信息页面中更加灵活地可视化您的信息，我们引入了为此页面创建自定义视图的功能。

除了添加两个已构建的详细信息页面视图（包含所有记录字段或仅包含表格视图中可见的字段）之外，您现在还可以为记录的详细信息页面创建自定义视图。 您创建的视图对可以访问该记录的每个人都可见。

此更新将删除&#x200B;**显示所有字段**&#x200B;设置，并将其替换为自定义详细信息视图。

有关信息，请参阅[管理记录页](/help/quicksilver/planning/records/manage-the-record-page.md)。

## 向“连接的项目”记录页面添加分组

>[!NOTE]
>
>预览： 2026年5月14日\
>快速生产： 2026年6月11日>为每个人生产： 2026年7月16日

您现在可以在Workfront Planning中记录的“连接的项目”记录页面中对您的信息进行分组。 在此增强功能之前，此区域中不存在此功能。

有关信息，请参阅[管理列表视图](/help/quicksilver/planning/views/manage-the-list-view.md)。
