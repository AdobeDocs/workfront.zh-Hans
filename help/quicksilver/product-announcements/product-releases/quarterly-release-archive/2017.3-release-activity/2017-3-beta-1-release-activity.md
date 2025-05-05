---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta 1发行版活动
description: 本页介绍了2017.3版的“预览”环境中最近提供的所有更改。 此页面上的功能已于2017年8月9日在预览环境中提供。 该版本将于2017年11月初在“生产”环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 33a91c25-98ec-4f08-b444-4e11e05e464b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---

# 2017.3 Beta 1发行版活动

本页介绍了2017.3版的“预览”环境中最近提供的所有更改。 此页面上的功能已于2017年8月9日在预览环境中提供。 该版本将于2017年11月初在“生产”环境中提供。

>[!IMPORTANT]
>
> 此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2017.3版中所做所有更改的列表，请参阅  [2017.3发布活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md)。

2017.3 Beta 1版本包含面向Workfront管理员和其他用户的增强功能：

管理员的&#x200B;**：**

* [阻止在记录小时数时删除任务和问题](#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged)
* [从设置区域删除“提前访问”设置](#removal-of-the-early-access-setting-from-the-setup-area)
* [Workfront默认电子邮件地址更改](#workfront-default-email-address-change)

所有用户&#x200B;**：**

* [资源计划改进](#resource-scheduling-improvements)
* [宽屏显示器](#widescreen-display)
* [调整报告和列表中的列大小并重新排序](#resize-and-reorder-columns-in-reports-and-lists)
* 复制任务和问题时[清除自定义数据选项](#clear-custom-data-option-when-copying-tasks-and-issues)
* [直接从模板创建项目](#create-a-project-directly-from-a-template)
* 订阅对象的[应用程序内通知](#in-app-notification-for-subscribed-objects)
* @Tagging0&rbrace;当前在预览环境中不可用[&#128279;](#tagging-currently-not-available-in-the-preview-environment)
* [在项目的利用率报告中包括用户分配信息](#include-user-allocation-information-in-the-utilization-report-on-a-project)

## 资源计划改进 {#resource-scheduling-improvements}

>[!NOTE]
>
>在23.1版本中，资源计划工具已弃用并从Workfront中删除。 有关使用工作负载均衡器计划资源的信息，请参阅[工作负载均衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

在为团队、项目或以资源管理器身份为多个项目计划资源时，可以使用以下资源计划改进：

* [以全屏模式查看计划区域](#view-scheduling-area-in-full-screen-mode)
* [查看资源计划区域的更多日期范围选项](#more-date-range-options-for-viewing-the-resource-scheduling-area)
* [在计划时间线上查看预计日期](#view-projected-dates-on-the-scheduling-timeline)

### 以全屏模式查看计划区域 {#view-scheduling-area-in-full-screen-mode}

您可以在全屏模式下查看计划时间线，从而可以在单个视图中查看更多信息。 

有关详细信息，请参阅“开始使用资源计划”。

### 查看资源计划区域的更多日期范围选项 {#more-date-range-options-for-viewing-the-resource-scheduling-area}

查看计划时间线时，您可以查看以下附加日期范围选项：

* 单日查看
* 4周查看
* 6周查看

在此更改之前，您只能在1周、2周或3周的视图中查看计划时间线。 除了新日期范围之外，这些日期范围仍然可用。

在一天视图中查看计划时间表时，无法显示用户分配（包括每日总小时数）。

有关详细信息，请参阅“开始使用资源计划”。

### 在计划时间线上查看预计日期 {#view-projected-dates-on-the-scheduling-timeline}

现在，您可以为任务和问题配置计划时间线以显示预计日期，而不是计划日期。 

在此更改之前，计划时间线上的任务和问题仅显示计划日期。

在计划时间线上查看预计日期时，无法显示用户分配（包括每日总小时数）。

有关详细信息，请参阅“开始使用资源计划”。

## 宽屏显示器 {#widescreen-display}

在Workfront中显示以下任何对象时，将自动填充整个浏览器窗口：

* 项目
* 任务
* 问题
* 报告
* 仪表板
* 日程表

在此更改之前，显示区域的两侧各有两个白色边栏。 现在，宽屏视图会动态调整到屏幕和浏览器窗口的宽度。

## 在报表和列表中调整列的大小和重新排序 {#resize-and-reorder-columns-in-reports-and-lists}

您现在可以重新排序报告或列表中的列并调整其大小，而无需编辑报告。 (今年早些时候，随着早期访问环境的弃用，此功能被删除。 目前正在重新引入。)

此功能不适用于仪表板列表或报表，因为这些列表已在新的数据网格结构中重新设计。 所有其他列表都将在此版本中启用此功能。

有关调整列大小和重新排序列的详细信息，请参阅[修改列宽和顺序](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)。

## 复制任务和问题时清除自定义数据选项 {#clear-custom-data-option-when-copying-tasks-and-issues}

在复制任务或问题时，您现在可以选择用于清除任何自定义数据的选项。 当您选择清除任务或问题的自定义数据时，表单会复制到新项目，但表单上的自定义数据不会。 清除自定义数据也会影响附加到附加到项目的文档的自定义表单，或附加到任务支出的自定义表单。

在此更改之前，当您复制任务或问题时，自定义表单中包含的自定义数据也会复制到新项目。 

有关复制任务的详细信息，请参阅[复制和复制任务](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

有关复制问题的详细信息，请参阅[复制问题](../../../../manage-work/issues/manage-issues/copy-issues.md)。

## 直接从模板创建项目 {#create-a-project-directly-from-a-template}

您现在可以从模板级别创建项目。

在此更改之前，您只能在Workfront的“项目”区域的“项目”选项卡上，使用&#x200B;**通过模板新建项目**&#x200B;选项，从模板创建项目。

有关从模板创建项目的详细信息，请参阅[使用模板创建项目](../../../../manage-work/projects/create-projects/create-project-from-template.md)。

## 在记录小时数时防止删除任务和问题 {#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged}

您现在可以将Workfront配置为允许或阻止删除记录了小时数的任务和问题。

在此更改之前，当您删除记录了小时数的任务或问题时，小时数随任务或问题一起删除，或者被移动到项目，具体取决于您的时间表和小时数首选项。

有关删除任务的详细信息，请参阅[删除任务](../../../../manage-work/tasks/manage-tasks/delete-tasks.md)。

有关删除问题的详细信息，请参阅[删除问题](../../../../manage-work/issues/manage-issues/delete-issues.md)。

有关启用任务和问题删除的系统设置的详细信息，请参阅[配置系统范围的任务和问题首选项](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

## 从设置区域删除“提前访问”设置 {#removal-of-the-early-access-setting-from-the-setup-area}

我们正在删除允许Workfront管理员注册用户以参与提前访问环境的设置。 自2016年底以来，此功能已被弃用。 我们尚未在2017年发布任何用于抢先访问的新功能，该环境中保留的所有功能都已移至生产环境。

在此更改之前，尽管没有要访问的新功能，Workfront管理员仍可以将用户添加到早期访问环境。

## Workfront默认电子邮件地址更改 {#workfront-default-email-address-change}

Workfront传出邮件的默认电子邮件地址已从[noreply@attask.com](mailto:noreply@attask.com)更改为[noreply@my.workfront.com](mailto:noreply@workfront.com)。

如果您当前过滤来自Workfront的电子邮件，则需要更改过滤器以反映新的默认地址。 

默认地址的更改对配置的Workfront电子邮件地址没有影响。 

有关更多信息，请参阅。

## 订阅对象的应用程序内通知 {#in-app-notification-for-subscribed-objects}

现在，当用户对您订阅的项目、任务和问题发表评论时，您会收到应用程序内通知。 若要了解有关订阅应用程序内通知的更多信息，请参阅[查看和管理应用程序内通知](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)。

根据Workfront管理员启用的功能，您还可以接收订阅项目的电子邮件通知。 您可以通过订阅电子邮件上的链接轻松取消订阅项目，如[Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md)中所述。

在此更改之前，您始终会收到订阅项目的电子邮件通知，并且没有接收应用程序内通知的选项。

虽然您可以禁用订阅电子邮件，但无法禁用订阅项目的应用程序内通知。 有关详细信息，请参阅[为系统中的每个人配置事件通知](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。

要了解有关订阅项目的更多信息，请参阅[在Adobe Workfront中订阅项目](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)。

## @Tagging在预览环境中当前不可用 {#tagging-currently-not-available-in-the-preview-environment}

在我们努力将富文本格式功能引入更新流时，您将暂时无法使用@符号在更新流中为预览环境中的以下对象标记其他用户：

* 项目
* 任务
* 问题
* 时间表

您仍然可以通过单击&#x200B;**将其他人包含在此更新中**&#x200B;图标来标记其他人。

有关详细信息，请参阅[为其他人标记更新](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)。

## 在项目的利用率报告中包括用户分配信息 {#include-user-allocation-information-in-the-utilization-report-on-a-project}

>[!NOTE]
>
>在23.1版本中，资源计划工具已弃用并从Workfront中删除。 有关使用工作负载均衡器计划资源的信息，请参阅[工作负载均衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

项目的利用率报告现在会考虑是否在任务持续期间重新分配了计划小时数。 修改小时用户分配（如“在计划区域中管理用户分配”中所述）后，如果在利用率报表中选择的日期只包含任务的一部分，则利用率报表中的数据可能会受到影响。

有关详细信息，请参阅[资源利用率报告概述](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。
