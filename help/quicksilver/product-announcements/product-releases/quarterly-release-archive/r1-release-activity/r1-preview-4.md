---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1预览4
description: 本页介绍R1.4版本的预览环境中所有可用的更改。 本页面上的功能已于2017年2月15日在预览环境中提供。
author: Luke
feature: Product Announcements
exl-id: 2945e058-74dd-4cc3-9d6c-e5618ee7041c
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# R1预览4

本页介绍R1.4版本的预览环境中所有可用的更改。 本页面上的功能已于2017年2月15日在预览环境中提供。

有关R1中所有更改的列表，请参阅 [Workfront R1版本](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/workfront-r1-release.md).

## 更新了项目、任务和发布批准

在为项目、任务和发布审批创建审批流程时，现在提供以下增强功能和更改： 

* 审批“步骤”现在称为审批“阶段”。
* 在每个阶段包括多种类型的批准者。\
   这包括用户、团队和工作角色。\
   在进行此更改之前，您只能包括同一类型的多个批准者。 例如，您可以包含多个作业角色，但不能包含作业角色和团队。

* 以下与修改现有全局批准流程相关的先前存在的限制已被删除：

   * 修改后的审批流程仅反映在审批流程尚未启动或审批流程未修改的整个系统中的对象上。 审批流程已启动或审批流程已修改的对象不会随您的更改而更新。
   * 您无法修改决定批准何时开始的状态。

* 更新了外观。

有关创建审批流程的更多信息，请参阅 [为工作项创建审批流程](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

在将审批流程与项目、任务或问题关联时，现在可以使用以下增强功能和更改：

* 更新了外观。
* 审批图表显示在审批选项卡上，以可视方式显示以前、当前和将来的审批步骤。

有关将审批与项目、任务和问题关联的详细信息，请参阅 [将新审批流程或现有审批流程与工作关联](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 直接从项目页面更改项目的状态

您不再需要编辑项目即可更改项目状态。 现在，您可以直接从项目的主页更改项目的状态。

有关更多信息，请参阅 [更改项目的状态](../../../../manage-work/projects/manage-projects/change-project-status.md).

## 计划用户停用

您现在可以安排在将来的日期停用用户。

在进行此增强之前，您只能立即手动停用用户。

在多种情况下，计划停用用户会非常有用。 例如，如果您在Workfront中创建临时聘用的用户，则可以将他们设置为在合同终止时停用。

在批量编辑用户时，此功能也可用。 

有关计划用户停用的更多信息，请参阅 [停用或重新激活用户](../../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) 和 [添加用户](../../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## 新增了“所需操作”的电子邮件摘要选项

“每日摘要”投放选项现在在“通知”设置的“需要的操作”区域中可用。

有关更多信息，请参阅 [激活或停用您自己的事件通知](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

请记住更新与您的帐户关联的电子邮件地址，以便能够测试此功能。 这是必需的，因为预览沙盒会清除所有用户的电子邮件地址。

## 回收站改进：在更新流中记录并接收电子邮件通知

在恢复已删除的项目、任务和问题时添加了以下增强功能：

* 现在，您在恢复对象后会收到电子邮件通知。\
   现在，作为Workfront管理员，您在恢复之前删除的项目、任务或问题后会收到一封电子邮件通知。 电子邮件通知会通知您恢复过程的状态。\
   有关在Workfront中恢复对象的更多信息，请参阅 [恢复已删除的项目](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* 当对象被恢复时，对象的删除和恢复现在记录在对象本身的更新流和父对象的更新流中。\
   以前，只在父对象的更新流中记录删除。\
   例如，在恢复任务时，将向项目和任务本身的更新流中添加一条消息，指示该任务已恢复。 (删除和还原操作不记录在子任务上。 有关删除和还原子任务的信息仅在父任务上可用。)\
   有关更多信息，请参阅 [恢复已删除的项目](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

 

## 更新了用于管理组成员资格的对话框

为群组和子群组的管理提供了一个新界面，可提供更轻松、更易用的体验。

“群组所有者”字段和“群组成员”字段现在组合到一个字段中，其中列出了群组成员列表。 此外，您还可以过滤群组成员列表并更改它们是所有者还是成员。 

有关向组添加子组以及将用户指定为组成员或组所有者的更多信息，请参阅 [创建群组](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) 和 [创建群组](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

 

## 在移动设备应用程序中复制文本

您可以复制以下字段中显示在移动设备应用程序中的所有对象的文本：

* 名称
* 描述
* 参考号
* 注释

此功能应于2月13日这一周发布到iOS和Android应用商店。
