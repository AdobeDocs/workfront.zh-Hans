---
content-type: release-notes
keywords: 注释，季度，更新
navigation-topic: product-releases
title: 21.1其他增强功能
description: 本页介绍21.1版本到“预览”环境的所有其他增强功能。 这些增强功能将于2021年2月15日这一周的生产环境中提供。
author: Luke
feature: Product Announcements
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# 21.1其他增强功能

本页介绍21.1版本到“预览”环境的所有其他增强功能。 这些增强功能将于2021年2月15日这一周的生产环境中提供。

有关21.1版本中可用的所有更改的列表，请参阅 [21.1版本概述](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## 更新了事件订阅失败要求

我们正在更新“事件订阅”失败的软禁用要求。 除了现有要求外，如果“事件订阅”在2000次尝试内未能成功交付，则现在将软性禁用它们。 这是为了加强现有的70%失败规则，在某些情况下，这一规则可能导致过多的失败。

此外，我们将从2021年2月起添加硬禁用要求。

有关新的软禁用和硬禁用要求的其他信息，请参阅 [常见问题解答 — 事件订阅](../../../wf-api/general/event-subs-faq.md).

## “每日摘要”中提供的新团队字段

我们在“需要的每日摘要操作”电子邮件中添加了“团队批准”和“分配”字段。

有关更多信息，请参阅 [通知：所需操作](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## 替换请求队列中的POP电子邮件选项

我们正在将请求队列的POP电子邮件选项替换为新的Workfront管理系统。 您仍可以通过电子邮件提交请求，但是您需要在“请求队列”区域设置一个由Adobe Workfront管理的新电子邮件地址。

这些更改可在“预览”中测试。

在所有“预览”环境中，电子邮件都会自动禁用。 要启用电子邮件以进行测试，请参阅 [允许从预览沙盒环境发送电子邮件](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

有关更多信息，请参阅 [允许用户将问题通过电子邮件发送到请求队列项目](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

有关我们为何进行此更改的更多信息，请参阅 [新的Adobe Workfront托管系统将请求队列的POP电子邮件替换为21.1](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

此功能现在包含在 [新Workfront体验中的队列管理](https://one.workfront.com/s/learningpath4/queue-management-MCYCJRWK36QZBP7PGMNDMSPRN3LE) 学习Workfront一号。

## 限制对工时单的时间编辑

为了更好地控制工时单和工时编辑，我们添加了一个设置，允许您将工时编辑限制在工时单所有者和系统管理员。

以前，在其访问级别中启用“工时单和工时”选项的用户可以编辑任何工时单上的工时。

有关更多信息，请参阅 [配置工时单和工时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## 改进了“工时单”区域中的过滤器和视图

在将项目、任务或问题添加到工时单时，我们添加了以下改进：

* 过滤器：我们为项目和问题添加了过滤器。 单击更多选项可查看这些过滤器。 以前，只有“任务”具有可用的过滤功能。
* 视图：我们在“搜索”(Search)页面中添加了“查看”(View)和“分组”(Grouping)选项。

有关更多信息，请参阅 [日志时间](../../../timesheets/create-and-manage-timesheets/log-time.md).

## 在工时单中隐藏超时框

现在，如果您不在Workfront中跟踪超时，则可以隐藏超时框以缓解用户混淆。 您可以隐藏一次性使用的工时单或工时单配置文件的超时框：

* 一次性工时单：如果选择隐藏单个工时单中的超时框，则仅对该工时单隐藏该超时框。 有关更多信息，请参阅 [创建一次性工时单](../../../timesheets/create-and-manage-timesheets/create-tmshts.md).
* 时间表配置文件：如果选择隐藏时间表配置文件中的超时框，则为分配给该配置文件的用户创建的所有未来时间表将看不到超时框。 有关更多信息，请参阅 [创建、编辑和分配工时单配置文件](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

以前，无法隐藏工时单上的超时框。

## 在痕迹导航导航中展开或折叠项目

为了更便于查看完整的痕迹导航路径，我们添加了展开和折叠功能。

现在，任何已截断的项目都会在项目之前分组，并包含文本“更多”。 例如，“3个以上”表示有3个对象未显示。

以前，您必须单击省略号才能在下拉菜单中显示任何截断的对象。

要查看痕迹导航中的所有项目，请在痕迹导航开头单击“更多”以展开这些项目。 展开后，您可以单击“更少”再次折叠项目。

## 痕迹导航的新外观

为帮助用户更好地识别他们在Workfront中的位置以及更轻松地在对象之间导航，我们对痕迹导航进行了以下改进：

* 痕迹导航中的每个项目现在都包含一个对象标签。
* 当前页面现在包含在痕迹导航中，且为斜体。
* 现在，可以为痕迹导航使用键盘导航和屏幕阅读器导航。
* 其他次要样式更改

