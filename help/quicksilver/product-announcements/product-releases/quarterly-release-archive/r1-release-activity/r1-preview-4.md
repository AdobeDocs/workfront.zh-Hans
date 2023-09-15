---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1预览4
description: 本页介绍R1.4版本在“预览”环境中可用的所有更改。 2017年2月15日，预览环境中提供了此页面上的功能。
author: Luke
feature: Product Announcements
exl-id: 2945e058-74dd-4cc3-9d6c-e5618ee7041c
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# R1预览4

本页介绍R1.4版本在“预览”环境中可用的所有更改。 2017年2月15日，预览环境中提供了此页面上的功能。

有关在R1中所做所有更改的列表，请参见 [Workfront R1版本](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/workfront-r1-release.md).

## 已更新项目、任务和问题审批

在为项目、任务和问题批准创建批准流程时，现在提供了以下增强功能和更改： 

* 批准“步骤”现在称为批准“阶段”。
* 在每个阶段包含多种类型的批准者。\
  这包括用户、团队和工作角色。\
  在此更改之前，您可以仅包含相同类型的多个批准者。 例如，您可以包含多个工作角色，但不能包含工作角色和团队。

* 删除了与修改现有全局审批流程相关的下列预先存在的限制：

   * 修改后的审批流程仅反映在审批流程尚未启动或审批流程未修改的系统对象上。 已启动审批流程或已修改审批流程的对象不会随您的更改而更新。
   * 您无法修改决定批准何时开始的状态。

* 更新了外观。

有关创建审批流程的详细信息，请参阅 [创建工作项的审批流程](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

将审批流程与项目、任务或问题关联时，现在提供了以下增强功能和更改：

* 更新了外观。
* 审批图显示在审批选项卡上，以可视化形式显示以前、当前和未来的审批步骤。

有关将审批与项目、任务和问题关联的更多信息，请参阅 [将新的或现有的审批流程与工作关联](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 直接从项目页面更改项目的状态

您不再需要编辑项目来更改项目状态。 您现在可以直接从项目主页更改项目的状态。

有关更多信息，请参阅 [更改项目的状态](../../../../manage-work/projects/manage-projects/change-project-status.md).

## 安排用户停用

您现在可以安排在将来的日期停用用户。

在此增强功能之前，您只能立即手动停用用户。

计划取消激活的用户在各种情况下可能很有用。 例如，如果您在Workfront中创建临时雇用的用户，则可以将其设置为在合同结束时停用。

在批量编辑用户时，此功能也可用。 

有关安排用户停用的更多信息，请参阅 [停用或重新激活用户](../../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) 和 [添加用户](../../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## 针对“所需操作”的新电子邮件摘要选项

“每日摘要”传送选项现在可在“通知”设置的“所需操作”区域使用。

有关更多信息，请参阅 [修改您自己的电子邮件通知](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

请记住更新与您的帐户关联的电子邮件地址，以便能够测试此功能。 这是必需的，因为预览沙盒会清除所有用户的电子邮件地址。

## 回收站改进：记录在更新流中并接收电子邮件通知

在恢复已删除的项目、任务和问题时添加了以下增强功能：

* 现在，您在恢复对象后会收到电子邮件通知。\
  作为Workfront管理员，现在，您在恢复之前删除的项目、任务或问题后会收到电子邮件通知。 电子邮件通知会告知您恢复过程的状态。\
  有关在Workfront中恢复对象的更多信息，请参阅 [恢复已删除的项目](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* 当对象被恢复时，对象的删除和恢复现在记录在对象本身的更新流和父对象的更新流中。\
  以前，仅在父对象的更新流中记录删除。\
  例如，当任务恢复时，将向项目和任务本身的更新流中添加一条消息，指示任务已恢复。 (子任务上不记录删除和恢复。 有关子任务的删除和恢复信息仅在父任务中可用。)\
  有关更多信息，请参阅 [恢复已删除的项目](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

 

## 更新了用于管理组成员资格的对话框

我们为组和子组的管理提供了一个新界面，可提供更简单、更友好的用户体验。

“组所有者”字段和“组成员”字段现在合并为一个字段，其中包含下面列出的组成员列表。 此外，您可以筛选组成员列表，并更改他们是所有者还是成员。 

有关将子组添加到组以及将用户指定为组的成员或组所有者的详细信息，请参阅 [创建组](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) 和 [创建组](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

 

## 在移动设备应用程序中复制文本

您可以复制移动设备应用程序中可见的所有对象的以下字段中的文本：

* 名称
* 描述
* 参考号
* 注释

此功能应在2月13日当周同时发布到iOS和Android应用商店。
