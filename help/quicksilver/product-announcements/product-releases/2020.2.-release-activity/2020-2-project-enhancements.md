---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2项目增强功能
description: 本页介绍了2020.2版本对生产环境的所有项目增强。 这些增强功能在2020年5月11日这一周的生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 150bc838-d6a5-445a-af77-62c4ed74dd1b
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# 2020.2项目增强功能

本页介绍了2020.2版本对生产环境的所有项目增强。 这些增强功能在2020年5月11日这一周的生产环境中提供。

有关2020.2版本可用的所有更改列表，请参阅[2020.2版本概述](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md)。

## 对于Workfront管理员：当新项目的项目状态为隐藏或解锁时，新增故障保护

在设置中，您可以配置首选项，以确保在创建项目时，每个新项目都具有特定状态。 这一点很重要，因为项目始终需要状态才能在Workfront中正常运行，即使该项目是全新项目。

为确保新项目始终具有状态，即使管理员隐藏或解锁为新项目配置的状态，系统现在也会将状态列表中的第一个状态分配给所有新项目，直到您再次为新项目配置新状态为止。

有关设置所有新项目状态的首选项的信息，请参阅[配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)(或者，如果您使用的是Adobe Workfront Classic，请参阅[设置项目首选项](https://experienceleague.adobe.com/zh-hans/docs/workfront/using/home))。

**在以下环境中可用：**

* Adobe Workfront Classic
* 新的Adobe Workfront体验

## 对于Workfront管理员：改进了项目偏好设置中的设计

现在，设置项目首选项的体验更加直观且易于使用：

* 标题比选项标签大，因此您可以更快地找到您要找的内容。
* 使用分线和额外空格分隔每个部分，以便您更轻松地专注于正在执行的操作。
* 如果为选项（如“每个工作日的典型小时数”）键入无效数字，则在单击“保存”后，将立即显示警告消息，而不是显示警告消息。
* 选项标签与Workfront中其他位置的相应界面文本匹配，例如详细信息区域和报表。

有关“项目首选项”区域的信息，请参阅[配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)(或者如果您使用的是Adobe Workfront Classic，请参阅[设置项目首选项](https://experienceleague.adobe.com/zh-hans/docs/workfront/using/home))。

**在以下环境中可用：**

* Adobe Workfront Classic
* 新的Adobe Workfront体验

## 选定的筛选器、视图和分组保留在报表列表中

现在，即使用户注销并重新登录Workfront，也会选择应用于特定报表的最后一个过滤器、视图或分组。

以前，当用户将筛选器、视图或分组应用于报告列表，然后导航离开该页面后，默认筛选器、视图或分组在用户下次导航到同一报告时显示。

**在以下环境中可用：**

* 新的Adobe Workfront体验
* Adobe Workfront Classic

## 将任务移动并复制到另一个项目会保留任务限制，当任务可以适应项目的时间表时

当您复制任务或将其移动到其他项目时，我们对Workfront处理任务的特定日期任务限制的方式进行了改进。 特定日期的任务约束的示例包括“必须开始于”、“必须完成于”、“固定日期”、“开始时间不晚于”等。

例如，当您将具有“必须开始于”限制的任务移动或复制到其“计划开始日期”早于任务的“开始日期”的另一个项目时，任务会在复制或移动后保留该限制。 当您将具有必须开始日期限制的任务移动或复制到其计划开始日期在任务开始日期之后的项目时，任务限制会尽快变为。

在此更改之前，任务限制始终会尽快更改为。

有关移动任务的信息，请参阅[移动任务](../../../manage-work/tasks/manage-tasks/move-tasks.md)(或者如果您使用的是Adobe Workfront Classic，请参阅[移动任务](https://experienceleague.adobe.com/zh-hans/docs/workfront/using/home))。

有关复制任务的信息，请参阅[复制和复制任务](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)(或者，如果您使用的是Adobe Workfront Classic，请参阅[复制和复制任务](https://experienceleague.adobe.com/zh-hans/docs/workfront/using/home))。

有关所有任务限制的概述，请参阅[任务限制概述](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (或者，如果您使用的是Adobe Workfront Classic，请参阅[任务限制概述](https://experienceleague.adobe.com/zh-hans/docs/workfront/using/home))。

**在以下环境中可用：**

* Adobe Workfront Classic
* 新的Adobe Workfront体验

## 在“详细信息”选项卡或任务列表中进行更改时防止数据丢失

为了防止在手动保存更改时更新项目级别任务列表中的对象或任务的“详细信息”页面上的信息时丢失数据，现在会显示一条警告消息，在您尝试编辑标题中的信息之前通知您有未保存的更改。 在保存更改之前，只允许订阅对象或将对象添加到收藏夹。

有关编辑列表中的任务的信息，请参阅[编辑列表中的任务](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**在以下环境中可用：**

* 新的Adobe Workfront体验

