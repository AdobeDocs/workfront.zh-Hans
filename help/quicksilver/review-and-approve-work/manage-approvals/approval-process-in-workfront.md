---
content-type: overview
product-area: projects
navigation-topic: approvals
title: 审批流程概述
description: 您可以创建批准流程并将其附加到对象，以确保指定用户在对象进行之前审阅某些更改。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '1804'
ht-degree: 0%

---

# 审批流程概述

<!-- Audited: 12/2023 -->

您可以创建批准流程并将其附加到对象，以确保指定用户在对象进行之前审阅某些更改。

这适用于Adobe Workfront中的以下对象类型：

* 工作项（项目、任务或问题、模板、模板任务）
* 文档
* 校样

本文包含与工作项关联的审批流程的一般信息。
有关创建审批流程的说明，请参阅[为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

## 工作项的审批流程类型

如果您是Adobe Workfront管理员或对审批流程具有管理访问权限的用户，则可以为项目、任务和问题创建以下审批流程：

* **系统级别的全局审批流程**：用户可以将这些流程附加到以下任何一项：

   * 审批部分中的项目、任务或问题
   * 在任务默认审批流程区域的编辑项目框中
   * 在项目的默认批准流程区域的队列详细信息或队列主题部分。 项目必须启用为请求队列。

* **组级全局审批流程**：用户可以将这些流程附加到以下内容：

   * 属于与审批部分中的审批流程关联的组的项目、任务或问题
   * 在任务默认审批流程区域的“编辑项目”框中，为属于与审批流程关联的组的项目
   * 在项目的默认批准流程区域的队列详细信息或队列主题部分。 项目必须启用为请求队列，并且必须属于与审批流程关联的组。

  有关创建系统级别或组级别审批流程的信息，请参阅[创建工作项的审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

* **一次性审批流程**：用于单个项目、任务、问题、模板或模板任务。 此类批准流程仅影响与其关联的对象，不能与任何其他对象关联。

  有关创建一次性审批流程的信息，请参阅[将新的或现有的审批流程与工作关联](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)。

>[!NOTE]
>
>本文使用“全局批准流程”一词来区分“一次性批准流程”。 可以重复使用全局批准流程。
>
>术语“组级别全局审批流程”是指可以重复用于项目的审批流程，其状态仅与特定组关联。

For information about creating a system-level approval process or a group-level approval process see [Create an approval process for work items](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Considerations about approval processes

* You must create the project, task, issue, template, or template task before the approval process can be associated with them.
* An approval process is always associated with two essential things:

   * Each approval process corresponds to a certain work item status in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.

     >[!TIP]
     >
     >
     >   
     >   
     >   * You can associate a group-level approval with a global or a group-level status.
     >   * You cannot change the status of an item using an approval process to a status other than the one associated with the approval process.
     >   
     >   
     >     For example, if you have a task approval associated with the status of In Progress, the task automatically changes its status to In Progress when the approval is granted. It cannot automatically change its status to Completed or any other status that is not associated with the approval.
     >   
     >   
     >

   * The entities associated with an approval process can be users, job roles, or teams. Users are ultimately responsible for accepting or rejecting the approval. You can assign approvals to users who fulfill a certain role on the project. For example, you can assign an approval to a Project Owner, or Sponsor. For more information, see [Create an approval process for work items](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

     存在以下情况：

      * When you assign an approval to job roles, any user on the Project Team who is associated with the job role can make a decision on the approval. The role associated with the approval can be either their Primary Role or any Other Roles.

        For information about the Project Team, see [Project Team overview](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * When you assign an approval to a team, any member of that team can make a decision on the approval. The team associated with the approval can be either their Home Team or any of their Other Teams.

        For information about a user&#39;s roles and teams, see [Edit a user&#39;s profile](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* When you create a work item, it does not automatically have an approval process attached. You must attach one manually if you want to use one. For information about attaching an approval process to an item, see [Associate a new or existing approval process with work](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* Workfront管理员或对批准流程具有管理访问权限的用户可以创建系统级别的全局批准流程，以在系统中使用。 对批准流程具有管理访问权限的组管理员可以创建组级别的全局批准流程，以便仅由他们管理的特定组使用。
* 如果不想对工作项使用预定义的系统级或组级全局审批流程，则可以在对要为其附加审批流程的对象具有“管理”权限时，创建并附加一次性审批流程。

  >[!NOTE]
  >
  >对于为其创建该流程的特定项目，您只能使用一次性审批流程。 您可以为项目、任务、问题、模板和模板任务的一次性审批流程关联全局状态和组级别状态。

* 当使用组级别自定义状态将组级别审批流程附加到项时，更改项目的组可能会导致上一个组的审批状态与系统级别上现有的审批状态之间发生冲突。 在更新组之前，请考虑删除项目或其任务或问题的组级别审批流程。 有关创建组级审批流程的信息，请参阅[组级审批流程](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md)。 有关创建自定义组状态的信息，请参阅[创建或编辑组状态](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)。 有关更新项目组的信息，请参阅[编辑项目](../../manage-work/projects/manage-projects/edit-projects.md)。

## 审批流程工作流

本节介绍有关批准工作项的以下内容：

* [审批流程依赖状态的方式](#how-approval-processes-rely-on-statuses)
* [典型的工作流如何使用审批流程](#how-a-typical-workflow-uses-an-approval-process)

### 审批流程如何依赖状态 {#how-approval-processes-rely-on-statuses}

将状态附加到审批流程可确保物料按正确的顺序在部门间移动。

**示例：**&#x200B;您可以将审批流程附加到需要财务部门审批的营销部门状态。 然后，当有人将某个工作项的状态更改为“营销部门”时，除非财务部门签收，否则该项无法移到该部门。

有关工作项状态的更多信息，请参阅以下文章：

* [访问系统项目状态列表](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [访问系统任务状态的列表](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [访问系统问题状态的列表](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### 典型的工作流如何使用审批流程 {#how-a-typical-workflow-uses-an-approval-process}

以下场景说明了审批流程如何帮助用户审批工作，因为Workfront对象将按此顺序通过包含多个步骤的工作流：

1. Workfront管理员或对批准流程具有管理访问权限的用户创建项目、任务或问题的批准流程。

   >[!NOTE]
   >
   >You can attach project approval processes to a template, and task approval processes to a template task. After you do this, when someone uses the template to create a project, the approval process becomes a project or task approval process respectively. A single-use approval process attached to a template or template task remains a single-use approval process for projects and tasks.

1. A user with Manage permission to the project, task or issue attaches the approval process to the item, or creates a single-use approval for the item.
1. A user assigned to the work item changes its status to the status that initiates the approval process and the approval process begins. (The person who created the approval process defined the relationship between the status and the approval process.)
1. The designated approvers receive a notification about the pending approval process and they review the work item.
1. The approval process ends after the designated approvers approve all steps of the process. Or, if they reject a step, the status is either reset to a predefined status, or an issue is created. (The person who created the approval process defined which of these automated steps happens after a rejection.)

**Example:** An advertising team has created a status called Ready for Printing and an approval process called Designer/ Copywriter Signoff that they associated with this status. This approval process is configured to:

* Require approval by the team&#39;s designer and copywriter
* Initiate whenever someone changes a work item&#39;s status to Ready for Printing

A brochure project owner attaches the Designer/ Copywriter Signoff approval process to the brochure project.

When someone on the project changes the status to Ready for Printing, the copywriter and designer receive notifications asking them to approve or reject it. During the approval process, when they are deliberating whether to approve it or not, the status of the projects displays as Ready for Printing - Pending Approval.

After they both approve the brochure in Workfront, the project status changes to Ready for Printing.

## Legacy document approval processes


Legacy document approvals are used for a more general approval. Feedback is captured in chat format on the Updates tab. You can use the approval buttons to approve, reject, or approve with changes.

To add approvers to a document after it&#39;s been uploaded to Workfront, see [Request a legacy document approval](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

>[!NOTE]
>
>There are currently several document approval options in Workfront. For more information, see [Available functionality for document approvals](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md).


## 验证审批流程

验证审批用于更深入的审查，通常包括更复杂的工作流。 反馈是通过验证查看者中的标记工具捕获的。 您可以使用批准按钮批准、拒绝或批准更改。

要将自动工作流添加到文档验证并指定工作流中的某些用户为验证的审批者，请参阅[使用自动工作流创建高级验证](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)。

## 配置工作项审批流程设置

作为Workfront管理员，您可以为系统中的工作项审批流程配置全局设置。 这些设置决定了批准流程的各种规则，例如允许批准决策保持打开状态的时间长度或如何在系统中管理批准委派。 有关审批流程设置的详细信息，请参阅[配置全局审批设置](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)。
