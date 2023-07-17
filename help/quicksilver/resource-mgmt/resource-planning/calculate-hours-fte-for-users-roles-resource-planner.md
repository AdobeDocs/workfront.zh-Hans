---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: 计算资源规划者中用户和角色的小时数和FTE的概览
description: 计算资源规划者中用户和角色的小时数和FTE的概览
author: Alina
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: 4331917d133c52cf727f148b75a213853c1e5679
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 1%

---

# 计算资源规划者中用户和角色的小时数和FTE的概览

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

您可以按小时、FTE或成本在资源计划程序中显示资源的分配和可用性。\
有关在资源规划程序中计算成本的详情，请参阅 [在资源规划者中计算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

“FTE”表示相当于全职。 它是一种时间度量，表示用户或工作角色在一天或一周中专用于实际工作的小时数。

以下资源信息集在资源计划程序中的计算方式不同：

* 可用小时数或FTE值是根据系统管理员在系统中配置资源管理首选项的方式计算的。\
  有关如何计算可用小时数和FTE值的更多信息，请参阅 [计算资源规划者中用户和工作角色的可用小时数或FTE](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner).\
  有关为Adobe Workfront系统定义资源管理首选项的更多信息，请参阅 [配置资源管理首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* 所有其他FTE值都是根据“系统默认值”时间表计算的。\
  有关在使用FTE时所有其他值如何在资源规划者中显示的信息，请参阅部分 [计算资源规划者中用户和工作角色的所有其他小时和FTE值](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner) 本文章中。

了解每个用户及其工作角色的FTE对于您分配他们的工作资源是非常重要的，这样可以准确地管理他们的资源。

## 计算资源规划者中用户和工作角色的可用小时数或FTE {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

* [在资源规划程序中计算用户的可用小时数和FTE](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)
* [计算资源规划者中工作角色的可用小时数和FTE](#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner)
* [在资源规划程序中计算用户的可用小时数和FTE（示例）](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example)

### 在资源规划程序中计算用户的可用小时数和FTE {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

Workfront管理员通过在“设置”的“资源管理”区域中选择使用下列选项之一，来确定用户可用时间的计算方式：

* 系统的默认计划和用户的FTE。
* 用户的计划。

有关更多信息，请参阅 [配置资源管理首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><br></p>
<p> <img src="assets/nwe-resource-management-system-setting-user's-schedule-350x157.png" style="width: 350;height: 157;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p>
<p>(NOTE: The determines how to calculate resource availability at the system level.For more information about defining the Resource Management preferences for the system, see Configure Resource Management preferences.)</p>
<p>Based on how this setting is configured, the availability of the users in the Resource Planner (hours as well as FTE availability) is calculated by using the following methods: </p>
<ul>
<li><strong>The Default Schedule</strong>: The Default Schedule of the system and the user FTE are used to determine the Available Hours and FTE value for the user in the Resource Planner. The Schedule of the user is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are calculated using the following formula:<br><code>User Available Hours = Default Schedule Hours * User FTE value</code> <span style="color: #dc143c;">( NOTE: this is the correct value. If this shows as a division in other articles, that is wrong. It's a multiplication between these 2 values).</span><br>For example, if the Default Schedule has 40 hours a week available for work, and the user FTE is 0.5, the user is available to work for 20 hours a week in the Resource Planner.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a></li>
<li style="font-weight: normal;"> The <strong>Available FTE</strong> for the user in the<strong>Resource Planner</strong> is the same as the user FTE specified in the user settings. <br>For example, if the user FTE is 0.5 in the user settings, the available FTE of the user is 0.5 in the Resource Planner. For more information about the value of the user FTE as it displays in the user settings, see <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.<br></li>
</ul></li>
<li><strong>The User's Schedule</strong>: The Schedule of the user is used to determine the availability of the user in the Resource Planner. The value of the user FTE is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are the same as the Hours from the Schedule of the user.<br>For example, if the Schedule of the user has 40 hours a week available for work, the user is available to work for 40 hours a week in the Resource Planner. </li>
<li> The <strong>Available FTE</strong> in the<strong>Resource Planner</strong> is calculated by the following formula:<br><em><code>User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code><br></em>For example, if the Schedule of the user has 20 hours available to work, and the Default Schedule in Workfront has 40 hours available to work, the user's FTE is 0.5.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li>
</ul></li>
</ul> <note type="note">
If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.
</note>
</div>
-->

### 计算资源规划者中工作角色的可用小时数和FTE {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

首先必须计算用户可用性，然后可以计算其每个工作角色的可用性。

资源规划者中工作角色的可用性会考虑用户的总可用性，并且 **FTE可用性的百分比** 与用户的每个角色相关联。\
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

有关关联的详细信息 **FTE可用性的百分比** 值以及用户的工作角色，请参见 [编辑用户配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

例如，如果用户的“可用小时数”值为40，并且他们可以在其中的75%时间内履行一个主要角色，并在其中的25%时间内履行一个其他角色，则资源规划者将显示 **可用小时数** “主要角色”一周的值是30小时，并且 **可用小时数** “其他角色”的值为10小时。 在这种情况下，主角色的FTE为0.75，而另一个角色的FTE为0.25。

>[!NOTE]
>
>用户总可用时间通过 [在资源规划程序中计算用户的可用小时数和FTE](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner) 章节。

在角色视图中查看资源规划者时，一个工作角色的可用性是能够履行该工作角色的所有用户的可用性总和。\
有关“资源规划程序”中资源可用性的详细信息，请参阅 [资源规划者概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### 在资源规划程序中计算用户的可用小时数和FTE（示例） {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

下表说明了如何在资源计划员中为用户计算可用小时数和可用FTE，具体取决于系统管理员在资源管理首选项中用于FTE计算的方法。

在本例中，我们使用以下数字：

* 40小时的系统默认计划
* 20小时的用户计划
* 用户FTE为0.75

| FTE计算方法（系统设置） | **距用户计划的小时数** | **距默认计划的小时数** | **用户FTE字段** | **资源规划者中的可用小时数** | **资源规划者中的可用FTE** |
|---|---|---|---|---|---|
| **默认计划** | 已忽略 | 40 | 0.75 | **30** （已计算） | **0.75** |
| **用户计划** | 20 | 40 | 已忽略 | **20** | **0.5** （已计算） |

计划例外和休息时间可能会影响计划小时数或FTE。 有关更多信息，请参阅 [配置资源管理首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## 计算资源规划者中用户和工作角色的所有其他小时和FTE值 {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

除了可用小时数或FTE之外，以下时间信息也会显示在资源计划员中：

* 计划小时
* 预算小时
* 小时差异
* 净小时\
  有关这些值的更多信息，请参阅 [资源计划员的“项目”和“角色”视图中的小时数、FTE和成本信息概览](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

* 小时差异\
  有关此值所表示内容的更多信息，请参阅 [资源计划员的“项目”和“角色”视图中的小时数、FTE和成本信息概览](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

您可以在资源规划者中显示与FTE或小时相同的信息。

Workfront使用以下公式在资源规划程序中以FTE形式显示所有其他值：

`FTE = Resource Planner Hours/ Default Schedule Hours`

>[!NOTE]
>
>在计算资源规划者中除可用(AVL) FTE值之外的所有值的FTE时，将忽略用户的计划。 计算仅考虑默认计划。

此计算适用于以下值：

* 计划FTE (PLN)
* 预算FTE (BDG)
* FTE差异(VAR)
* 净FTE
* FTE差异(DIF)
