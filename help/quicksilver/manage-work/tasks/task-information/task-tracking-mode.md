---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任务跟踪模式概述
description: 在创建或编辑任务时，您可以调整任务的“跟踪模式”设置，以控制任务的“进度状态”指示器的显示方式和显示时间。 Adobe Workfront在您为跟踪任务进度配置某些设置时会显示进度状态标记。
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 3%

---

# 任务跟踪模式概述

在创建或编辑任务时，您可以调整任务的“跟踪模式”设置，以控制任务的“进度状态”指示器的显示方式和显示时间。 Adobe Workfront在您为跟踪任务进度配置某些设置时会显示进度状态标记。

有关任务进度状态的详细信息，请参阅 [任务进度状态概述](../../../manage-work/tasks/task-information/task-progress-status.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set Tracking Mode for tasks</h2>
<p>(NOTE: drafted, because we created a new article and linked it below. Left this article as a "Overview" article only.) </p>
<p>To set the tracking mode:</p>
<ol>
<li value="1">Go to the task you want to set the tracking mode for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png">next to the name of the task, then click&nbsp;<strong>Edit</strong>.</p> <p>The Edit Task dialog box opens. </p> </li>
<li value="3"> <p>In the&nbsp;<strong>Settings</strong> section, use the&nbsp;<strong>Tracking Mode</strong> drop-down menu to select the Tracking Mode for the task.</p> <p>For more information about the tracking mode options, see the <a href="#tracking-mode-options" class="MCXref xref" xrefformat="{para}">Tracking Mode options</a> section in this article. </p> </li>
<li value="4">Click&nbsp;<strong>Save Changes.</strong></li>
</ol>
</div>
-->

## 跟踪模式选项 {#tracking-mode-options}

作为任务所有者或项目经理，您可以选择Workfront如何指示每项任务的进度状态。 有关如何在任务中设置跟踪模式的信息，请参阅 [设置任务的跟踪模式](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

您可以从以下选项中进行选择：

* [用户必须更新](#user-must-update)
* [假设准时](#assume-on-time)
* [忽略迟到警告](#ignore-late-warnings)
* [自动完成](#auto-complete)
* [前置任务](#predecessor)

### 用户必须更新 {#user-must-update}

选择此选项后，Workfront将使用任务的“完成百分比”和“记录的实际小时数”来确定任务的“进度状态”。 这是默认选项。

### 假设准时 {#assume-on-time}

Workfront假定无论当前的完成状态如何，任务都将按时完成。 如果没有，则Workfront会自动假定下一个工作日的计划完成日期。 您仍必须指示任务何时完成。 当用户不会定期更新其任务时，请使用此选项。

### 忽略迟到警告 {#ignore-late-warnings}

任务的进度状态将保持为“按时”，直到它变为“延迟”。 例如，如果您将任务计划为10天，并在任务完成当天，该任务显示完成百分比为60%，则Workfront会通过添加4天来更新预计完成日期，而任务的进度状态将变为“延迟”。

### 自动完成 {#auto-complete}

Workfront假定任务将按计划完成，并在其到期或计划完成日期标记为完成。 在此之前，Workfront使用“完成百分比”和“实际记录的小时数”来确定进度状态。 但是，无论在计划完成日期之前处于进度状态，Workfront仍会标记任务已完成。

存在以下例外：

* 如果任务的前置任务不完整，则在所有前置任务完成之前，不会自动完成该任务。
* 如果任务具有“固定日期”约束，则无论其前置任务是否完成，任务始终在“计划完成日期”完成。

>[!IMPORTANT]
>
>如果选择任务自动完成，则在重新计算项目时间时，会将任务标记为完成。 如果项目的“更新类型”设置为“自动”或“自动”并且“更改时”，则每天都会计算项目时间轴。 有关项目时间轴重新计算的信息，请参阅 [重新计算项目时间表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).
>
>实际完成日期的时间是时间轴自动计算日期的午夜。 用于生成此时间戳的时间是您系统的时区，由您的Workfront管理员在“设置”的“客户信息”部分中定义。 有关设置系统时区的信息，请参阅 [配置系统的基本信息](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### 前置任务 {#predecessor}

Workfront根据其先前关系估计任务的预计完成日期。 任务的进度状态根据此估计确定。 例如，任务B的持续时间为1天，并计划在其前任任务A完成两天，该时间应为5天。 然后，用户将任务B更新为完成50%，但前身任务A尚未开始。 Workfront将从属任务B的完成时间安排在上一任务开始日期后6天，从而允许任务A为5天，任务B为1天。
