---
content-type: overview
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 日历报表概述
description: 日历报告实际上是一种动态报告，它提供了工作的可视化表示形式。
author: Lisa
feature: Reports and Dashboards
exl-id: c65cf8ab-e37f-42a4-9a81-70962629e9ba
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 1%

---

# 日历报表概述

日历报告实际上是一种动态报告，它提供了工作的可视化表示形式。 您可以在日历报表中显示以下对象的日期信息：

* 任务
* 问题
* 项目

您在中访问日历报表的能力 [!DNL Adobe Workfront] 由以下各项决定 [!DNL Workfront] 管理员。 有关查看日历报表所需的访问级别的详细信息，请参阅 [授予对报告、功能板和日历的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## 创建您自己的日历

[!UICONTROL Workfront] 在以下情况下，自动创建默认个人日历：

* 无权访问任何其他日历的新创建用户首次访问日历报告页面\
   或
* 用户手动删除所有日历，并且无权访问任何其他日历

>[!NOTE]
>
>如果用户有权访问任何其他日历，例如系统范围的共享日历或专门与用户共享的日历，则不会创建个人日历。

此外，用户可以创建日历并访问其他用户与其共享的日历。 在Workfront中，用户可以访问的日历数量没有限制。

>[!NOTE]
>
>您必须拥有 [!UICONTROL 编辑] 访问 [!UICONTROL 报表]， [!UICONTROL 仪表板]、和 [!UICONTROL 日历] 创建日历报表的访问级别。 联系 [!DNL Workfront] 管理员。

## 按日期对项目分组

在每个日历报表中，您可以创建项目组，以缩小日历的焦点。 例如，您可以有一个日历分组，用于显示特定项目上所有任务的日期、当前处理该项目的营销团队成员，以及分配给项目团队的逾期问题。 有关更多信息，请参阅以下文章：

* [使用 [!UICONTROL 计划日期] 在日历报表中](../../../reports-and-dashboards/reports/calendars/use-planned-dates.md)
* [使用 [!UICONTROL 预计日期] 在日历报表中](../../../reports-and-dashboards/reports/calendars/use-projected-dates.md)
* [在日历报告中使用自定义日期字段](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md)

>[!NOTE]
>
>如果您在运行日历报表时看到504错误，则可能是报表中的过滤器太多。 减少过滤器数量应该有助于报表运行。

## 将日历添加到功能板

通过在功能板上显示日历报表，您可以快速访问这些报表。 要了解如何将日历添加到仪表板，请参阅 [编辑功能板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md).
