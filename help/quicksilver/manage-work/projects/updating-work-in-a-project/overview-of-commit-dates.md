---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: 提交日期概述
description: “提交日期”是指分配给任务或问题的用户提交完成任务或问题的日期。 这与计划完成日期不同，因为它是仅由负责工作的用户提供的完成日期的更实际估计。 有关计划完成日期的信息，请参阅：任务计划完成日期概览
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# 提交日期概述

“提交日期”是指分配给任务或问题的用户提交完成任务或问题的日期。 这与计划完成日期不同，因为它是仅由负责工作的用户提供的完成日期的更实际估计。 有关计划完成日期的信息，请参阅 [任务计划完成日期概览](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

## 提交日期概述

使用提交日期时，请考虑以下事项：

* 只有任务和问题具有提交日期。
* 提交日期不会由Adobe Workfront自动设置。\
   创建任务或问题时，未为任务或问题分配提交日期。
* 如果您被分配到任务或问题，则可以通过执行以下操作之一来设置提交日期：

   * 通过单击任务或问题上的“处理任务”、“开始问题”或“开始任务”，让Workfront设置“提交日期”以匹配任务或问题的现有计划完成日期。 有关将“Work On It（处理）”按钮替换为“Start（开始）”按钮的信息，请参阅  [将“Work On It（处理它）”按钮替换为“Start（开始）”按钮](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * 根据您认为任务或问题可能已完成的时间，自行手动设置提交日期。 这是作为受让人，您对项目经理的估计和承诺，即任务或问题将在特定日期之前完成。

>[!NOTE]
>
>您必须是任务的任务所有者才能更改提交日期。 以下用户无法更改任务的提交日期：
>
>* 项目所有者
>* 项目赞助者
>* 资源管理器
>* 系统管理员
>* 任何其他任务受让人
>* 具有任务权限的任何其他用户。
>
>有关任务所有者的详细信息，请参阅部分 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) 在文章中 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## 通过更改提交日期触发的通知和更新 {#notifications-and-updates-triggered-by-changing-the-commit-date}

当任务或问题受分配人选择的提交日期与项目责任人设置的计划完成日期不同时，会有许多通知和更新，提醒项目责任人和其他用户进行此更改。

>[!NOTE]
>
>对提交日期所做的更改不会自动更改计划日期，对计划日期所做的更改不会自动更改提交日期。 

设置任务或问题的提交日期会触发以下更改：

* 提交日期填充任务或问题的更新流中的。

   ![](assets/update-stream-confirmation-that-commit-date-changed-nwe-350x73.png)

   当Workfront管理员在“设置”的“更新馈送”区域中启用此更新时，“提交日期”的更改将显示在任务或问题的“更新”区域中。 有关信息，请参阅 [系统跟踪的更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

* 任务或问题的预计完成日期设置为同一日期，因为任务现在可以更准确地指示完成时间。

   有关预计完成日期的详细信息，请参阅 [项目、任务和问题的预计完成日期概览](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

   ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* 在任务的通知区域和更新选项卡中，系统会通知项目所有者此更改是否会影响项目时间轴。

   ![](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

   >[!TIP]
   只有当Workfront管理员启用在“设置”的“更新馈送”区域中显示“提交日期”时，“提交日期已更改”通知才会发送给项目所有者。 有关信息，请参阅 [系统跟踪的更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

   如果项目所有者不想接受更改，我们建议他们向建议新日期的用户做出评论，要求他们将提交日期更改回原始计划日期，或选择新日期。 如果项目所有者接受更改，则他们可以手动调整计划完成日期，以匹配分配给物料的用户提供的提交日期。

   项目责任人可以使用提交日期重置计划完成日期。 为此，请在任务的“更新”选项卡中选择“将计划日期设置为”选项。 您必须有权管理任务，并且项目有权接受此更改。

   >[!NOTE]
   如果要查看接受更改任务的计划完成日期对项目时间轴有何影响，请单击 **项目时间轴**. 此时将打开甘特图，您可以在其中评估日期更改。
   ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >

有关更新工作项时可用的其他功能的信息，请参阅  [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

有关更新任务和问题的提交日期的信息，请参阅 [更新任务和问题的提交日期](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update Commit Dates on tasks and issues</h2>
<p>(NOTE:&nbsp;moved to its own article) </p>
<p>Updating the Commit Date is identical for tasks and issues.</p>
<ol>
<li value="1"> <p>Go to a task or issue that you are assigned to as the <strong>Task Owner</strong>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li>
<li value="2"> <p>Click Work on it in the task or issue header</p> <p>Or</p> <p>Click <strong>Start Task</strong> or <strong>Start Issue</strong> if the Work on it button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <strong>Undo</strong> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On&nbsp;It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
The option to undo your selection to start your work is not available when you click
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>.
</note> </li>
<li value="4"> <p> Expand the <strong>This will be done by</strong> date picker, and select a new Commit Date.</p>
<div>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>Updates</strong> in the left panel, then click the <strong>Start a new update</strong>><strong>Commit Date</strong></p>
<p>Or</p>
<p>Click <strong>Task Details</strong> or <strong>Issue Details</strong> in the left panel, then double click&nbsp;<strong>Commit Date</strong> and select a new date from calendar. </p>
</div>
<p>The Commit Date and the Planned Completion date are no longer the same.</p>
<p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p>
<p>The changes are saved automatically.</p>
<p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifications-and-updates-triggered-by-changing-the-commit-date" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p>
</div> </li>
</ol>
</div>
-->
