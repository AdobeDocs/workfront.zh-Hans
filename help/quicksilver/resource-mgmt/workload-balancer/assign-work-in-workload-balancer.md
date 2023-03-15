---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 工作负载平衡器中分配工作的概述
description: 作为资源管理器，您可以使用Adobe Workfront工作负载平衡器来查看尚未分配给用户的工作项，并将这些项分配给用户。
author: Alina
feature: Resource Management
exl-id: 98779b67-b975-4501-8426-63e255b1d7df
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 0%

---

# 工作负载平衡器中分配工作的概述

作为资源管理器，您可以使用Adobe Workfront工作负载平衡器来查看尚未分配给用户的工作项，并将这些项分配给用户。

有关工作负载平衡器的一般信息，请参阅 [工作负载平衡器概述](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

您可以将工作项（任务和问题）分配给Workfront其他区域的用户。 但是，通过使用工作负载平衡器，您可以轻松地了解用户的可用性，并在为他们分配更多工作之前清楚地看到他们分配到的所有其他项目。

有关在Workfront其他区域分配工作项的信息，请参阅以下文章：

* [分配任务](../../manage-work/tasks/assign-tasks/assign-tasks.md)
* [分配问题](../../manage-work/issues/manage-issues/assign-issues.md)

## 工作负载平衡器中的用户可用性

您可以在负载平衡器中分配工作以匹配用户的可用时间。 为确保您分配正确的工作量而不是过度分配用户，分配给用户的工作项的计划小时总数必须与用户的每日或每周分配相匹配。

您必须了解Workfront如何计算用户的可用时间。

Workfront使用以下信息在负载平衡器中计算用户的容量：

* 资源管理首选项。 Workfront管理员通过选择在“设置”的“资源管理”区域中使用以下任一选项来确定系统的可用时间计算方式：

   * Workfront系统的默认计划和用户的FTE。
   * 用户的计划，如“用户配置文件”区域中所示。

      这会计算用户的每日和每周可用性。 所选计划的任何计划例外都反映在负载平衡器中用户的容量中。
   有关更多信息，请参阅 [配置资源管理首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

   有关计划的信息，请参阅 [创建计划](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

* 用户的休息时间。 这表示用户计划起飞的日期。

   有关更多信息，请参阅 [在Adobe Workfront中配置个人休息时间](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* 用户的工作时间。 这表示用户可用于执行实际项目相关工作（不包括间接费用）的FTE时间百分比。 将“工作时间”值设置为1，以指示用户可用于与项目相关的工作，且其整个全时对等工作。


## 在工作负载平衡器中分配工作

您可以分配尚未分配给用户的工作项，或重新分配已分配给负载平衡器中用户的项。

可以通过以下方式在工作负载平衡器中分配工作：

* 通过手动分配每个项目，一次只分配一个项目。

   在人工分配项目时，您可以一次进行一次高级分配。

   有关更多信息，请参阅 [使用工作负载平衡器手动分配工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

* 通过将工作项拖放到需要分配的用户，一次只需一个项目。

   有关更多信息，请参阅 [通过拖放在工作负载平衡器中分配工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md).

* 使用“批量分配”选项，一次可处理多个项目。 您可以定义规则，以便将项目一次分配给多个用户。

   有关更多信息，请参阅 [使用工作负载平衡器批量分配工作](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

有关取消分配工作的信息，请参阅 [在负载平衡器中取消分配工作](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

## 工作负载平衡器中的分配区域

您可以在“资源”区域、项目或团队级别使用负载平衡器将工作分配给用户。 有关工作负载平衡器在Workfront中的位置的详细信息，请参阅 [找到工作负载平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

工作负载平衡器中有两个区域，您可以在其中查看工作项：

* **未分配的工作**:显示未分配给用户的项目。
* **分配的工作**:显示分配给用户的项目。

下表描述了根据项目的分配在每个区域中显示哪些项目：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>分配类型</strong> </td> 
   <td colspan="2"><strong>分配可见的区域</strong> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td>未分派工作 </td> 
   <td>已分派工作 </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span style="font-weight: normal;">未分配项目</span> </td> 
   <td><span>✔</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>团队</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span data-mc-edit-date="2020-04-08T15:57:40.7175506-04:00" data-mc-editor="alinawilson" data-mc-comment="Drafted because role only is not displayed; first it will be displayed in Unassigned - 20.2 beta" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:24:04.5189150-05:00">角色</span> </td> 
   <td><span>✔</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>角色和团队</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>用户和团队</td> 
   <td> <p> </p> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>用户、角色和团队</td> 
   <td>✔*</td> 
   <td>✔**</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>用户和角色</p> </td> 
   <td><span data-mc-edit-date="2019-11-15T13:37:42.5435254-05:00" data-mc-editor="alinawilson" data-mc-comment="drafted because it's not in the Unassigned" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:37:33.3097484-05:00">✔</span>*</td> 
   <td>✔**</td> 
  </tr> 
 </tbody> 
</table>

&#42;将工作项分配给用户和角色后，只有在角色是主要代理人时，它才会显示在“未分配的工作”区域中。

&#42;&#42;将工作项分配给用户和其他实体后，只有当用户是主要代理人时，它才会显示在“已分配的工作”区域中。

有关负载平衡器的“未分配”和“已分配”区域的详细信息，请参阅 [导航工作负载平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 对工作角色、团队和用户进行多种分配的注意事项

在为工作项分配多个资源时，请考虑以下事项：

* 用户可以拥有与其配置文件关联的多个作业角色。 有关将用户与作业角色关联的信息，请参阅 [编辑用户的配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 任务或问题通常首先分配给一个或多个作业角色或团队。 当项目准备好启动时，可能还需要将它们分配给用户。\
   如果任务或问题被分配到一个或多个角色，然后您又分配了一个用户，则Adobe Workfront会根据以下规则确定要与附加用户关联的作业角色（如果有）：

   * 如果只分配了一个作业角色，并且该角色与用户的主角色相匹配，则该任务或问题将仅分配给执行其主角色的用户。
   * 如果分配了多个角色，并且其中至少一个角色与用户的辅助角色匹配，则任务或问题会分配给执行其中一个其他角色(如果存在多个匹配，Workfront将随机选择)的用户，以及分配的任何其他角色。
   * 如果分配了一个或多个作业角色，并且与用户的角色没有匹配，则任务或问题将分配给角色或角色以及用户。

* 如果任务或问题被分配给团队，并且您也分配了用户，则任务或问题仍会同时分配给团队和用户。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2 data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Manually assign one item at a time</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Moved manual assignment and drag-and-drop to their own articles) </p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items</p> <p>Or</p> <p>Go to the <strong>Assigned Work</strong> area and expand the name of a user to view the work items assigned to them.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area. You can only reassign issues already assigned to users in the Assigned Work area. Otherwise,</span> you can assign issues from a list or at the issue level. For information, see
<a href="../../manage-work/issues/manage-issues/assign-issues.md" class="MCXref xref">Assign issues</a>.
</note> </li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> on the bar of a work item, then click <strong>Assign this to</strong>. </p> <p> <img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"> </p> <note type="tip">
<p><span>You can also use the following shortcuts to assign tasks or issues:</span> </p>
<ul>
<li><span>In Windows: CTRL+click the task or issue bar.</span> </li>
<li><span>In&nbsp;Mac: CMD+click the task or issue bar.</span> </li>
</ul>
</note> </li>
<li value="4"> <p>Start typing the name of a user, job role, or team that you want to assign to the item in the <strong>Search people, role or teams</strong> field, select it when it displays in the list, then click&nbsp;<strong>Save</strong>. </p> <p> <img src="assets/assignments-box-wb.png"> </p> <p>This assigns or reassigns the work item to the specified assignees.</p> <p>If you assign an item to just a team or a job role, the item displays only in the Unassigned Work area. You must assign work items to users in order to display them in the Assigned Work area of the Workload Balancer.</p> <note type="tip">
<p>You can assign multiple users or job roles, and you can assign only one team. <span>You can assign only active users, <span>job roles</span>, and teams.</span></p>
<p><span>If a user, <span>job role</span>, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:</span> </p>
<ul>
<li> <p><span>Reassign the work item to active resources.</span> </p> </li>
<li> <p><span>Associate the users in a deactivated team with an active team and reassign the work item to the active team.</span> </p> </li>
</ul>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>.</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2>Assign an item by dragging and dropping</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider retitling this to "Assign one item at a time by dragging and dropping" when bulk assignments will come???)&nbsp;</p>
<p>You can assign an item from the Unassigned Work area to a user, or you can reassign an already assigned item to another user in the Assigned Work area.</p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area.</span>
</note> </li>
<li value="3"> <p>Click the bar of a work item that indicates either the planned or the projected timeline and drag it over the name of a user in the <strong>Assigned</strong> area.</p> <p>The user you hover over to drop the work item to is highlighted.</p> <note type="tip">
The Planned Hours for the user you're hovering over update in real time with the number of daily Planned Hours from the work item, to indicate what the impact of adding a new item might be to their overall allocation.
</note> <p> <img src="assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png" style="width: 350;height: 152;"> </p> </li>
<li value="4"> <p>When you are ready, drop the selected work item in the same line as the user's name in the Assigned Area. The item is assigned and the allocated Planned Hours are updated for the user with the new hours from the work item.</p> <note type="tip">
<p>If you enabled Group by Project in the Settings area, the assigned task displays under the corresponding project. If the setting is disabled, the assigned task displays in the user area. </p>
<p>The item displays according to the Workload Balancer criteria for sorting work items.&nbsp;For more information, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>. (NOTE: make sure these are still called this, and that the icon has not changed)</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol> 
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Assign items in bulk</h2>
<p>(NOTE: This is also a separate article. Should we keep this section or the separate article?) </p>
</div>
<p>&nbsp;</p>
</div>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Unassign work items in the Workload Balancer</h2>
<p>(NOTE: moved this section to a new article. Draft here at release to preview) </p>
<p>You can either unassign items from users and move them to the Unassigned Work area, or reassign them to other users. </p>
<p>To unassign work items from users: </p>
<ol>
<li value="1">In the Workload Balancer, go to the <strong>Assigned Work</strong> area and expand a user.</li>
<li value="2">Do 
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
one of
</MadCap:conditionalText>
the following:
<ul>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Find the item you want to unassign in a user's area, click it, drag and drop it in the Unassigned area or in another user's area. </p></li>
<li><p>Click the <strong>More</strong> icon <img src="assets/more-icon-task-list.png"> to the right of the name of a work item, click&nbsp;<strong>Assign this to</strong> , then remove the name of the entities assigned to the work item or enter another name and click&nbsp;<strong>Save</strong>.</p><p><img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"></p></li>
</ul><p>The item displays in the Unassigned Work area if it matches the filtering criteria for that area and it is not assigned to any users or it displays in the user area if it is assigned to that user. </p><note type="tip">
Unassigned issues do not display in the Unassigned area.
</note><p>For information about filtering information in the Workload Balancer, see <a href="../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md" class="MCXref xref">Manage filters in the Workload Balancer</a>. </p></li>
</ol>
</div>
-->
