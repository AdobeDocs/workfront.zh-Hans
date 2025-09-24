---
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
title: 使用用户视图时查看资源规划者中的可用、计划和实际小时数或FTE
description: 在RP中使用用户视图计划时查看资源计划员中的可用小时数、计划小时数和实际小时数或FTE — 可能是“RP中的预算资源”或“RP中的管理资源”。 等…… — 或可能需要从其他POV重新调整用途?!)
author: LIsa
feature: Resource Management
exl-id: 6b532aa2-435f-4fda-b7ce-abe0a785638f
source-git-commit: 13621c29f32a514af46489fb58397f3e96f640ce
workflow-type: tm+mt
source-wordcount: '1739'
ht-degree: 1%

---

# 使用用户视图时查看资源规划者中的可用、计划和实际小时数或FTE

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Consider renaming this article (probably split already) to something other than "Planning" in the RP" - maybe "budgeting resources in the RP" or "Managing Resources in the RP." etc... - or might need to be repurposed from another POV?!)</p>
-->

除了在“项目”和“角色”视图中预算资源外，您还可以使用Adobe Workfront资源规划者的“用户视图”来显示有关项目和资源的已计划、可用和实际小时数或FTE值的信息。

## 资源规划者中的用户视图概览

在资源计划员中查看小时数或FTE信息时，请考虑以下事项：

* 您可以在资源规划者的所有视图中查看用户、工作角色和项目的可用和已计划小时数或FTE信息。
* 您只能在“用户视图”中查看以下信息：

   * 计划小时数或FTE数量与可用小时数或FTE数量之间的差额。 然后，您可以根据项目视图和角色视图中的此差异来预算用户分配。
   * 实际小时数或FTE。

* 您可以在“用户”视图中将“可用用户”与“计划小时数”或“FTE”之间的差额显示为数字或百分比值。
* 您不能在“按成本列出的用户”视图中显示此信息。
* Adobe Workfront根据用户在其时间表中关联的工作时间填充可用小时数或FTE。\
  未与计划关联的用户按照默认计划显示可用性。\
  有关默认计划的信息，请参阅[创建计划](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

* Workfront根据项目任务和问题的计划小时数信息填充计划小时数或FTE。
* Workfront使用分配给任务和问题的用户记录的实际时间填充实际小时数。 这包括项目的登录时间。
* 在“用户”视图中，您可以执行以下操作：

   * 展开每个用户以显示分配该用户的项目列表。

     >[!NOTE]
     >
     >只能展开与筛选器中包含的项目关联的用户。

   * 展开每个项目以显示用户可以在这些项目中完成的工作角色列表。
   * 展开每个角色以显示该角色中的用户所分配到的任务的列表。

  如果用户没有与其关联的工作角色，则其可用小时数、计划小时数和实际小时数或FTE将在&#x200B;**无角色**&#x200B;部分中列出。\
  有关将用户视图应用于资源规划者时显示的字段和项的信息，请参阅[资源规划者导航概述](../../resource-mgmt/resource-planning/resource-planner-navigation.md)中的“项目/角色/用户视图选择”部分。

## 资源规划者用户视图中可见的字段概述

请参阅下表以了解资源规划者的“用户”视图中显示的信息。 该信息以小时或FTE值显示。

* [AVL （可用）列](#the-avl-available-column)
* [计划（计划）列](#the-pln-planned-column)
* [ACT （实际）列](#The%C2%A0ACT)
* [DIF（差异）列](#the-dif-difference-column)
* [百分比（计划小时数分配百分比）列](#the-planned-hours-allocation-percentage-column)

### AVL（可用）列 {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>显示者</strong> </td> 
   <td> <p><strong>描述</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td>用户根据其计划可用的小时数或FTE总数。 </td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td>将用户视图应用于资源规划者时，此信息不可用于项目。 </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>根据用户的计划以及角色的<strong>FTE可用性百分比</strong>，角色的可用小时数或FTE总数。</p> </td> 
  </tr> 
  <tr> 
   <td>任务或问题</td> 
   <td>此信息不适用于任务或问题。 </td> 
  </tr> 
 </tbody> 
</table>

有关如何根据用户计划和角色的FTE可用性百分比计算用户和角色可用性的详细信息，请参阅[计算资源规划者中用户和角色的小时和FTE概览](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md)。

### PLN （计划）列 {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>显示者</strong> </td> 
   <td> <p><strong>描述</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td> 从所有项目上分配给用户的所有任务或问题中的总计划小时数或FTE。<br><p>这包括已分配给用户但与任何工作角色无关联的任务和问题，以及您有权管理的项目上没有的任务或问题。</p><p>当使用工作负载均衡器修改用户小时分配时，如果所选日期仅包含任务或问题的一部分，则资源规划者中的数据可能会受到影响。 有关修改用户分配的信息，请参阅<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作负载均衡器中管理用户分配</a> 。 </p></td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td> 分配给项目上特定用户的所有任务和问题的总计划小时数或FTE。<br><p>注意：这不包括未分配给任何用户的任务或问题中的计划小时数或FTE。 </p></td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>分配给项目中此角色的用户的所有任务和问题的总计划小时数或FTE。</p> <p> <p>注意：这不包括已分配给此角色但不分配给此角色中此用户的任务或问题的计划小时数或FTE。 </p> </p> </td> 
  </tr> 
  <tr> 
   <td>任务或问题</td> 
   <td>与项目中的任务或问题关联的计划小时数或FTE。</td> 
  </tr> 
 </tbody> 
</table>

查看计划小时数时，请考虑以下事项：

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view)</p>
-->

* 对于分配给任务的每个资源，已计划的小时数平均分配给任务和问题持续时间内的每一天。 任务或问题持续时间基于其计划的开始和完成日期，包括该时间段内的每个日历日。\
  在向用户或项目分配计划小时数时，Workfront会考虑用户或项目的计划。 在这种情况下，计划小时数平均分配到任务或问题持续时间内的每一天，不包括周末、休息日和计划例外。

  例如，如果按周显示资源规划者，并且您的任务在项目上跨越多周，则每周的计划小时数取决于该周内的多少天是任务持续时间的一部分。 在按月或季度显示资源规划者时以及任务跨越多个月或季度时，其工作方式类似。\
  周末日、计划例外和休息日将从此分配中排除。

* 计算每个资源的计划小时数时，包括以下任务类别：

   * 分配给资源池、工作角色或项目团队中用户的任务。

     >[!TIP]
     >
     >如果将任务分配给团队，则其分配将显示在&#x200B;**无角色**&#x200B;和&#x200B;**无用户**&#x200B;分区下。 您可以看到与团队关联的计划小时数，但无法预算小时数，因为没有任何角色或用户与任务关联。

* 资源规划者中的计划小时数不包括与以下项关联的计划小时数：

   * 父任务
   * 未分配任务
   * 问题，当&#x200B;**包括来自问题的小时数**&#x200B;设置禁用时。

* 如果任务或问题持续时间为零，则计划小时数未显示在资源规划者中。
* 未显示与已停用用户关联的计划小时数。

有关资源规划者中计划小时数和FTE的更多信息，请参阅资源规划者的项目和角色视图中的[小时数概述、FTE和成本信息](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)。

### ACT（实际）列

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>显示者</strong> </td> 
   <td> <p><strong>描述</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>用户 </td> 
   <td> <p>用户在分配给他们的所有任务或问题上记录的时间。</p> <p>这包括以下内容：</p> 
    <ul> 
     <li>分配给用户但不与任何工作角色相关联的任务和问题。</li> 
     <li>不在您有权管理的项目中的任务和问题。 </li> 
    </ul> <p>这包括仅当将用户分配给项目中的任务或问题时登录项目的时间。  </p> </td> 
  </tr> 
  <tr> 
   <td>项目 </td> 
   <td> <p>用户在项目上分配给他们的所有任务和问题记录的时间。</p> <p>这包括用户直接登录项目的任何时间。</p> <p>这不包括以下内容：</p> 
    <ul> 
     <li> <p>未分配给任何用户的任务和问题的登录时间。 </p> </li> 
     <li> <p>父任务登录时间。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>登录分配给此角色中用户的所有任务或问题的时间。 </p> <p>这不包括以下内容：</p> 
    <ul> 
     <li>登录分配给此角色但未分配给此角色中此用户的任务和问题的时间。</li> 
     <li>直接在项目或父任务上记录的时间。 </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>任务或问题 </td> 
   <td> <p>由也分配给任务和问题的用户登录这些任务和问题的时间。 </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>记录的时间显示在与小时条目的输入日期对应的时间范围内，而不管记录了小时数的任务、问题或项目的时间范围如何。

有关实际小时数的详细信息，请参阅[查看实际小时数](../../manage-work/tasks/task-information/actual-hours.md)。

### DIF（差异）列 {#the-dif-difference-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>显示者</strong> </td> 
   <td> <p><strong>描述</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td> <p>用户的可用小时数和计划小时数或FTE之间的差值。 </p> <p>小时或FTE差异使用以下公式计算：</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <p>注：如果值显示为负的红色数字，则表示用户分配过量。 </p> </p> </td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td>此信息不适用于项目。 </td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> <p>工作角色的可用小时数与计划小时数或FTE之间的差异。 </p> <p>小时或FTE差异使用以下公式计算：</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <p>注：如果值显示为负的红色数字，则职责分配过量。 </p> </p> </td> 
  </tr> 
  <tr> 
   <td>任务或问题</td> 
   <td>此信息不适用于任务、问题或项目。 </td> 
  </tr> 
 </tbody> 
</table>

### 百分比（计划小时数分配百分比）列 {#the-planned-hours-allocation-percentage-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>显示者</strong> </td> 
   <td> <p><strong>描述</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td> <p>计划小时数或FTE占可用小时数的百分比。 使用以下公式计算计划小时数分配的百分比：</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>FTE值使用相同的计算。 </p> </td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td>将<strong>按用户查看</strong>视图应用于资源规划者时，此信息不可用于项目。</td> 
  </tr> 
  <tr> 
   <td>角色</td> 
   <td> 计划小时数或FTE占可用小时数的百分比。 <p>使用以下公式计算计划小时数分配的百分比：</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>FTE值使用相同的计算。</p></td> 
  </tr> 
  <tr> 
   <td>任务或问题</td> 
   <td>此信息不适用于任务、问题或项目。 </td> 
  </tr> 
 </tbody> 
</table>

如果计划小时数或FTE的值为零，则百分比分配为0%。 如果可用小时数或FTE的值为零，则无法计算百分比分配。

有关计划小时数和FTE以及它们如何在资源规划程序中显示的详细信息，请参阅使用项目和角色视图的资源规划程序中的[预算资源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this table is ideal but it does not render in Markdown) </p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours or FTE)</strong> </td>
<td><strong>Displayed By</strong> </td>
<td> <p><strong>Description</strong> </p> </td>
</tr>
<tr>
<td rowspan="5">AVL <br>(Available Hours or FTE)</td>
<td>User</td>
<td>The total of Available Hours or FTE for the user according to their schedule. </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the User view to the Resource Planner. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Available Hours or FTE for the role according to the schedule of the user and the <strong>Percentage of FTE Availability</strong> of the role.</p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project.</td>
</tr>
<tr>
<td colspan="2"> <p colspan="2">For more information about how user and role availability is calculated based on the schedule of the user and the Percentage of FTE Availability of the role, see <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">PLN <br>(Planned Hours or FTE)</td>
<td>User</td>
<td> The total of Planned Hours or FTE from all the tasks or issues assigned to the user on all the projects.<br><p>This includes tasks and issues that are assigned to the user but not associated with any job role and tasks or issues that are not on projects that you have access to Manage.</p><p>When the user allocation for hours has been modified using the Workload Balancer, the data in the Resource Planner can be affected if the dates selected contain only a portion of a task or issue. For information about modifying allocations for users, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a> . </p></td>
</tr>
<tr>
<td>Project</td>
<td> The total of Planned Hours or FTE from all the tasks and issues assigned to a specific user on the project.<br><note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are not assigned to any users.
</note></td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Planned Hours or FTE from all the tasks and issues assigned to the user in this role on the project.</p> <p> <note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are assigned to this role but not to this user in this role.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>The Planned Hours or FTE associated with the task or the issue on the project.</td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view))</p>
<ul>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks and issues , for each resource assigned to them. The task or issue Duration is based on their Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks or issues excluding weekends, time-off days, and schedule exceptions.</p> <p>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> <p>The following categories of tasks are included in calculating the Planned Hours for each resource: </p>
<ul>
<li> <p> tasks assigned to users in Resource Pools, job roles, or teams on the project.</p> <note type="tip">
If tasks are assigned to teams, their allocation will appear under
<strong>No Role</strong> and
<strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks.
</note> </li>
</ul> </li>
</ul>
<ul>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>unassigned tasks</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task or issue Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> <p>For more information about Planned Hours and FTE in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">ACT<br>(Actual Hours or FTE) </td>
<td>User </td>
<td> <p>The time logged by the user on all the tasks or issues assigned to them.</p> <p>This includes the following:</p>
<ul>
<li>Tasks and issues that are assigned to the user but not associated with any job role.</li>
<li>Tasks and issues that are not on projects for which you have access to Manage.. </li>
</ul> <p>This does not include time logged directly on the project or on parent tasks. </p> </td>
</tr>
<tr>
<td>Project </td>
<td> <p>The time logged by the user on all the tasks and issues assigned to them on the project.</p> <p>This includes any time that they logged directly on the project.</p> <p>This does not include the following:</p>
<ul>
<li> <p>Time logged on tasks and issues that are not assigned to any users. </p> </li>
<li> <p>Time logged on parent tasks. </p> </li>
</ul> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The time logged on all the tasks or issues assigned to the user in this role. </p> <p>This does not include the following:</p>
<ul>
<li>Time logged on tasks and issues assigned to this role but not to this user in this role.<em> </em></li>
<li>Time logged directly on the project or parent tasks. </li>
</ul> </td>
</tr>
<tr>
<td>Task or Issue </td>
<td> <p>The time logged on tasks and issues by the user who is also assigned to them. </p> </td>
</tr>
<tr>
<td colspan="2"> <p> <note type="important">
The time logged is displayed in the timeframe corresponding to the Entry Date of the hour entry, regardless of the timeframe of the task, issue, or project where the hours are logged.
</note> </p> <p>For more information about Actual Hours, see <a href="../../manage-work/tasks/task-information/actual-hours.md" class="MCXref xref">View Actual Hours</a></p> </td>
</tr>
<tr>
<td rowspan="4">DIF <br>(Hour or FTE Difference) <br><br></td>
<td>User</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the user. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <note type="note">
If the value displays in negative red numbers, the user is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the job role. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <note type="note">
If the value is displayed in negative red numbers, the role is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td rowspan="5">Planned Hours or FTE Allocation Percentage (%)</td>
<td>User</td>
<td> <p>The allocation of the Planned Hours or FTE as a percentage of the Available Hours. The percentage of the Planned Hours Allocation is calculated using the following formula:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>The same calculation is used for FTE values. </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the <strong>View by User</strong> view to the Resource Planner.</td>
</tr>
<tr>
<td>Role</td>
<td> The allocation of the Planned Hours or FTE as a percentage of the Available Hours. <p>The percentage of the Planned Hours Allocation is calculated using the following formula:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>The same calculation is used for FTE values.</p></td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td colspan="2"> <p> If the value of the Planned Hours or FTE is zero, the Percentage Allocation is 0%. If the value of the Available Hours or FTE is zero, the Percentage Allocation cannot be calculated. </p> <p>For more information about Planned Hours and FTE and how they are displayed in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> </td>
</tr>
</tbody>
</table>
-->
