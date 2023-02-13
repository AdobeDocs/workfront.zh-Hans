---
content-type: release-notes
keywords: 注释，季度，更新，发行
navigation-topic: 2021-2-release-activity
title: 21. 2报表增强功能
description: 本页介绍了在“预览”环境的21.2版本中所做的所有报表增强功能。 这些增强功能将于2021年5月10日这一周的生产环境中提供。 有关21.2版本中可用的所有更改的列表，请参阅21.2版本概述。
author: Luke
feature: Product Announcements
exl-id: 1d5f76ef-bea7-4630-8051-454b0d109341
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---

# 21. 2报表增强功能

本页介绍了在“预览”环境的21.2版本中所做的所有报表增强功能。 这些增强功能将于2021年5月10日这一周的生产环境中提供。 有关21.2版本中可用的所有更改的列表，请参阅 [21.2版本概述](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## 限制在项目和报表中进行小时编辑

为了在项目和小时报表的“小时”选项卡上对小时编辑提供更多控制，我们添加了一个设置，允许Workfront管理员将小时编辑限制为小时所有者和系统管理员。

以前，在访问级别启用工时单和工时的用户可以编辑工时。

有关更多信息，请参阅 [配置工时单和工时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## 更新列表和报表中“工作总揽”字段的新外观

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用。

为了与新Workfront体验中其他区域的现代外观相匹配，更新列表和报表中“工作总揽”字段的样式已发生更改。 这项重新设计包括：

* 用户配置文件图片、工作角色和团队的四舍五入头像
* 为没有个人资料图片的用户显示缩写
* 新的“作业”角色图标
* 高级分配的新“人员”图标
* 新的“受限访问”图标
* 其他次要设计更改

有关列表中分配的详细信息，请参阅 [分配任务](../../../manage-work/tasks/assign-tasks/assign-tasks.md) 或 [分配问题](../../../manage-work/issues/manage-issues/assign-issues.md).

![](assets/assignments-updates-350x193.png)

## 更新的列表和报表中提前键入字段的新外观

>[!NOTE]
>
>2021年5月20日从生产环境中临时删除。

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用。

为了与新Workfront体验中其他区域的现代外观相匹配，更新列表和报表中的类型字段的样式已发生更改。 这些更改包括：

* 已从字段中删除Typeahead图标。
* 现在，当您单击提前键入字段时，会在输入文本之前显示建议菜单。
* 建议菜单对值长度的响应更灵敏，现在，当满足字符限制时，这些值会在末尾被截断，而不是在值的中间。

有关更新列表的信息，请参阅 [更新列表与旧版列表之间的差异](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) 章节 [开始使用Adobe Workfront中的列表](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

![](assets/typeahead-updates-350x336.png)

## 系统更新报告

新的“日记帐分录”报表允许您深入查看系统更新，从而为您提供更强的可审计性，包括：

* 项目、任务或问题的状态更改
* 已删除的任务或问题
* 自定义字段中的值
* 计划完成日期
* 项目所有者更改

例如，您可以设置此报表来显示特定自定义字段周围的活动，包括自定义字段的项目、首次输入值时、该值是什么、字段更新时、上一个值是什么、新输入的值是什么、用户完成了这些操作等。

以前，您只能通过Workfront API报告系统更新。

要进一步了解此报表以及可用于什么用途，请参阅 [报告更新区域](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

