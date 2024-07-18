---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1预览1和2
description: 本页介绍R1.1和R1.2版本在“预览”环境中提供的所有更改。 2017年1月19日，预览环境中提供了此页面上的功能。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 2%

---

# R1预览1和2

本页介绍R1.1和R1.2版本在“预览”环境中提供的所有更改。 2017年1月19日，预览环境中提供了此页面上的功能。

有关R1中所做所有更改的列表，请参阅[R1发布活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md)。 

## 从回收站恢复项目、任务和问题 

Workfront管理员现在可以恢复过去30天内删除的项目、任务和问题。 与项目、任务或问题相关的所有信息都会恢复，包括文档和自定义数据。

新选项也可用于配置针对已删除的项目、任务或问题记录的小时数的变化情况。 有关详细信息，请参阅[在删除并还原对象时配置影响时间](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md)。

有关在Workfront中还原对象的详细信息，请参阅[还原已删除的项目](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。

有关如何查看最近恢复的项目、任务和问题的信息，请参阅[查看已恢复的项目](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md)。

## 审批流程图显示先前、当前和未来审批步骤的可视化表示形式

现在，当项目、任务或问题等待审批时，会显示图表。 批准图显示了批准流程中的当前步骤（待定），并允许您快速查看以前和未来的批准步骤，而无需导航到批准选项卡。

在此更改之前，有关审批步骤的信息仅在项目、任务或问题的审批选项卡上可用，并且仅显示在列表视图而非图视图中。 （此信息在“审批”选项卡中仍可用且未更改。）

在项目中，审批信息显示在标题旁边的标题中。 在任务和问题上，批准信息显示在右侧面板中。

有关详细信息，请参阅[批准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md)，位于  [审批工作](../../../../review-and-approve-work/manage-approvals/approving-work.md)。

## 配置待审批的待更新对象

当项目、任务或问题正在等待审批时，您现在可以配置用户是否可以：

* 编辑待审批项目、任务或问题的自定义表单。\
  有关如何配置待审批时要编辑的项目、任务和问题的信息，请参阅[配置全局审批设置](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* 将问题添加到待审批的项目。\
  有关如何配置项目以允许用户在项目未决批准时添加问题的信息，请参阅[配置系统范围项目首选项](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

* 编辑待审批项目中的任务和问题。\
  有关如何配置项目以允许用户在项目未决批准时编辑任务和问题的信息，请参阅[配置系统范围项目首选项](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

在此更改之前，无法编辑未决批准的项目、任务和问题；此外，无法将问题添加到未决批准的项目，并且无法在未决批准的项目中编辑任务和问题。

## 将布局模板分配给组

您现在可以将布局模板分配给组。

在此更改之前，您可以将布局模板分配给用户、团队和工作角色。 将布局模板分配给组时，其分配优先级最低。 

有关详细信息，请参阅创建和管理布局模板。

## 更改了批量编辑用户通知

围绕批量编辑用户电子邮件通知设置的功能已更改。 如果选择多个用户编辑其通知电子邮件设置，则所有选定用户仅会更改要更新的特定通知。 对于所选的所有用户，所有未更改的电子邮件通知设置保持不变，即使这些设置因用户而异。 

在此更改之前，您选择的电子邮件通知设置已保存，并且在保存更改时，所有其他未更改通知设置都已取消选择。 

有关详细信息，请参阅[修改您自己的电子邮件通知](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)中的“批量修改用户通知设置”。

## 更新了多个电子邮件通知的外观

以下电子邮件通知的外观已更新为新的UI：

* 问题分配
* 提交日期更改
* 我参与的一个项目成为活动状态
* 向利害关系方作出批准决定
* 前置任务完成到任务依赖
* 未决批准（项目、任务、问题）
* 项目、任务、问题的状态更改

请记住更新与您的帐户关联的电子邮件地址，以便能够测试此功能，因为预览沙盒将清除所有用户的电子邮件地址。    有关电子邮件通知的详细信息，请参阅[Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md)。  

## 多个通知区域的新电子邮件摘要选项

以下通知区域已添加“每日摘要”选项：

* 有关我参与的项目的信息
* “我赞助的项目”相关信息
* 批准信息
* “分配给我的工作”相关信息
* 通信

有关详细信息，请参阅[Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md)。  请记住更新与您的帐户关联的电子邮件地址，以便能够测试此功能，因为预览沙盒将清除所有用户的电子邮件地址。 

## 将组设为公用

现在，将组设为公共组时，您可以将该组添加到用户，而无需成为组所有者。 您必须具有用户管理权限才能编辑用户。

有关将组公开的详细信息，请参阅[创建组](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)中的[创建组](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public)部分。

## 共享移动应用程序中对象的URL 

现在，您可以在Workfront移动设备应用程序上的以下对象中共享URL：

* 项目
* 任务
* 问题
* 工时表
* 文档

可以在以下应用程序中共享对象的URL：

* 文本消息
* 电子邮件
* 存储驱动器（例如iCloud驱动器）
* 其他已安装的应用程序(例如Notes、Facebook)
* 您可以将指向对象的链接复制到剪贴板，然后将其粘贴到任何其他应用程序中。 

## 设置中的上下文相关帮助

“设置”菜单下的所有区域已更新，区域右上角有一个帮助图标。 此图标提供指向有关该区域的帮助站点文章的链接。 “设置”区域中的一些部分也更新了“帮助”图标。 

## 添加更精确的费用率

现在，您可以在创建费用类型时添加更准确的费用率。 小数点后费用费率最多可包含4个字符（例如，1.0375）。 这意味着，任何使用此速率的字段都可以更精确。

在此更改之前，费用费率最多只能包含小数点后的2个字符（例如1.03）。

有关创建费用率的详细信息，请参阅[创建自定义费用类型](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md)。

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## R1 Preview 1和2 Release网络研讨会录像

此网络研讨会由Workfront发布准备团队于2017年1月19日主持。 此网络研讨会重点讨论了2017年的版本更改，并涵盖了可在预览中测试的新功能。
