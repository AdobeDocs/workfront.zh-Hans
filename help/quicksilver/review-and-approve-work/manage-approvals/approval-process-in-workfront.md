---
content-type: overview
product-area: projects
navigation-topic: approvals
title: 审批流程概述
description: 您可以创建批准流程并将其附加到对象，以确保指定用户在对象继续运行之前查看某些更改。
author: Courtney
feature: Work Management
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1747'
ht-degree: 0%

---

# 审批流程概述

您可以创建批准流程并将其附加到对象，以确保指定用户在对象继续运行之前查看某些更改。

这适用于Adobe Workfront中的以下类型的对象：

* 工作项（项目、任务或问题、模板、模板任务）
* 文档
* Proof

有关创建批准流程的说明，请参阅 [为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

本文包含有关与工作项关联的审批流程的一般信息。

## 审批流程类型

如果您是Adobe Workfront管理员，或者是对审批流程具有管理访问权限的用户，则可以为项目、任务和问题创建以下审批流程：

* **系统级全局批准流程**:用户可以将这些值附加到以下任意值：

   * “审批”部分中的项目、任务或问题
   * 在“编辑项目”框中，任务默认审批流程区域
   * 在项目的“队列详细信息”或“队列主题”部分的“默认审批流程”区域中。 项目必须作为请求队列启用。

* **组级全局批准流程**:用户可以将这些值附加到以下内容：

   * 属于与审批部分中的审批流程相关联的组的项目、任务或问题
   * 在“编辑项目”框中，属于与审批流程关联的组的项目的“任务默认审批流程”区域
   * 在项目的“队列详细信息”或“队列主题”部分的“默认审批流程”区域中。 项目必须作为请求队列启用，并且必须属于与审批流程关联的组。

   有关创建系统级或组级审批流程的信息，请参阅 [为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

* **一次性审批流程**:用于单个项目、任务、问题、模板或模板任务。 此类审批流程仅影响与其关联的对象，且不能与任何其他对象关联。

   有关创建一次性审批流程的信息，请参阅 [将新审批流程或现有审批流程与工作关联](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>本文使用术语“全局批准流程”来区分“单次使用批准流程”。 全局批准流程可重复使用。
>
>术语“组级全局批准流程”是指可重复用于项目且状态仅与特定组关联的批准流程。

有关创建系统级审批流程或组级审批流程的信息，请参阅 [为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 有关审批流程的注意事项

* 您必须先创建项目、任务、问题、模板或模板任务，然后审批流程才能与它们关联。
* 审批流程始终与两个基本事项相关联：

   * 每个审批流程都对应于Workfront系统中的特定工作项状态。 当您更改工作项的状态时，附加的对该状态的批准要求先确认状态更改，然后才能将新状态分配给该项。

      >[!TIP]
      >
      >
      >   
      >   
      >   * 您可以将组级别审批与全局或组级别状态关联。
      >   * 您不能使用审批流程将物料的状态更改为与审批流程关联的状态以外的状态。

         >   
         >   
         >     例如，如果任务批准与“进行中”状态关联，则在批准后，任务会自动将其状态更改为“进行中”。 它无法自动将其状态更改为“已完成”或与审批无关的任何其他状态。


   * 与审批流程关联的实体可以是用户、职务或团队。 用户最终有责任接受或拒绝批准。 您可以为在项目中履行特定角色的用户分配批准。 例如，您可以为项目所有者或赞助商分配批准。 有关更多信息，请参阅 [为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

      存在以下情形：

      * 在为职务角色分配批准时，项目团队中与职务角色关联的任何用户都可以对批准作出决定。 与批准关联的角色可以是其主要角色，也可以是任何其他角色。

         有关项目团队的信息，请参阅 [项目团队概述](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * 当您为团队分配批准时，该团队的任何成员都可以对批准做出决策。 与批准关联的团队可以是其主团队，也可以是其任何其他团队。

         有关用户角色和团队的信息，请参阅 [编辑用户的配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 创建工作项时，不会自动附加批准流程。 如果要使用，则必须手动附加一个。 有关将审批流程附加到项目的信息，请参阅 [将新审批流程或现有审批流程与工作关联](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* Workfront管理员或具有审批流程管理访问权限的用户可以创建系统级别的全局审批流程，以在整个系统中使用。 具有审批流程管理访问权限的组管理员可以创建组级别的全局审批流程，以便仅供其管理的特定组使用。
* 如果您不想对工作项使用预定义的系统级别或组级别全局审批流程，则当您对要附加审批流程的对象具有“管理”权限时，可以创建一次性审批流程并将其附加到该流程。

   >[!NOTE]
   对于为其创建审核流程的特定项目，您只能使用一次一次性审批流程。 您可以关联项目、任务、问题、模板和模板任务的一次性审批流程的全局状态和组级别状态。

* 在使用组级别自定义状态将组级别审批流程附加到项目时，更改项目组可能会在上一组的审批状态与系统级别的现有审批状态之间产生冲突。 在更新项目组之前，请考虑删除项目上的组级审批流程或其任务或问题。 有关创建组级审批流程的信息，请参阅 [组级别的审批流程](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). 有关创建自定义群组状态的信息，请参阅 [创建或编辑群组状态](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). 有关更新项目组的信息，请参阅 [编辑项目](../../manage-work/projects/manage-projects/edit-projects.md).

## 审批流程工作流程

本节将介绍有关批准工作项目的以下内容：

* [审批流程如何依赖状态](#how-approval-processes-rely-on-statuses)
* [典型工作流程如何使用批准流程](#how-a-typical-workflow-uses-an-approval-process)

### 审批流程如何依赖状态 {#how-approval-processes-rely-on-statuses}

将状态附加到审批流程可确保项目按正确顺序在各部门之间移动。

**示例：** 您可以将审批流程附加到营销部门状态，该状态需要财务部门的批准。 然后，当某人将工作项的状态更改为“营销部”时，该项目只有在财务部门注销后才能移至该部门。

有关工作项目状态的更多信息，请参阅以下文章：

* [访问系统项目状态列表](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [访问系统任务状态列表](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [访问系统问题状态列表](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### 典型工作流程如何使用批准流程 {#how-a-typical-workflow-uses-an-approval-process}

以下情景说明了在Workfront对象按此顺序通过多个步骤的工作流程进行时，审批流程如何帮助用户批准工作：

1. Workfront管理员或对审批流程具有管理访问权限的用户会为项目、任务或问题创建审批流程。

   >[!NOTE]
   您可以将项目审批流程附加到模板，将任务审批流程附加到模板任务。 在执行此操作后，当有人使用模板创建项目时，审批流程将分别变为项目或任务审批流程。 附加到模板或模板任务的一次性审批流程对于项目和任务来说仍然是一次性审批流程。

1. 对项目、任务或问题具有“管理”权限的用户将审批流程附加到项目，或为项目创建一次性审批。
1. 分配给工作项的用户将其状态更改为启动审批流程和审批流程开始的状态。 （创建审批流程的人员定义了状态与审批流程之间的关系。）
1. 指定的批准者接收有关待批准流程的通知，并审核工作项。
1. 批准流程在指定批准者批准流程的所有步骤后结束。 或者，如果拒绝某个步骤，则状态将重置为预定义状态，或者创建问题。 （创建审批流程的人员定义了其中哪些自动化步骤会在拒绝后发生。）

**示例：** 广告团队创建了一个名为“准备打印”的状态，以及一个名为“设计人员/撰稿人签名”的批准流程，该流程与此状态关联。 此批准流程配置为：

* 需要团队的设计人员和撰稿人批准
* 当某人将工作项的状态更改为“准备打印”时启动

手册项目所有者将设计人员/撰稿人签字批准流程附加到手册项目。

当项目中的某人将状态更改为“准备打印”时，撰稿人和设计人员会收到通知，要求他们批准或拒绝该项目。 在审批过程中，当审议是否批准时，项目状态显示为“准备打印 — 待批”。

在两人批准Workfront中的手册后，项目状态将变为“准备打印”。

## 文档批准流程

文档批准用于更一般的批准。 在“更新”选项卡上，以聊天格式捕获反馈。 您可以使用批准按钮批准、拒绝或批准更改。

要在文档上传到Workfront后将批准者添加到文档，请参阅 [请求文档批准](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## 验证批准流程

校样批准用于进行更深入的审阅，通常包含更复杂的工作流。 在校样查看器中使用标记工具捕获反馈。 您可以使用批准按钮批准、拒绝或批准更改。

要向文档校样添加自动工作流并指定工作流中的某些用户作为校样的批准者，请参阅 [使用自动工作流创建高级校样](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## 为工作项审批流程配置设置

作为Workfront管理员，您可以在系统中为工作项审批流程配置全局设置。 这些设置决定了批准流程的各种规则，如允许批准决定保持打开状态的时间长短，或您如何在系统中管理批准委派。 有关批准流程设置的更多信息，请参阅 [配置全局批准设置](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).
