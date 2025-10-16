---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任务跟踪模式概述
description: 在创建或编辑任务时，您可以调整任务的“跟踪模式”设置，以控制任务的进度状态指示器的显示方式和时间。 当您配置某些设置以跟踪任务的进度时，Adobe Workfront会显示进度状态标记。
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 3%

---

# 任务跟踪模式概述

<!-- Audited: 01/2024 -->

在创建或编辑任务时，您可以调整任务的“跟踪模式”设置，以控制任务的进度状态指示器的显示方式和时间。 当您配置某些设置以跟踪任务的进度时，Adobe Workfront会显示进度状态标记。

有关任务进度状态的详细信息，请参阅[任务进度状态概述](../../../manage-work/tasks/task-information/task-progress-status.md)。

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

## “跟踪模式”选项 {#tracking-mode-options}

作为任务所有者或项目经理，您可以选择Workfront如何指示每个任务的进度状态。 有关如何设置任务的跟踪模式的信息，请参阅[为任务设置跟踪模式](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md)。

您可以从下列选项中进行选择：

* [用户必须更新](#user-must-update)
* [假设发生时间](#assume-on-time)
* [忽略迟到警告](#ignore-late-warnings)
* [自动完成](#auto-complete)
* [前置任务](#predecessor)

### 用户必须更新 {#user-must-update}

选择此选项时，Workfront使用任务的完成百分比和记录的实际小时数来确定任务的进度状态。 这是默认选项。

### 假设准时 {#assume-on-time}

Workfront假定任务将按时完成，而不考虑当前的完成状态。 如果任务未按时（在计划完成日期）完成，则Workfront会自动假定下一个工作日的计划完成日期。 您仍然必须指示任务何时完成。 当用户不会定期更新其任务时，可使用此选项。

### 忽略迟到警告 {#ignore-late-warnings}

任务的进度状态将为“准时”，直到变为“延迟”。 例如，如果您安排一项任务耗时10天，而任务在要完成的当天显示完成百分比为60%，则Workfront会添加四天来更新预计完成日期，并且任务的进度状态将变为“延迟”。

### 自动完成 {#auto-complete}

Workfront假定任务将按计划完成，并在其到期或计划完成日期将任务标记为完成。 在此之前，Workfront使用完成的百分比和记录的实际小时数来确定进度状态。 但是，无论在计划完成日期之前的进度状态如何，Workfront仍会将任务标记为已完成。

存在以下例外：

* 如果任务的前置任务不完整，则在完成所有前置任务之前不会自动完成该任务。 必须强制前置任务。
* 如果任务具有固定日期限制，则无论前置任务是否已完成，任务始终在计划完成日期完成。

>[!IMPORTANT]
>
>选择让任务自动完成会在重新计算项目时间时将任务标记为“完成”。 如果项目的“更新类型”设置为“自动”或“自动”且“发生更改”，则每天计算项目的时间表。 有关项目时间表重新计算的信息，请参阅[重新计算项目时间表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)。
>
>实际完成日期的时间是自动计算时间线的当天午夜。 按照Workfront管理员在设置的客户信息部分中的定义，用于生成此时间戳的时间是您系统的时区。 有关设置系统时区的信息，请参阅[配置系统的基本信息](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)。

### 前置任务 {#predecessor}

Workfront根据其前置任务关系估计任务的预计完成日期。 任务的“进度状态”是根据此估计确定的。 例如，任务B的工期为1天，并且计划在其前置任务A的两天后完成，这应需要5天。 然后，用户将任务B更新为已完成50%，但前置任务（任务A）尚未开始。 Workfront计划在前置任务开始日期后六天完成从属任务B，为任务A留出5天，为任务B留出1天。
