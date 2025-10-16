---
product-area: projects
navigation-topic: manage-tasks
title: 在任务列表中保存并发更改的概览
description: 在列表中编辑任务时，可以使用单独的保存设置来指示在编辑列表中的任务时是否希望自动手动保存更改。
author: Alina
feature: Work Management
exl-id: dff52425-4711-40a8-8f40-205d75c506ef
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# 在任务列表中保存并发更改的概览

在列表中编辑任务时，可以使用单独的保存设置来指示在编辑列表中的任务时是否希望自动手动保存更改。

有关编辑任务列表中的任务的信息，请参阅文章[编辑列表中的任务](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)。

有时，如果两个用户更改了同一任务，则可能会出现冲突。

在任务列表中编辑任务时，请考虑以下事项：

* 如果项目更新类型为自动、自动或更改时，当您选择自动保存更改时，Adobe Workfront会立即保存您对任务所做的更改。 有关项目更新类型的信息，请参阅[选择项目更新类型](../../../manage-work/projects/manage-projects/select-project-update-type.md)。
* Workfront会使用其他用户可能在系统中的任何其他位置进行的更改来更新您每分钟都在处理的列表上的信息。 这可确保您始终获得有关任务的最新信息。

当多个用户编辑相同的任务时，会出现以下情况：

* **一个用户自动保存任务列表中的更改，另一个用户手动保存更改**：如果用户（用户A）在用户B编辑相同任务时手动保存更改，但自动保存更改，则用户B所做的实时更改每分钟会在用户A的列表中更新。 如果两个用户所做的更改之间存在冲突，则手动保存的用户（用户A）在保存更改之前会看到一条警告消息。 警告消息显示具有冲突更改的项目。 此时，用户A可以选择是保留更改（覆盖用户B所做的更改）还是放弃更改（保留用户B所做的更改）。

>[!NOTE]
>
>当您选择放弃所做的更改时，这适用于所有更改，而不仅仅适用于那些与另一用户所做的编辑有冲突的更改。

* **多个用户正在手动保存任务列表中的更改**：如果对列表中的任务进行更改的多个用户同时手动保存，则Workfront将保存最先保存的用户所做的更改。 保存这些更改不会遇到任何冲突。 然后，Workfront将所有其他用户所做的更改与它已经保存的信息进行比较，并在其他用户保存其信息之前显示关于冲突更改的警告。

>[!IMPORTANT]
>
>如果选择保留对所有其他更改所做的更改，则会保存所有更改，除非您对所做更改的任务被其他用户删除。 在这种情况下，警告消息会通知您对已删除的任务所做的更改已丢失。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
<p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - when replaced with the above live section; does it need an edit??) </p>
<div>
<p>When editing tasks in a list, you can select whether you want each change to be saved automatically or if you want to manually save multiple changes at one time by clicking the Save button. This depends on whether you enable the Autosave setting in the task list or not. </p>
<p>For information about editing tasks in a task list, see the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref" xrefformat="{para}">Edit tasks</a>. </p>
<p>Sometimes, conflicts might appear if two users are making changes on the same tasks. </p>
<p>Consider the following when editing tasks in a task list: </p>
<ul>
<li>Workfront saves the changes you make to tasks immediately when you have enabled the Autosave setting. </li>
<li>Workfront updates the information on the list you are working on every minute with changes that other users might make anywhere else in the system. This ensures that you always get the latest information on the tasks. </li>
</ul>
<p>The following scenarios exist when multiple users are editing the same tasks:</p>
<ul>
<li>One user has Autosave disabled and another has it enabled: If a user (User A) has disabled the Autosave setting and is editing the task list while User B is editing the same tasks but they have enabled the Autosave setting, the live changes made by User B are updated on the list for User A every minute. If there are conflicts between the changes made by the two users, the user with the Autosave setting disabled (User A) sees a warning message before they can save their changes, that shows the items that have those conflicting changes. At this time, User A can choose whether they should keep their changes (which overwrites the changes made by User B), or discard them (which keeps the changes made by User B.) </li>
</ul> <note type="note">
When you select to discard the changes you made, this applies to all the changes and not just to those that have conflicts with the edits made by another user.
</note>
<ul>
<li>Several users have disabled the Autosave setting: If several users that have disabled the Autosave setting are making changes at the same time, Workfront saves the changes made by the user who saves first. Saving these changes should not encounter any conflicts. Workfrontthen compares the changes made by all the other users with the information that it already saved and displays a warning about the conflicting changes to the other users before they can save their information. </li>
</ul> <note type="important">
When you select to keep your changes over all other changes, your changes are saved, unless the tasks you made changes to were deleted by another user. In this case, the warning message informs you that the changes you made to the deleted tasks are lost.
</note>
</div>
</div>
-->
