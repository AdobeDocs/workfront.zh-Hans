---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1预览3
description: 本页介绍R1.3版本在“预览”环境中可用的所有更改。 此页面上的功能已于2017年2月1日在预览环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1347'
ht-degree: 2%

---

# R1预览3

本页介绍R1.3版本在“预览”环境中可用的所有更改。 此页面上的功能已于2017年2月1日在预览环境中提供。

有关在R1中所做所有更改的列表，请参见 [R1发布活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## 链接外部文件的改进方法

现在，链接来自外部源的文档(如Google Drive、Box、Dropbox等)的选项位于“文档”区域中更显眼的位置。 

此外，在首次链接来自文档提供程序的文件之前对该提供程序进行授权的操作现在更直观了（这只是从外部提供程序链接文件时的额外步骤）。

在这些更改之前，从外部源链接文件的选项位于“文档”区域的“添加文档”对话框中。 在首次从外部源链接文档之前，链接文档的用户必须在“设置”区域中授权该文档提供商。

有关更多信息，请参阅  [链接来自外部应用程序的文档](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## 已更新团队正在处理日历

>[!NOTE]
>
>在23.1版本中，资源计划工具已弃用并从Workfront中删除。 有关使用工作负载均衡器调度资源的信息，请参阅 [工作负载均衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

适用于团队的“正在处理”日历现在包含附加功能和更新的外观。 处理日历的团队现在的工作方式类似于项目的资源计划工具。

更新后的团队正在处理日程表包括以下改进：

* 按字母顺序查看用户或按角色分组用户。
* 按项目优先级、状态和单个项目筛选计划时间线。 您还可以按角色和用户筛选计划时间线。 （在为项目计划资源时，“筛选器”区域包含的选项比少。）
* 将问题包含在计划时间表中。
* 显示用户分配并修改每天用户分配给某些任务和问题的小时数。
* 查看指示器，以显示在任何给定日期用户过度分配的时间。
* 配置是否将已完成的工作显示在计划时间线上。

在计划项目的资源时与资源计划工具的区别：

* 所有团队成员都显示在团队正在处理的日历中。\
  在计划项目的资源时，仅显示其关联角色与“未分配”区域中一个或多个任务的角色匹配的用户。
* “交换”工具不可用，未包括在团队处理日历中。
* 任何团队成员都可以对团队处理日历进行更改。\
  在计划项目的资源时，只有资源经理才能为项目做出资源决策。
* 默认情况下，问题显示在处理日程表的团队中。\
  在计划项目的资源时，默认情况下不显示问题。

有关使用更新后的团队处理日程表的详细信息，请参阅“资源计划”。

## 资源计划增强功能

计划时间线包括以下增强功能：

* “使用过滤器控制在计划时间轴上显示的用户”
* “用户在被分配任务后保持时间线上”

### 使用筛选器可控制要在计划时间线上显示的用户 {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

>[!NOTE]
>
>在23.1版本中，资源计划工具已弃用并从Workfront中删除。 有关使用工作负载均衡器调度资源的信息，请参阅 [工作负载均衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

筛选器现在可用于控制在计划时间线上显示哪些用户，以及哪些任务和问题显示在“未分配”区域中。 在筛选器中选择用户后，仅显示您选择的用户，无论这些用户是否具有与“未分配”区域中任务的角色分配匹配的角色分配。 此时还会显示当前分配给该用户的所有任务。

在此更改之前，过滤器仅控制在“未分配”区域显示哪些任务和问题。 仅当用户与“未分配”区域中任务的角色分配匹配时，才会在计划时间轴中显示用户。

有关使用过滤器控制计划时间轴上显示的内容的更多信息，请参阅“在计划区域中过滤信息”和“在计划区域中手动分配未分配的任务和问题”。

### 用户在被分派任务后保留在时间轴上 {#users-remain-on-the-timeline-after-being-assigned-a-task}

分配任务或问题后，即使没有具有匹配角色分配的剩余任务或问题，用户仍会保留在计划时间线上。 这允许您在分配用户后进行任何必要的更改。

在此更改之前，如果“未分配”区域中没有具有匹配角色分配的剩余任务或问题，则在为用户分配任务或问题后，用户将立即从计划时间表中消失。

有关更多信息，请参阅“在计划区域中手动分配未分配的任务和问题”。

## 通过更改对象名称自定义Workfront术语

您现在可以通过更改某些对象的名称来自定义Workfront术语。\
使用布局模板，您现在可以更改以下工作对象的名称以符合您组织中的需求：

* 项目组合
* 项目群
* 项目
* 任务
* 问题

例如，如果在您的组织中使用活动而不是项目，则可以将“项目”对象的名称替换为“活动”。

进行此替换时，应用程序的以下区域显示对象的更新名称：

* 全局导航栏
* 所有选项卡
* 所有菜单 
* Report Builder和报告元素（视图、筛选器和分组）
* 保存按钮
* 导出的文件
* 电子邮件

以下区域不显示对象的更新名称：

* 资源评估
* 资源预算管理器
* 性能规划者
* 资源网格
* 团队创建者
* Portfolio优化器 
* 移动应用程序
* Outlook加载项

有关如何使用布局模板自定义Workfront术语的更多信息，请参阅创建和管理布局模板中的“自定义术语”部分和以下内容中的“了解自定义对象名称的含义”部分 [了解Adobe Workfront中的对象](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 在报告中包括批准开始日期和结束日期

现在，在创建或修改报告时，您可以包含以下字段：

* 审批路径开始日期
* 审批路径完成日期

利用这些字段，可深入了解当前或最近审批路径的启动时间和标记为完成时间。

有关这些字段的更多信息，请参阅 [Adobe Workfront术语表](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

有关批准路径、创建和触发路径的方式以及路径在批准流程中使用的功能的更多信息，请参阅 [创建工作项的审批流程](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

以下字段已从Workfront中删除，无法再包含在报表中（这些字段提供了有关项目的信息，而不是有关审批本身的信息，并且经常被滥用）：

* 计划审批开始日期
* 审批预计开始日期
* 审批估计开始日期

## “我已做的请求”的新电子邮件摘要选项

每日摘要投放选项已添加到通知设置的“我已提出的请求”区域。

有关更多信息，请参阅 [修改您自己的电子邮件通知](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

请记住更新与您的帐户关联的电子邮件地址，以便能够测试此功能。 这是必需的，因为预览沙盒会清除所有用户的电子邮件地址。

## 更新了文档审批电子邮件通知的外观

“文档审批”通知的外观已通过新的UI更新：

有关电子邮件通知的更多信息，请参阅 [Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md).

请记住更新与您的帐户关联的电子邮件地址，以便能够测试此功能。 这是必需的，因为预览沙盒会清除所有用户的电子邮件地址。

## 里程碑视图中的增强功能

查看项目列表或项目报告时可用的里程碑视图现在包含以下增强功能：

* 计划日期可编辑
* 此时会显示项目和任务的完成百分比

在此更改之前，为了编辑日期或查看完成百分比，您必须转到单个任务。

有关更多信息，请参阅 [使用里程碑视图](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
