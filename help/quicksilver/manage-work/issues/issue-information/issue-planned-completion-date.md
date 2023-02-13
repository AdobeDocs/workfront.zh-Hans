---
product-area: projects
navigation-topic: issue-information
title: 计划完成日期问题概述
description: 发行的计划完成日期是预期发行完成的日期。
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# 计划完成日期问题概述

发行的计划完成日期是预期发行完成的日期。

您可以指定问题的计划完成日期，也可以将其留待Adobe Workfront根据特定条件计算。 

问题的计划完成日期不会影响项目的计划完成日期。 只有任务的计划完成日期会影响项目的计划完成日期。 有关项目计划完成日期的详细信息，请参阅 [设置项目计划完成日期](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>问题的计划完成日期与问题的提交日期或问题的预计完成日期有所不同，具体方式如下：
>
>* 提交日期是分配给问题的人员手动估计他们将完成问题的日期。 有关更多信息，请参阅以下文章：
   * [提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
   * [提交日期与计划完成日期之间的交互](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
* 预计完成日期是Workfront计算的日期，该日期考虑外部因素以确定实际可以完成问题的实际起始日期。 有关更多信息，请参阅 [项目、任务和问题的预计完成日期概览](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>


## 手动设置问题的计划完成日期

您必须对问题具有编辑访问权限并管理问题的权限，才能更新问题的计划完成日期。

您可以在Workfront的以下区域中手动设置问题的计划完成日期：

* 在“编辑问题”框或“问题详细信息”区域中创建或编辑问题。 有关信息，请参阅 [编辑问题](../../../manage-work/issues/manage-issues/edit-issues.md).
* 在“主页”区域中，如果查看问题时显示计划完成日期。 有关信息，请参阅 [在“主页”区域更新或编辑工作项](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* 在问题标题中。 有关信息，请参阅 [新对象标头](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* 在问题列表或报表中，“计划完成日期”字段显示在视图中。

   有关信息，请参阅 [编辑列表中的问题](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Workfront如何自动计算问题的计划完成日期

当Workfront自动计算发行的计划完成日期时，以下内容可能会影响该日期：

* 计划开始日期

   在您首次创建问题时，登入日期和计划开始日期应与问题相匹配。

* 在项目的“队列详细信息”部分中配置的默认持续时间。 有关信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   如果默认持续时间为0天，则计划完成日期与发行的计划开始日期匹配。

* 项目计划

自动设置后，计划完成日期将根据以下计算确定： 

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**示例：** 例如，如果您的任务的开始日期为1月14日星期五，而默认持续时间为5天，则计划完成日期为1月21日星期五，如果项目计划为星期一至星期五，每天8小时。

存在以下情况：

* 如果项目没有计划，则会考虑Workfront系统的默认计划。 有关信息，请参阅 [计划概述](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).
* 如果计划时间为星期一至星期五上午9点至下午1点（每天4小时），并且您的Workfront系统的每个工作日的典型小时数为8小时，则计划完成日期为1月27日。

>[!TIP]
Workfront在计算计划完成日期时会考虑计划例外，如节假日和周末。

 
