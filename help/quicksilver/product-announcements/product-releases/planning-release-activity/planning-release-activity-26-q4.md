---
content-type: release-notes
title: Adobe Workfront Planning 2026年第四季度发布活动
description: 这是Adobe Workfront Planning产品2026年第四季度的发布活动。
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 81eb918df24ec95f911d7c91268239503af434ee
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 0%

---

# Adobe Workfront Planning 2026年第四季度发布活动

本文介绍了在2026年第四季度版本中为Workfront计划发布的功能。

有关为Adobe Workfront Planning发布的所有功能的列表，请参阅[Adobe Workfront Planning发布活动：文章索引](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。

## 更新了相关已连接记录字段的列标题

>[!NOTE]
>
>预览： 2026年8月20日
>生产快速发布： 2026年9月17日
>适用于所有人的生产： 2026年10月15日

我们在可视化方面改进了表视图中相关已连接记录字段的列标题。

有关信息，请参阅[管理从属连接](/help/quicksilver/planning/architecture/manage-dependent-connections.md)。

## 拖放多行时的表格视图增强功能

>[!NOTE]
>
>预览： 2026年8月13日
>生产快速发布： 2026年8月13日
>适用于所有人的生产： 2026年10月15日

在表格视图中拖放多行时，会出现新的可视指示器。 现在，更突出的加号和数字指示器可显示为拖放操作选择的行数。

有关信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。

<!--

## Collapse and expand all groupings in the timeline view

>[!NOTE]
>
>Preview: August 13, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

Timeline views now include Collapse all and Expand all options for grouped timelines. This makes it easier to navigate large roadmap views: you can quickly reduce the view to grouping headings, then expand only the sections you want to review.

For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).

-->

## 使用全局记录类型时，将提交的请求对象路由到正确的工作区

>[!NOTE]
>
>预览： 2026年8月13日
>生产快速发布： 2026年9月17日
>适用于所有人的生产： 2026年10月15日

现在，通过提交请求表单为全局记录类型创建的记录会自动路由到从中提交这些记录的工作区。

通过从全局记录类型的辅助工作区提交请求而创建的记录将添加到该辅助工作区。 通过从原始工作区或主请求区域提交请求而创建的记录将添加到原始工作区。

如果摄取表单包含Workspace字段，并且用户在提交之前选择工作区，则无论表单是在何处启动的，请求都会路由到所选工作区。 这可确保从创建记录的那一刻起，就按预期的工作区对记录进行整理。

有关信息，请参阅[提交Adobe Workfront计划请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)。

## Workfront Planning解决方案架构师技能简介

>[!NOTE]
>
>预览： 2026年8月10日
>生产日期： 2026年8月10日

我们将发布一项新技能，即Workfront Planning解决方案架构师，该技能将Workfront Planning的代理式最佳实践指导直接带入克劳德：

* **配置**&#x200B;要规范的新Planning工作区，Workfront MCP服务器在您的环境中执行安装程序。
* **审核**&#x200B;大规模反模式的现有配置。
* **根据建议的限制（记录、连接、层次结构深度）检查使用情况**。
* **随时询问有关Planning的问题**。

除了初始设置外，该技能还通过以下方式支持日常管理：在配置漂移引发摩擦之前捕获配置漂移，在接近限制成为阻滞器之前标记这些限制，在每个工作区中强制实施一致的标准，无论配置者是谁，以及为团队中的任何成员提供准确的答案，而无需等待专家。 总体而言，这涵盖了正确设置工作区并随着使用量增长保持该工作区的整个生命周期。

有关信息，请参阅[可用于直接安装的技能](/help/quicksilver/workfront-basics/workfront-mcp-server/direct-skills.md)。

## 在表格视图中拖放行

>[!NOTE]
>
>预览： 2026年7月30日
>生产快速发布： 2026年8月13日
>全部生产： 2026年10月15日

在表视图中拖放行的体验在视觉上得到了改进。

有关信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。


## 从属已连接记录字段

>[!NOTE]
>
>预览： 2026年7月30日
>生产快速发布： 2026年8月13日
>适用于所有人的生产： 2026年10月15日

Workspace Manager现在可以定义连接的记录类型之间的依赖关系。 例如，确保区域字段仅显示与选定地理位置关联的值。 这直接在连接字段设置中配置：当将连接从地域记录类型添加到从属记录类型（如区域）时，新设置允许工作区管理员使用在这些记录类型之间已建立的关系将其标记为从属地域记录类型。

配置完毕后，任何引用这两个字段（例如营销策划）的记录类型都会立即看到效果：选择地域值会将“区域”选取器缩小为仅包含那些实际链接到该地域的地区。 这会自动实施记录结构，从而消除不匹配的组合并减少手动清理。

此更新包括以下功能：

* 在连接记录类型时，我们在“新建连接”选项卡中添加了新的连接设置部分
* 我们已在新部分中添加了“使此连接依赖于”设置


有关信息，请参阅[管理从属连接](/help/quicksilver/planning/architecture/manage-dependent-connections.md)。




## 在表格视图中显示记录的新注释指示符

>[!NOTE]
>
>预览： 2026年7月30日
>生产快速发布： 2026年8月13日
>适用于所有人的生产： 2026年10月15日

我们添加了一个新指示器，当记录中存在未读注释时会显示该指示器。 指示器显示在表视图中记录的主字段的右上角。

有关详细信息，请参阅[管理记录注释](/help/quicksilver/planning/records/manage-record-comments.md)。

## 可定制的记录颜色和基于连接的颜色编码

>[!NOTE]
> 
>预览： 2026年7月23日
>生产快速发布： 2026年8月13日
>全部生产： 2026年10月15日

记录现在支持可自定义的调色板，这使您能够将自动分配给新记录的颜色更新为标准或自定义颜色。

此增强功能中包含以下更改： 

* 我们在以下区域添加了“颜色”选项：
  * 表格视图中的字段图标。 
  * 时间轴和日历视图的“设置”区域中的“条形图样式”部分

    当“颜色”设置打开时，指定给新记录的颜色将显示在这些视图中记录显示的所有位置。 

* 颜色圆圈将添加到记录的“详细信息”页面。 
* 当按字段值着色时，您现在可以将单选、多选和连接的记录字段添加到时间轴和日历视图中条块的颜色编码中。 
* 在创建连接的记录字段时，除了记录名称和图像外，您还可以启用显示颜色。 
* 设置区域中的“颜色”部分也通过删除“无”选项进行了简化。  

有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。 

## 规划Designer现在需要接受Beta协议

>[!NOTE]
>面向所有客户的预览和生产： 2026年7月20日
>[!BADGE 超出计划]{type=Neutral}

现在，规划Designer需要使用已接受的Beta协议。 您的公司不需要签署AI协议。 这适用于所有客户。

为此，我们已将设置部分中的规划Designer选项移动到选择加入人工智能测试版部分下。

现在，在启动工作区生成器之前，如果没有已接受的Beta协议，则启动计划Designer时将会提示您接受接受接受协议。

有关信息，请参阅[Adobe Workfront规划Designer入门](/help/quicksilver/planning/general/planning-ai-designer.md)。
