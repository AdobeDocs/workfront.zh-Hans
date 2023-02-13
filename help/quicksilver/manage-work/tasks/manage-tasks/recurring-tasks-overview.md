---
content-type: overview
product-area: projects
keywords: 重复，重现，重现
navigation-topic: manage-tasks
title: 定期任务概述
description: 定期任务概述
author: Alina
feature: Work Management
exl-id: 9ddb75bf-1c7b-4f4b-b80b-a9512192920d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 3%

---

# 定期任务概述

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: DO NOT DO NOT EDIT OR CHANGE!!! linked to the NWE UI, this is not linked to classic - direct links:</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=workfront-classic</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=the-new-workfront-experience >> this)</p>
</div>
-->

您可以为必须在单个项目中重复的活动创建定期任务。

本文概述了有关创建和编辑循环任务的信息和注意事项。

有关如何在Adobe Workfront中创建定期任务的信息，请参阅 [创建定期任务](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).

## 定期任务概述和注意事项

您可以选择创建循环任务来指示项目生命周期中的可重复工作。

例如，在IT项目期间，可能需要定期备份软件。 为此活动创建定期任务可减少设置多个单独任务所需的时间。

在Workfront中创建定期任务时，请考虑以下事项：

* 不能向模板添加循环任务。
* 不能向现有任务添加重复频率。
* 循环任务显示为主要实例的子任务或子任务，主实例显示为父任务。
* 不能将批准附加到父定期任务。
* Workfront会将您在创建父级定期时更新的大多数字段传输到子级任务。 创建子任务时，以下字段不会转移到子任务：

   * 子任务的任务约束会自动更改为：

      * 对于从开始日期开始计划的项目，必须从开始。
      * 必须从完成日期开始计划的项目完成。
   * 附加到父项的文档不会传输给子项。


* 在指示该任务已重复后，父任务会发生以下更改：

   * 对于父任务，“持续时间”字段将重命名为“每次出现的持续时间”。 对于子任务，它仍保持持续时间。
   * 在父任务上状态处于禁用状态，并且在子任务上状态自动设置为“新建”。 父任务会自动完成，并且当所有子项都完成时，状态会更新为“完成”。
   * 可用于定期任务的持续时间类型仅包括：

      * 简单
      * 投入比导向

## 编辑定期任务的注意事项

您对循环任务父项所做的某些更改可能不会对所有现有的循环进行更新。 在更新父项时，显示进度或已单独更新的子项任务不会更新。 Workfront认为任务在以下情况下显示进度：

* 状态已更新，且任务不再为新任务
* 任务完成百分比大于零
* 该任务具有前身关系

下表说明了对父触发器所做的更改是否对尚未单独编辑的子级进行了更新或显示进度：

| 父任务更新的字段 | 更新了传输到未编辑的子项或子项，且未记录任何进度 |
|---|---|
| 循环频率* | ✔ |
| 分配&#42;&#42; | ✔ |
| 名称 | ✔ |
| 描述 | ✔ |
| 优先级 | ✔ |
| 持续时间 | ✔ |
| 计划小时 | ✔ |
| 成本类型 | ✔ |
| 收入类型 | ✔ |
| 资源均衡 | ✔ |
| 均衡延迟 | ✔ |
| 任务约束 | 不更新子项 |
| 附加或删除自定义Forms | 不更新子项 |
| 持续时间类型 | 不更新子项 |
| 自定义表单信息 | 不更新子项 |

{style=&quot;table-layout:auto&quot;}

&#42; 更新父任务的“重复频率”时，会出现以下情况：

* 如果更改现有父任务上的重复频率，则现有子任务将被删除，并替换为新子任务，这些子任务将遵循新的重复频率（如果它们未显示任何进度，或者您未手动更新它们）。
* 如果更改现有父任务上的重复频率，则不会删除显示进度的子任务。 此时，这些任务被视为与重复任务分开。

&#42;&#42; 对父任务进行的分配将应用于循环中的所有子任务。 对父任务上的分配所做的任何更改都会覆盖子任务上的任何单个分配。 如果任务显示进度，则分配不会更改。

 
