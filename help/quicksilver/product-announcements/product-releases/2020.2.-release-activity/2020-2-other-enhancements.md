---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2年其他增强功能
description: 本页介绍了2020.2版本对生产环境的所有其他增强功能。 这些增强功能在2020年5月11日这一周的生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 46ed705e-b966-4ae9-a602-a5a73a3de3aa
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# 2020.2年其他增强功能

本页介绍了2020.2版本对生产环境的所有其他增强功能。 这些增强功能在2020年5月11日这一周的生产环境中提供。

有关2020.2版本可用的所有更改列表，请参阅 [2020.2版概述](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## 对于Workfront管理员：在Workfront Classic中创建的较新布局模板现在可在新的Workfront Experience中获取

现在，新的Workfront Experience中提供了2019年秋季之后在Workfront Classic中创建的布局模板。 最好在新的Workfront Experience中更新这些布局模板，以便利用新功能，并尽可能让新功能对该环境中的用户有用。

有关更多信息，请参阅 [布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

**在以下环境中可用：**

* 新的Adobe Workfront体验

## 特定于组的批准流程适用于所有对象

要充分利用特定于组的审批流程，您现在可以在编辑这些对象时将其添加到任务、问题和项目。

在项目上配置请求队列或队列主题时，您也可以自动将特定于组的批准流程附加到“编辑项目”框的“任务”区域中的任务以及问题。

有关将审批流程添加到项目、任务和问题的信息，请参阅以下文章：

* [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)
* [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [编辑问题](../../../manage-work/issues/manage-issues/edit-issues.md)
* [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
* [创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)

## 使用自定义状态为组创建批准流程

为了更便于组管理自己的独特工作流，您现在可以在审批流程中使用特定于组的自定义状态。

以前，组无法将其自身的自定义状态用于其特定于组的审批流程。 只有系统范围状态可用，并且这些状态并不总是适合组审批流程。

现在，可在一次性审批流程和系统范围审批流程中使用自定义状态：

* 为对象（项目、任务或问题）创建一次性审批流程，并将其基于与处理该对象的组相关联的状态。 这包括与该组关联的任何自定义状态。
* 创建一个全局审批流程，使其仅适用于该组或系统中的每个人。

对于对批准流程具有管理访问权限的用户，有关配置批准流程的信息，请参阅 [创建工作项的审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (或者，如果您使用的是Adobe Workfront Classic，请参阅 [创建批准流程](https://one.workfront.com/s/article/Creating-Approval-Processes-1001577410))。

对于用户，有关将审批流程与工作项关联的信息，请参阅 [将新的或现有的审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (或者，如果您使用的是Adobe Workfront Classic，请参阅 [将新的或现有的审批流程与工作相关联](https://one.workfront.com/s/article/Associating-a-New-or-Existing-Approval-Process-with-Work-708455630))。

**在以下环境中可用：**

* Adobe Workfront Classic
* 新的Adobe Workfront体验

## 用于搜索的新覆盖页面

为了使用户能够在新的Workfront Experience中更轻松地在搜索页面和之前的页面之间来回导航，我们添加了一个部分覆盖屏幕的搜索叠加页面。

现在，当您在“搜索”菜单中单击“高级搜索”或执行基本搜索时，页面幻灯片将从屏幕右侧打开。

有关更多信息，请参阅 [搜索Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

**在以下环境中可用：**

* 新的Adobe Workfront体验

## 活动订阅的更新

为了更好地使用户能够分类、排除故障和解决问题，我们修改了行为并向事件订阅API添加了更多数据。 我们还进行了以下更改：

* 迁移了底层消息传递技术
* 重新构建服务，减少复杂的依赖关系，从而更有效地扩展
* 改进了监控和警报

要了解更多信息，请参阅 [常见问题解答 — 活动订阅](../../../wf-api/general/event-subs-faq.md) 和 [事件订阅最佳实践](../../../wf-api/general/event-sub-best-practice.md).
