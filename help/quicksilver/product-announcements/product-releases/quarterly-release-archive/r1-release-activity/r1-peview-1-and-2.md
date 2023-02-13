---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1预览1和2
description: 本页介绍R1.1和R1.2版本在“预览”环境中可用的所有更改。 此页面上的功能于2017年1月19日在预览环境中提供。
author: Luke
feature: Product Announcements
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 2%

---

# R1预览1和2

本页介绍R1.1和R1.2版本在“预览”环境中可用的所有更改。 此页面上的功能于2017年1月19日在预览环境中提供。

有关R1中所有更改的列表，请参阅 [R1发行活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## 从回收站恢复项目、任务和问题 

Workfront管理员现在可以恢复过去30天内已删除的项目、任务和问题。 与项目、任务或问题关联的所有信息都将恢复，包括文档和自定义数据。

还提供了新选项，用于配置针对已删除的项目、任务或问题记录的小时数所发生的情况。 有关更多信息，请参阅 [配置在删除和还原对象时对小时数的影响](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

有关在Workfront中恢复对象的更多信息，请参阅 [恢复已删除的项目](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

有关如何查看最近还原的项目、任务和问题的信息，请参阅 [查看还原的项目](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

## 审批图显示了以前、当前和将来审批步骤的可视化表示形式

现在，当项目、任务或问题的批准处于待批准状态时，将显示一个图表。 审批图显示了审批流程中的当前步骤（待定），还允许您快速查看以前和将来的审批步骤，而无需导航到“审批”选项卡。

在进行此项更改之前，有关批准步骤的信息仅在项目、任务或问题的“批准”选项卡上可用，并且仅在列表视图中显示，而不是在图表视图中显示。 （此信息仍可用，且在“批准”选项卡中未更改。）

在项目上，审批信息显示在项目标题旁边的标题中。 对于任务和问题，审批信息会显示在右侧面板中。

有关更多信息，请参阅 [批准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md) in  [批准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## 配置要更新的待批准对象

当项目、任务或问题等待批准时，您现在可以配置用户是否可以：

* 编辑待批准的项目、任务或问题的自定义表单。\
   有关如何配置待批准时要编辑的项目、任务和问题的信息，请参阅 [配置全局批准设置](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* 向待批准的项目添加问题。\
   有关如何配置项目以允许用户在项目处于待批准状态时添加问题的信息，请参阅 [配置系统范围的项目首选项](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 编辑项目中待批准的任务和问题。\
   有关如何配置项目以允许用户在项目等待批准时编辑任务和问题的信息，请参阅 [配置系统范围的项目首选项](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

在进行此项更改之前，无法编辑待批准的项目、任务和问题；此外，无法将问题添加到待批准的项目中，以及无法在待批准项目中编辑任务和问题。

## 将布局模板分配给组

您现在可以将布局模板分配给组。

在进行此更改之前，您可以将布局模板分配给用户、团队和工作角色。 将布局模板分配给组具有布局模板分配优先级中最低的排名。 

有关更多信息，请参阅“创建和管理布局模板”。

## 对批量编辑用户通知的更改

关于批量编辑用户电子邮件通知设置的功能已发生更改。 当您选择多个用户以编辑其通知电子邮件设置时，只会更改所有选定用户的正在更新的特定通知。 所有未更改的电子邮件通知设置对于选定的所有用户都保持相同，即使这些用户不同于用户。 

在进行此项更改之前，已保存您选择的电子邮件通知设置，并且在保存更改时，已取消选择所有其他未更改的通知设置。 

有关更多信息，请参阅 [激活或停用您自己的事件通知](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## 更新了多个电子邮件通知的外观

以下电子邮件通知的外观已更新为新的UI:

* 问题分配
* 提交日期更改
* 当项目状态从 idea/approved/rejected/requested/planning 更改为当前，发送电子邮件给团队
* 对利害关系方的批准决定
* 任务依赖项的前置任务完成
* 待批准（项目、任务、问题）
* 项目、任务、问题的状态更改

请记住，更新与您的帐户关联的电子邮件地址，以便能够测试此功能，因为预览沙盒会清除所有用户的电子邮件地址。    有关电子邮件通知的更多信息，请参阅 [Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md).  

## 多个通知区域的新电子邮件摘要选项

以下通知区域已添加“每日摘要”选项：

* 有关我正在执行的项目的信息
* “我赞助的项目”相关信息
* 批准信息
* “分配给我的工作”相关信息
* 通信

有关更多信息，请参阅 [Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md).  请记住，更新与您的帐户关联的电子邮件地址，以便能够测试此功能，因为预览沙盒会清除所有用户的电子邮件地址。 

## 将群组设为公用

将群组设为公用群组时，您现在可以将该群组添加到用户中，而无需成为群组所有者。 您必须具有用户管理访问权限才能编辑用户。

有关将群组公开的更多信息，请参阅 [创建群组](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public) 部分 [创建群组](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## 在移动设备应用程序中共享对象的URL 

现在，您可以在Workfront移动设备应用程序上共享以下对象的URL:

* 项目
* 任务
* 问题
* 时间表
* 文档

您可以在以下应用程序中共享对象的URL:

* 文本消息
* 电子邮件
* 存储驱动器（例如iCloud驱动器）
* 另一个已安装的应用程序(例如，Notes、Facebook)
* 您可以将指向对象的链接复制到剪贴板，稍后再粘贴到任何其他应用程序中。 

## 设置中的上下文相关帮助

“设置”菜单下的所有区域都已更新，其右上角都有一个“帮助”图标。 此图标提供有关该区域的帮助网站文章的链接。 “设置”区域内的某些部分也已更新为“帮助”图标。 

## 添加更精确的费用率

现在，您可以在创建费用类型时添加更准确的费用率。 费用率在小数后最多可包含4个字符（例如1.0375）。 这意味着使用此比率的任何字段都可以更精确。

在进行此项更改之前，费用率最多只能包含小数后的2个字符（例如1.03）。

有关创建费用率的详细信息，请参阅 [创建自定义费用类型](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## R1预览1和2版网络研讨会记录

此网络研讨会由Workfront版本准备团队于2017年1月19日召开。 此网络研讨会重点讨论了2017年版本更改，并介绍了可在“预览”中测试的新功能。
