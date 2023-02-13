---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: 智能分配概述
description: 在管理任务和问题分配时，您可以使用智能分配来确定最适合用户完成工作的人。 智能分配是在您根据算法将工作项分配给资源时Adobe Workfront向您提供的建议，算法可确定最适合该作业的资源。
author: Alina
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: 7e220e496aff2675910416bd86e3ddf7b9231afa
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# 智能分配概述

在管理任务和问题分配时，您可以使用智能分配来确定最适合用户完成工作的人。 智能分配是在您根据算法将工作项分配给资源时Adobe Workfront向您提供的建议，算法可确定最适合该作业的资源。

>[!NOTE]
>
>智能分配未考虑用户的可用性。 但是，根据任务的计划提供它们会影响任务和问题在分配时的计划日期和预计日期。 有关计划的信息，请参阅文章 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

本文包含有关智能分配的一般信息。 有关使用智能分配将任务和问题分配给用户的信息，请参阅 [进行智能分配](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md).

## 智能分配概述

使用智能分配时请考虑以下事项：

* 算法可独立处理任务和问题。 这意味着问题的建议用户列表可能与任务的建议用户列表不同，因为Workfront会根据与问题和任务相关的标准分别构建列表。
* 智能分配不推荐工作角色或团队。 相反，这些建议是最适合完成任务或问题的用户的建议。
* 建议的分配始终为活动用户。
* 最先列出的用户应该是该任务的最佳匹配。

## 找到智能分配建议

您可以在以下区域中查看智能分配，以便分配任务或问题：

* 任务或问题列表或报告

   ![](assets/smart-assignments-task-list-nwe-350x280.png)

* 任务或问题标题

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

* 任务或问题摘要面板

   ![](assets/smart-assignments-summary-panel-nwe-350x332.png)

* 在“主页”区域中列出的项目的“工作总揽”字段

   ![](assets/smart-assignments-in-home-nwe-350x216.png)


<!--removed for scheduling deprecation: 

* Resource Scheduling

  ![](assets/smart-assignments-scheduling-350x219.png)

  >[!CAUTION]
  >
  >Resource Scheduling is a deprecated feature. For more information, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* 工作负载均衡器

   ![](assets/smart-assignments-workload-balancer-bulk-assignments.png)


## 智能分配标准

智能分配会根据专有算法显示前50项推荐。

根据以下条件的组合（按从最重要到最不重要的顺序列出），在智能分配下拉列表中推荐用户：

* 过去30天内由进行分配的用户分配给其他工作项的用户。 将显示符合此标准的前50个用户。 最常被分配的用户将首先显示。

   如果将工作项分配给团队或角色，则会进一步过滤建议用户的列表，同时考虑下面现有的分配。 在这种情况下，建议列表中仅显示以下用户：

   * 其“主团队”是分配给工作项的团队的用户。
   * “主角色”是分配给工作项的角色的用户。

      >[!TIP]
      >
      >* 如果 <!--you're not part of any team and --> 没有为任务或问题分配角色或团队，Workfront会显示过去30天（最多50个用户）分配的所有用户。
      >* 如果您在过去30天内未进行任何分配，则只有属于已分配团队或已分配了工作项角色的用户才会显示在智能分配列表中。


<!--the commented out piece in the tip above was live before but I am not totally sure that smart assignments look at your team. I think they look JUST at the team/ role assigned to the work item; see this help site request for more info: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/62fd222200037eb87572c5b6ad6bf53e/overview -->
<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h3>Smart assignments criteria for the Production environment</h3>
<p>(NOTE: drafted,this was the case BEFORE we updated the logic in the WB - with the 21.4 release)</p>
</div>
<p>Smart assignments display on tasks and issues when the following conditions are met:</p>
<ul>
<li>The task or issue is subordinate to a parent task or issue that has a user, team, or job role currently assigned. </li>
</ul>
<p>Smart assignments display the top twenty recommendations based on a proprietary algorithm that uses your own team information.</p>
<p>Users are recommended in the smart assignments drop-down list based on a combination of the following criteria (listed in order from most important to least important):</p>
<ul>
<li>The user has the team assigned to the task or issue designated as their Home Team</li>
<li>The user is also assigned to the parent task</li>
<li>The user has the same primary job role as is currently assigned to the task or issue</li>
<li>The user has the team assigned to the parent task or issue designated as their Home Team</li>
<li>The user is associated with the same primary job role currently assigned to the parent task</li>
<li>The user is a member of the same team as the user who assigned the task or issue and the team is designated as their Home Team</li>
<li>The user is a member of the same Home Group as the user who is assigning the task or issue</li>
<li>The user has the same primary job role as the user who is assigning the task or issue.</li>
</ul>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Make smart assignments</h2>
<p>(NOTE:&nbsp;this was moved to its own article: make-smart-assignments.) </p>
<p>Smart assignments are available in most locations where you can make assignments in Workfront.</p>
<p>You can use smart assignments on tasks and issues that have previously been assigned to a job role or a team.</p> <note type="note">
You must have a Plan or a Work license and have at least Contribute permissions to a task or an issue to be able to make assignments to the task or the issue. You must have the Make Assignments option enabled in your permission level to make assignments.
</note>
<p>To use smart assignments:</p>
<ol>
<li value="1">Navigate to an issue or a task and click one of the following fields to edit them: <br>
<ul>
<li><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The <strong>Assignments</strong> field in the task or issue header</p></li>
<li>The <strong>Assignments</strong> field of a task or issue list using in-line editing in a task or issue list. </li>
<li>The <strong>Assignee</strong> field after you have clicked <strong>Advanced</strong> from a task or an issue. </li>
</ul></li>
<li value="2"> <p>Place your cursor in the assignment field, and wait for two seconds, then the <strong>Suggestions</strong> list is displayed.</p> <p>Users displayed in this list are the smart assignment suggestions for the task or the issue.<br></p> <p> <img src="assets/nwe-smart-assignment-suggestions-350x160.png" style="width: 350;height: 160;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p>Select the user in the recommendations list by clicking their name. </p> <p>If there are no suggestions, the suggestion list does not open.</p> </li>
<li value="4">(Optional) If you do not want to use one of the recommended users from the smart assignments list, start typing the name of the desired user and select the name when it appears in the list.</li>
<li value="5">Click <strong>Enter</strong> to make the assignment. </li>
</ol>
</div>
-->
