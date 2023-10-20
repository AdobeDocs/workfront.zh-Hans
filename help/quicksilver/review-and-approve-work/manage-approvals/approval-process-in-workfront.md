---
content-type: overview
product-area: projects
navigation-topic: approvals
title: 审批流程概述
description: 您可以创建批准流程并将其附加到对象，以确保指定用户在对象进行之前审阅某些更改。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '1747'
ht-degree: 0%

---

# 审批流程概述

您可以创建批准流程并将其附加到对象，以确保指定用户在对象进行之前审阅某些更改。

这适用于Adobe Workfront中的以下对象类型：

* 工作项（项目、任务或问题、模板、模板任务）
* 文档
* Proof

有关创建审批流程的说明，请参阅 [创建工作项的审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

本文包含与工作项关联的审批流程的一般信息。

## 审批流程类型

如果您是Adobe Workfront管理员或对审批流程具有管理访问权限的用户，则可以为项目、任务和问题创建以下审批流程：

* **系统级全局审批流程**：用户可以将这些内容附加到以下任意位置：

   * 审批部分中的项目、任务或问题
   * 在编辑项目框中的任务默认审批流程区域
   * 在项目的队列详细信息或队列主题部分、默认批准流程区域中。 项目必须启用为请求队列。

* **组级全局审批流程**：用户可以将这些文件附加到以下内容：

   * 属于与审批部分中的审批流程关联的组的项目、任务或问题
   * 在编辑项目框中，属于与审批流程关联的组的项目的任务默认审批流程区域
   * 在项目的队列详细信息或队列主题部分、默认批准流程区域中。 项目必须启用为请求队列，并且必须属于与审批流程关联的组。

  有关创建系统级别或组级别审批流程的信息，请参阅 [创建工作项的审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

* **一次性审批流程**：用于单个项目、任务、问题、模板或模板任务。 此类批准流程仅影响与其关联的对象，不能与任何其他对象关联。

  有关创建一次性审批流程的信息，请参阅 [将新的或现有的审批流程与工作关联](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>本文使用“全局批准流程”一词来区分“一次性批准流程”。 可以重复使用全局批准流程。
>
>术语“组级别全局审批流程”是指可以重复用于项目的审批流程，其状态仅与特定组关联。

有关创建系统级审批流程或组级审批流程的信息，请参阅 [创建工作项的审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 关于批准流程的注意事项

* 您必须先创建项目、任务、问题、模板或模板任务，然后才能将审批流程与其关联。
* 审批流程始终与以下两项基本要素相关联：

   * 每个审批流程都对应于Workfront系统中的特定工作项状态。 当您更改工作项的状态时，该状态的附加审批要求先确认状态更改，然后才能将新状态分配给该项。

     >[!TIP]
     >
     >
     >   
     >   
     >   * 您可以将组级别审批与全局或组级别状态相关联。
     >   * 您不能使用审批流程将项目的状态更改为与审批流程关联的状态以外的状态。
     >   
     >   
     >     例如，如果您有一个与状态为“进行中”的任务审批关联，则当审批被授予时，任务会自动将其状态更改为“进行中”。 它不能自动将其状态更改为“已完成”或任何其他与批准无关联的状态。
     >   
     >   
     >

   * 与审批流程关联的实体可以是用户、工作角色或团队。 用户最终负责接受或拒绝批准。 您可以将审批分配给在项目上履行特定职责的用户。 例如，您可以将审批分配给项目所有者或发起人。 有关更多信息，请参阅 [创建工作项的审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

     存在以下情况：

      * 将审批分配给工作角色时，项目团队中与该工作角色关联的任何用户都可以作出审批决定。 与批准关联的角色可以是其主要角色或任何其他角色。

        有关项目团队的信息，请参阅 [项目团队概述](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * 将审批分配给团队时，该团队的任何成员都可以对审批做出决定。 与批准关联的团队可以是他们的主团队或他们的任何其他团队。

        有关用户的角色和团队的信息，请参阅 [编辑用户配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 在创建工作项时，不会自动附加审批流程。 如果要使用一个，则必须手动附加。 有关将审批流程附加到项目的信息，请参阅 [将新的或现有的审批流程与工作关联](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* Workfront管理员或对批准流程具有管理访问权限的用户可以创建系统级别的全局批准流程，以在系统中使用。 对批准流程具有管理访问权限的组管理员可以创建组级别的全局批准流程，以便仅由他们管理的特定组使用。
* 如果不想对工作项使用预定义的系统级或组级全局审批流程，则可以在对要为其附加审批流程的对象具有“管理”权限时，创建并附加一次性审批流程。

  >[!NOTE]
  >
  对于为其创建该流程的特定项目，您只能使用一次性审批流程。 您可以为项目、任务、问题、模板和模板任务的一次性审批流程关联全局状态和组级别状态。

* 当使用组级别自定义状态将组级别审批流程附加到项时，更改项目的组可能会导致上一个组的审批状态与系统级别上现有的审批状态之间发生冲突。 在更新组之前，请考虑删除项目或其任务或问题的组级别审批流程。 有关创建组级审批流程的信息，请参阅 [组级别审批流程](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). 有关创建自定义组状态的信息，请参阅 [创建或编辑组状态](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). 有关更新项目组的信息，请参见 [编辑项目](../../manage-work/projects/manage-projects/edit-projects.md).

## 审批流程工作流

本节介绍有关批准工作项的以下内容：

* [审批流程如何依赖状态](#how-approval-processes-rely-on-statuses)
* [典型的工作流如何使用审批流程](#how-a-typical-workflow-uses-an-approval-process)

### 审批流程如何依赖状态 {#how-approval-processes-rely-on-statuses}

将状态附加到审批流程可确保物料按正确的顺序在部门间移动。

**示例：** 您可以将审批流程附加至需要财务部门审批的市场营销部门状态。 然后，当有人将某个工作项的状态更改为“营销部门”时，除非财务部门签收，否则该项无法移到该部门。

有关工作项状态的更多信息，请参阅以下文章：

* [访问系统项目状态的列表](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [访问系统任务状态的列表](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [访问系统问题状态的列表](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### 典型的工作流如何使用审批流程 {#how-a-typical-workflow-uses-an-approval-process}

以下场景说明了审批流程如何帮助用户审批工作，因为Workfront对象将按此顺序通过包含多个步骤的工作流：

1. Workfront管理员或对批准流程具有管理访问权限的用户创建项目、任务或问题的批准流程。

   >[!NOTE]
   >
   您可以将项目审批流程附加到模板，将任务审批流程附加到模板任务。 执行此操作后，当有人使用模板创建项目时，审批流程将分别变为项目或任务审批流程。 附加到模板或模板任务的一次性审批流程仍然是项目和任务的一次性审批流程。

1. 具有项目、任务或问题管理权限的用户将审批流程附加到项目，或为项目创建一次性审批。
1. 分配给工作项的用户将其状态更改为启动审批流程的状态，审批流程随即开始。 （创建审批流程的人员定义了状态与审批流程之间的关系。）
1. 指定的批准者会收到有关未决批准流程的通知，并会审阅工作项目。
1. 批准流程在指定的批准者批准流程的所有步骤后结束。 或者，如果他们拒绝某个步骤，则状态会重置为预定义状态，或者会创建一个问题。 （创建批准流程的人员定义了在拒绝后执行其中的哪些自动步骤。）

**示例：** 广告团队已创建了一个名为“准备打印”的状态，并创建了一个名为“设计者/撰稿人签署”的审批流程，该流程与其关联。 此审批流程配置为：

* 需要团队的设计人员和撰稿人批准
* 每当有人将工作项的状态更改为“准备打印”时启动

宣传册项目所有者将设计人员/撰稿人签名审批流程附加到宣传册项目。

当项目中的某人将状态更改为“准备打印”时，撰稿人和设计人员会收到通知，要求他们批准或拒绝此项目。 在审批过程中，当他们考虑是否审批时，项目的状态显示为准备打印 — 未决批准。

在Workfront中审批宣传册后，项目状态将更改为准备打印。

## 文档审批流程

文档审批用于更一般的审批。 在“更新”选项卡上以聊天格式捕获反馈。 您可以使用批准按钮批准、拒绝或批准更改。

要在文档上传到Workfront后添加审批者，请参阅 [请求文档审批](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## 验证审批流程

验证审批用于更深入的审查，通常包括更复杂的工作流。 反馈是通过验证查看者中的标记工具捕获的。 您可以使用批准按钮批准、拒绝或批准更改。

要将自动工作流添加到文档验证，并将工作流中的某些用户指定为验证的审批者，请参阅 [使用自动化工作流创建高级验证](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## 配置工作项审批流程设置

作为Workfront管理员，您可以为系统中的工作项审批流程配置全局设置。 这些设置决定了批准流程的各种规则，例如允许批准决策保持打开状态的时间长度或如何在系统中管理批准委派。 有关审批流程设置的详细信息，请参阅 [配置全局审批设置](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).
