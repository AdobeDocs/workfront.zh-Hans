---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: 计算资源规划者中用户和角色的小时和FTE的概览
description: 计算资源规划者中用户和角色的小时数和FTE的概述
author: Lisa
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: 3c3175c347431b10aed1a6034df6c756056399b3
workflow-type: tm+mt
source-wordcount: '1392'
ht-degree: 0%

---

# 计算资源规划者中用户和角色的小时数和FTE的概述

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

您可以按小时数、FTE或成本在资源计划员中显示资源的分配和可用性。\
有关计算资源规划者中成本的更多信息，请参阅[计算资源规划者中的成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md)。

“FTE”表示相当于全职。 它是测量时间，表示用户或工作角色在一天或一周内用于实际工作的小时数。

以下资源信息集在资源规划者中的计算方式有所不同：

* 可用小时数或FTE值是根据系统管理员在系统中配置资源管理首选项的方式计算的。\
  有关如何计算可用小时数和FTE值的详细信息，请参阅[计算资源规划者中用户和工作角色的可用小时数或FTE](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner)。\
  有关为Adobe Workfront系统定义资源管理首选项的详细信息，请参阅[配置资源管理首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

* 所有其他FTE值都是根据“系统默认值”时间表计算的。\
  有关在使用FTE时所有其他值如何在资源规划者中显示的详细信息，请参阅本文中的[计算资源规划者中用户和工作角色的所有其他小时和FTE值](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner)部分。

了解每个用户及其工作角色的FTE是什么，以便在您为他们分配工作资源时准确地管理他们非常重要。

## 计算资源规划者中用户和工作角色的可用小时数或FTE {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

* [计算资源规划者中用户的可用小时数和FTE](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)
* [计算资源规划者中工作角色的可用小时数和FTE](#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner)
* [在资源规划程序中计算用户的可用小时数和FTE（示例）](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example)

### 在资源规划程序中计算用户的可用小时数和FTE {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

Workfront管理员通过在“设置”的“资源管理”区域中选择使用下列选项之一，来确定用户可用时间的计算方式：

* 系统的默认计划和用户的FTE。
* 用户的计划。

![用户计划的系统设置](assets/setup-resource-mgmt.png)

>[!NOTE]
>
>这决定了如何在系统级别计算资源可用性。 有关为系统定义资源管理首选项的详细信息，请参阅[配置资源管理首选项](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

根据此设置的配置方式，使用以下方法计算资源规划者中用户的可用性（小时数和FTE可用性）：

* **默认计划**：系统的默认计划和用户FTE用于确定资源规划者中用户的可用小时和FTE值。 用户的计划将被忽略。 在本例中：

   * 资源规划者中的&#x200B;**可用小时数**&#x200B;使用以下公式计算：

     `User Available Hours = Default Schedule Hours * User FTE value`

     例如，如果默认计划每周有40小时可用于工作，并且用户FTE为0.5，则用户可在资源规划者中每周工作20小时。

     有关计划（包括默认计划）的详细信息，请参阅[创建计划](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

   * 资源规划者中用户的&#x200B;**可用FTE**&#x200B;与用户设置中指定的用户FTE相同。

     例如，如果用户设置中的用户FTE为0.5，则用户在资源规划者中的可用FTE为0.5。 有关显示在用户设置中的用户FTE值的详细信息，请参阅[编辑用户配置文件](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

* **用户的计划**：用户的计划用于确定用户在资源规划者中的可用性。 忽略用户FTE的值。 在本例中：

   * 资源规划者中的&#x200B;**可用小时数**&#x200B;与用户计划中的小时数相同。

     例如，如果用户的计划每周有40小时可用于工作，则用户可在资源规划者中每周工作40小时。

   * 资源规划者中的&#x200B;**可用FTE**&#x200B;按以下公式计算：

     `User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours`

     例如，如果用户计划有20个小时工作可用，而Workfront中的默认计划有40个小时工作可用，则用户的FTE为0.5。

     有关计划（包括默认计划）的详细信息，请参阅[创建计划](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

>[!NOTE]
>
>如果用户未与时间表关联，则使用默认时间表计算用户的可用小时数。

### 计算资源规划者中工作角色的可用小时数和FTE {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

您首先必须计算用户可用性，然后可以计算每个工作角色的可用性。

资源规划者中工作角色的可用性考虑了用户的总可用性以及与用户的每个角色关联的&#x200B;**FTE可用性百分比**。\
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

有关将&#x200B;**FTE可用性百分比**&#x200B;值与用户的工作角色关联的更多信息，请参阅[编辑用户配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

例如，如果用户的“可用小时数”值为40，并且他们可以在75%的时间内完成一个主角色，在25%的时间内完成一个其他角色，则资源规划者显示一周的主角色的&#x200B;**可用小时数**&#x200B;值为30小时，而其他角色的&#x200B;**可用小时数**&#x200B;值为10小时。 在这种情况下，主角色的FTE为0.75，而另一个角色的FTE为0.25。

>[!NOTE]
>
>用户总可用时间通过本文资源规划者[&#128279;](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)部分中的计算用户的可用小时数和FTE中所述的两种方法之一来计算。

在角色视图中查看资源规划者时，一个工作角色的可用性是能够履行该工作角色的所有用户可用性的总和。\
有关资源规划者中资源可用性的详细信息，请参阅[资源规划者概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

### 在资源规划程序中计算用户的可用小时数和FTE（示例） {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

下表说明了如何在资源规划程序中为用户计算可用小时数和可用FTE，具体取决于系统管理员在资源管理首选项中用于FTE计算的方法。

在本例中，我们使用以下数字：

* 系统默认计划为40小时
* 20小时的用户计划
* 用户FTE为0.8

| FTE计算方法（系统设置） | 距用户计划&#x200B;**小时** | 距默认计划&#x200B;**小时** | **用户FTE字段** | 资源规划者中的&#x200B;**可用小时数** | 资源规划者中的&#x200B;**可用FTE** |
|---|---|---|---|---|---|
| **默认计划** | 已忽略 | 40 | 0.8 | **32**（已计算） | **0.8** |
| **用户的计划** | 20 | 40 | 已忽略 | **20** | **0.5**（已计算） |

计划例外和休息时间可能会影响计划小时数或FTE。 有关详细信息，请参阅[配置资源管理首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

按用户和小时数列出的示例资源规划者视图：

![资源规划者视图（按用户和小时）](assets/resource-planner-by-user-by-hours.png)

按用户和FTE列出的示例资源规划者视图：

![资源规划者视图（按用户和FTE）](assets/resource-planner-by-user-by-fte.png)

## 计算资源规划者中用户和工作角色的所有其他小时和FTE值 {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

除了可用小时数或FTE之外，以下时间信息也会显示在资源规划程序中：

* 规划小时数
* 预算小时
* 小时差异
* 净小时\
  有关这些值的详细信息，请参阅资源规划者的“项目”和“角色”视图中的[小时概览、FTE和成本信息](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

* 小时差异\
  有关此值表示什么的详细信息，请参阅资源规划者[&#128279;](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)的项目和角色视图中的小时概述、FTE和成本信息。

您可以在资源规划者中显示与FTE或小时相同的信息。

Workfront使用以下公式在资源规划者中将所有其他值显示为FTE：

`FTE = Resource Planner Hours/ Default Schedule Hours`

>[!NOTE]
>
>在计算资源规划者中所有值(可用(AVL) FTE值除外)的FTE时，将忽略用户的计划。 计算仅考虑默认计划。

此计算适用于以下值：

* 计划FTE (PLN)
* 预算FTE (BDG)
* FTE差异(VAR)
* 净FTE
* FTE差异(DIF)
