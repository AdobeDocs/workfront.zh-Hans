---
content-type: release-notes
keywords: 注释，每季，更新
navigation-topic: product-releases
title: 21.1其他增强功能
description: 本页介绍了在21.1版本中对“预览”环境进行的所有其他增强。 这些增强功能将在2021年2月15日这一周的“生产”环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# 21.1其他增强功能

本页介绍了在21.1版本中对“预览”环境进行的所有其他增强。 这些增强功能将在2021年2月15日这一周的“生产”环境中提供。

有关21.1版本的所有可用更改列表，请参阅[21.1版本概述](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md)。

## 更新了事件订阅失败要求

我们正在更新事件订阅失败的软禁用要求。 除了现有要求之外，如果事件订阅在2000次尝试中未能成功交付，现在将软禁用。 这是为了强化现有的70%失效规则，在某些情况下这可能导致过量的失效。

此外，我们将从2021年2月起添加硬禁用要求。

有关新的软禁用和硬禁用要求的更多信息，请参阅[常见问题解答 — 事件订阅](../../../wf-api/general/event-subs-faq.md)。

## 可用于《每日摘要》的新团队字段

我们已在“需要执行的操作每日摘要”电子邮件中添加了“团队批准”和“工作分配”字段。

有关详细信息，请参阅[通知：需要操作](../../../workfront-basics/using-notifications/notifications-action-needed.md)。

## 替换请求队列中的POP电子邮件选项

我们正在将请求队列的POP电子邮件选项替换为新的Workfront托管系统。 您仍可以通过电子邮件提交请求，但您需要在“请求队列”区域中设置一个新的Adobe Workfront管理的电子邮件地址。

这些更改可在“预览”中测试。

在所有预览环境中自动禁用电子邮件。 要启用电子邮件以进行测试，请参阅[从预览Sandbox环境启用电子邮件投放](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)。

有关详细信息，请参阅[允许用户通过电子邮件将问题发送到请求队列项目](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md)。

有关我们为什么要进行此更改的详细信息，请参阅[新的Adobe Workfront托管系统使用21.1](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md)替换请求队列的POP电子邮件。

此功能现已包含在Workfront One上的新Workfront Experience[&#128279;](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home)学习路径的队列管理中。

## 限制工时表上的小时编辑

为了更好地控制时间表和小时编辑，我们添加了一个设置，该设置允许您限制对时间表所有者和系统管理员进行小时编辑。

以前，在访问级别中启用了时间表和小时选项的用户可以编辑任何时间表上的小时。

有关详细信息，请参阅[配置工时表和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。

## 改进了时间表区域中的过滤器和视图

在将项目、任务或问题添加到时间表时，我们添加了以下改进：

* 筛选器：我们为项目和问题添加了筛选器。 单击更多选项以查看这些过滤器。 以前，只有“任务”才有可用的筛选。
* 视图：我们向搜索页面添加了视图和分组选项。

有关详细信息，请参阅[记录时间](../../../timesheets/create-and-manage-timesheets/log-time.md)。

## 隐藏工时表中的加班框

现在，如果不跟踪Workfront中的加班情况，则可以隐藏加班框，以免造成用户混淆。 您可以为一次性使用的时间表或时间表配置文件隐藏超时框：

* 一次性时间表：如果您选择隐藏单个时间表中的超时框，则它仅对该时间表隐藏。 有关详细信息，请参阅[创建一次性时间表](../../../timesheets/create-and-manage-timesheets/create-tmshts.md)。
* 时间表配置文件：如果您选择隐藏时间表配置文件中的超时框，则将来为分配给该配置文件的用户创建的所有时间表都将看不到超时框。 有关详细信息，请参阅[创建、编辑和分配时间表配置文件](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。

以前，无法在时间表上隐藏超时框。

## 在痕迹导航中展开或折叠项目

为了更便于查看完整的痕迹导航路径，我们添加了展开和折叠功能。

现在，任何截断的项目都会在项目之前进行分组，并带有文本“更多”。 例如，“另外3个”表示有3个对象未显示。

以前，必须单击省略号才能在下拉菜单中显示任何截断的对象。

要查看痕迹导航中的所有项目，请单击痕迹导航开头的“更多”以展开这些项目。 展开后，您可以单击“更少”以再次折叠这些项目。

## 痕迹导航的新外观

为了帮助用户更好地识别他们在Workfront中的位置以及更轻松地在对象之间导航，我们对痕迹导航进行了以下改进：

* 现在，痕迹导航中的每个项目都包含一个对象标签。
* 当前页面现已包含在痕迹导航中，并且为斜体。
* 键盘导航和屏幕阅读器导航现在可用于痕迹导航。
* 其他次要样式更改

