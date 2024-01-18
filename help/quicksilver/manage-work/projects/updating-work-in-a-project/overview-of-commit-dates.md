---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: 提交日期概述
description: 提交日期是指分配给任务或问题的用户承诺完成任务或问题的日期。 这与计划完成日期不同，因为它是仅由负责工作的用户提供的对完成日期的更现实的估计。 有关计划完成日期的信息，请参阅任务计划完成日期概览。
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 0%

---

# 提交日期概述

提交日期是指分配给任务或问题的用户承诺完成任务或问题的日期。 这与计划完成日期不同，因为它是仅由负责工作的用户提供的对完成日期的更现实的估计。 有关计划完成日期的信息，请参阅 [任务计划完成日期概览](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

## 提交日期概述

处理提交日期时，请考虑以下事项：

* 只有任务和问题具有提交日期。
* Adobe Workfront不会自动设置提交日期。\
  创建任务或问题时，没有向任务或问题分配提交日期。
* 如果分配给任务或问题，则可以通过执行以下操作之一来设置提交日期：

   * 允许Workfront通过单击任务或问题中的工作、开始问题或开始任务，将提交日期设置为与任务或问题的现有规划完成日期匹配。 有关将“处理此项工作”按钮替换为“开始”按钮的信息，请参阅  [将“处理此项工作”按钮替换为“开始”按钮](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * 根据您认为任务或问题可能完成的时间手动设置提交日期。 这是您作为工作负责人对项目经理的估计和承诺，即您将在特定日期前完成任务或问题。

>[!NOTE]
>
>您必须是任务的任务所有者才能更改提交日期。 以下用户无法更改任务的提交日期：
>
>* 项目所有者
>* 项目赞助者
>* 资源管理器
>* 系统管理员
>* 任务上的任何其他被分配人
>* 对任务具有权限的任何其他用户。
>
>有关任务所有者的详细信息，请参阅部分 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) 在文章中 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## 通过更改提交日期触发的通知和更新 {#notifications-and-updates-triggered-by-changing-the-commit-date}

当任务或问题被分配人选择与项目责任人设置的计划完成日期不同的提交日期时，会有许多通知和更新提醒项目责任人和其他用户此更改。

>[!NOTE]
>
>对提交日期所做的更改不会自动更改计划日期，对计划日期所做的更改不会自动更改提交日期。

为任务或问题设置提交日期会触发以下更改：

* 提交日期将填充在任务或问题的更新流中。

  ![](assets/update-stream-confirmation-that-commit-date-changed-nwe-350x73.png)

  当Workfront管理员在“设置”的“更新源”区域中启用此更新时，提交日期的更改会显示在任务或问题的更新区域中。 有关信息，请参阅 [系统跟踪更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

* 任务或问题的预计完成日期被设置为相同的日期，因为任务现在可以更准确地指示可能何时完成。

  有关预计完成日期的详细信息，请参阅 [项目、任务和问题的预计完成日期概述](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

  ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* 如果项目所有者使用旧版注释体验，则会在任务的更新选项卡中通知他们此更改是否会影响项目时间线，并让他们有机会更新同一区域中任务的规划完成日期。

  新的评论体验不支持此功能。 有关信息，请参阅 [新的评论体验](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

  >[!TIP]
  >
  >  项目所有者无权更新问题的规划完成日期，因为问题日期不会影响项目时间表。

  如果项目所有者不想接受更改，我们建议他们回访用户以建议一个新日期，要求他们将提交日期更改为原始计划日期，或选择一个新日期。 如果项目所有者接受更改，则可以手动调整计划完成日期，以匹配由分配给物料的用户提供的提交日期。 他们还可以单击 **将计划日期设置为： &lt;日期>** 在更新区域，该区域会自动设置规划完成日期以匹配新的提交日期。

  您必须具有管理任务和项目的权限才能接受此更改。

  >[!NOTE]
  >
  >如果您想了解接受更改任务的规划完成日期对项目时间线有何影响，请单击 **项目时间线**. 这将打开任务列表，您可以在其中评估日期更改和项目时间线。
  >
  >
  >![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >
  >

* 在“通知”区域中通知项目所有者，任务提交日期已更改。

  ![](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

  >[!TIP]
  >
  >只有当Workfront管理员在“设置”的“更新源”区域启用显示“提交日期”时，才会将提交日期已更改通知发送给项目所有者。 有关信息，请参阅 [系统跟踪更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).



有关更新工作项时可用的附加功能的信息，请参阅  [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

有关更新任务和问题的提交日期的信息，请参阅 [更新任务和问题的提交日期](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update Commit Dates on tasks and issues</h2>
<p>(NOTE: moved to its own article) </p>
<p>Updating the Commit Date is identical for tasks and issues.</p>
<ol>
<li value="1"> <p>Go to a task or issue that you are assigned to as the <strong>Task Owner</strong>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li>
<li value="2"> <p>Click Work on it in the task or issue header</p> <p>Or</p> <p>Click <strong>Start Task</strong> or <strong>Start Issue</strong> if the Work on it button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <strong>Undo</strong> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
The option to undo your selection to start your work is not available when you click
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>.
</note> </li>
<li value="4"> <p> Expand the <strong>This will be done by</strong> date picker, and select a new Commit Date.</p>
<div>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>Updates</strong> in the left panel, then click the <strong>Start a new update</strong>><strong>Commit Date</strong></p>
<p>Or</p>
<p>Click <strong>Task Details</strong> or <strong>Issue Details</strong> in the left panel, then double click <strong>Commit Date</strong> and select a new date from calendar. </p>
</div>
<p>The Commit Date and the Planned Completion date are no longer the same.</p>
<p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p>
<p>The changes are saved automatically.</p>
<p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifications-and-updates-triggered-by-changing-the-commit-date" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p>
</div> </li>
</ol>
</div>
-->
