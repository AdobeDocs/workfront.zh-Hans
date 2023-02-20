---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1预览3
description: 本页介绍R1.3版本的“预览”环境中所有可用的更改。 此页面上的功能已于2017年2月1日在预览环境中提供。
author: Luke
feature: Product Announcements
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: f4cc5ae89c8746ec4c40ece88bfdb21dc1996575
workflow-type: tm+mt
source-wordcount: '1345'
ht-degree: 2%

---

# R1预览3

本页介绍R1.3版本的“预览”环境中所有可用的更改。 此页面上的功能已于2017年2月1日在预览环境中提供。

有关R1中所有更改的列表，请参阅 [R1发行活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## 改进的外部文件链接方法

现在，用于链接来自外部源(如Google驱动器、框、Dropbox等)的文档的选项位于“文档”区域中较为突出的位置。 

此外，在首次链接来自该提供商的文件之前授权文档提供商的操作现在更加直观（在链接来自外部提供商的文件时，这只是一个额外的步骤）。

在进行这些更改之前，用于从外部源链接文件的选项位于“文档”区域的“添加文档”对话框中。 首次从外部源链接文档之前，链接文档的用户必须在“设置”区域中授权该文档提供程序。

有关更多信息，请参阅  [从外部应用程序链接文档](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## 更新了处理日历的团队

>[!NOTE]
>
>在23.1版本中，资源计划工具已弃用并从Workfront中删除。 有关使用负载平衡器计划资源的信息，请参阅 [工作负载平衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

现在，适用于团队的“工作”日历包含其他功能以及更新的外观。 “工作日历”团队现在的功能与项目的资源计划工具类似。

更新的“工作日历”团队包括以下改进：

* 按角色的字母顺序或分组查看用户。
* 按项目优先级、状态和单个项目过滤计划时间轴。 您还可以按角色和用户过滤计划时间轴。 （与计划项目资源时相比，“筛选器”区域包含的选项更少。）
* 包括计划时间表上的问题。
* 显示用户分配并修改用户每天分配给某些任务和问题的小时数。
* 查看显示用户在任何给定日期过度分配的时间的指标。
* 配置是否在计划时间轴上显示已完成的工作。

计划项目资源时与资源计划工具的差异：

* 所有团队成员都显示在“工作于”(Working On)团队日历上。\
   在计划项目资源时，只显示与其关联的角色与“未分配”区域中一个或多个任务的角色相匹配的用户。
* “交换”工具不可用未包含在“工作于”(Working On)团队日历中。
* 任何团队成员都可以在“工作于”(Working On)团队日历上进行更改。\
   在计划项目资源时，只有资源经理才能为项目做出资源决策。
* 默认情况下，“工作于”(Working On)团队日历中会显示问题。\
   在计划项目资源时，默认情况下不会显示问题。

有关使用更新的团队处理日历的更多信息，请参阅“资源计划”。

## 资源计划增强功能

计划时间轴包括以下增强功能：

* “使用过滤器控制在计划时间线上显示哪些用户”
* “用户在被分配任务后仍停留在时间轴上”

### 使用过滤器控制在计划时间轴上显示哪些用户 {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

>[!NOTE]
>
>在23.1版本中，资源计划工具已弃用并从Workfront中删除。 有关使用负载平衡器计划资源的信息，请参阅 [工作负载平衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

过滤器现在可用于控制在计划时间轴上显示哪些用户，以及在“未分配”区域中显示哪些任务和问题。 在筛选器中选择用户后，将仅显示您选择的用户，而不管他们的角色分配是否与“未分配”区域中任务的角色分配相匹配。 此外，还会显示当前分配给该用户的所有任务。

在进行此项更改之前，过滤器仅控制在“未分配”区域中显示哪些任务和问题。 仅当用户与“未分配”区域中任务的角色分配匹配时，才会在计划时间轴中显示用户。

有关使用过滤器控制计划时间轴上显示内容的更多信息，请参阅“在计划区域中过滤信息”和“在计划区域中手动分配未分配的任务和问题”。

### 为用户分配任务后，用户将停留在时间轴上 {#users-remain-on-the-timeline-after-being-assigned-a-task}

在为用户分配任务或问题后，即使没有具有匹配角色分配的剩余任务或问题，用户仍会停留在计划时间线上。 这允许您在分配用户后进行任何必要的更改。

在进行此更改之前，如果“未分配”区域中没有具有匹配角色分配的剩余任务或问题，则在为用户分配任务或问题后，用户将立即从计划时间轴中消失。

有关更多信息，请参阅“在计划区域中手动分配未分配的任务和问题”。

## 通过更改对象名称自定义Workfront术语

您现在可以通过更改某些对象的名称来自定义Workfront术语。\
现在，使用布局模板，您可以更改以下工作对象的名称以满足您组织的需求：

* 项目组合
* 项目群
* 项目
* 任务
* 问题

例如，如果您在组织中使用营销活动而不是项目，则可以将“项目”对象的名称替换为“营销活动”。

进行此替换时，应用程序的以下区域会显示对象的更新名称：

* 全局导航栏
* 所有选项卡
* 所有菜单 
* 报表生成器和报表元素（视图、过滤器和分组）
* 保存按钮
* 导出的文件
* 电子邮件

以下区域不显示对象的更新名称：

* 资源评估
* 资源预算管理器
* 性能规划者
* 资源网格
* 团队创建者
* Portfolio优化程序 
* 移动设备应用程序
* Outlook插件

有关如何使用布局模板自定义Workfront术语的更多信息，请参阅 [了解Adobe Workfront中的对象](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 在报表中包括批准开始和结束日期

现在，您可以在创建或修改报表时包含以下字段：

* 审批路径开始日期
* 批准路径完成日期

利用这些字段，可洞察当前或最近的批准路径何时开始以及标记为完成的时间。

有关这些字段的更多信息，请参阅 [Adobe Workfront术语表](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

有关批准路径、其创建和触发方式以及在批准流程中提供的功能的更多信息，请参阅 [为工作项创建审批流程](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

以下字段已从Workfront中删除，不再能包含在报告中（这些字段提供了有关项目的信息，而不是有关批准本身的信息，而且经常被滥用）：

* 批准计划开始日期
* 预计批准开始日期
* 估计批准开始日期

## 新增了“我发出的请求”的电子邮件摘要选项

“每日摘要”提交选项已添加到“通知”设置的“我已发出的请求”区域。

有关更多信息，请参阅 [激活或停用您自己的事件通知](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

请记住更新与您的帐户关联的电子邮件地址，以便能够测试此功能。 这是必需的，因为预览沙盒会清除所有用户的电子邮件地址。

## 更新了文档批准电子邮件通知的外观

“文档批准”通知的外观已更新为新的UI:

有关电子邮件通知的更多信息，请参阅 [Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md).

请记住更新与您的帐户关联的电子邮件地址，以便能够测试此功能。 这是必需的，因为预览沙盒会清除所有用户的电子邮件地址。

## 里程碑视图中的增强功能

查看项目列表或项目报表时可用的里程碑视图现在包含以下增强功能：

* 计划日期可编辑
* 将显示项目和任务的完成百分比

在进行此更改之前，要编辑日期或查看完成百分比，您必须转到单个任务。

有关更多信息，请参阅 [使用里程碑视图](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
