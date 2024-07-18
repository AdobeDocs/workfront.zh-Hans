---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '持续时间类型概述：计算分配'
description: 计算分配是一种持续时间类型，您可以在Adobe Workfront中为任务设置此类型。 有关Workfront中持续时间类型的一般信息，请参阅任务持续时间和持续时间类型概述。
author: Alina
feature: Work Management
exl-id: 5f1f6109-5d54-4c3f-9aa5-dc6ce165a1cd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# 持续时间类型概览：计算分配

计算分配是一种持续时间类型，您可以在Adobe Workfront中为任务设置此类型。 有关Workfront中持续时间类型的一般信息，请参阅[任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

## 计算分配持续时间类型概览

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This Hub issue has a powerpoint that highlights information that is useful to users when using Calculated Assignment duration type. I don't think we can use the powerpoint, because it's old. I also don't know if the things they discuss are still relevant, since the PP is from 2015. I've closed the issue, but I'm putting a link here just in case the info is useful. https://hub.workfront.com/issue/5a9dd7d5007d02a8966014557c23cc89/updates)</p>
-->

* 使用计算的分配持续时间类型时，必须为任务指定持续时间和计划小时数。 然后，Workfront将计划小时数除以持续时间中的小时数，再除以分配给任务的资源数，从而计算每个资源的分配百分比（计算分配）。 每个资源的分配百分比值都将相同。 在这种情况下，您无法修改每个资源的分配值。
* 您的Workfront或组管理员可以将系统或组的默认持续时间类型设置为计算分配。 在这种情况下，将使用此持续时间类型创建所有新任务。 有关将任务和问题首选项作为系统级或组级项目首选项的一部分进行更改的信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

  在这种情况下，任务的默认值为1天持续时间，默认值为0小时计划小时数。 除非项目经理设置更准确的持续时间并使用实际估计值填充计划小时数字段，否则资源似乎未充分分配。

在以下情况下，计算分配是首选的持续时间类型：

* 当分配具有活动窗口，但未完成其工作所分配的整个持续时间时。 例如，您被指定在周末之前向主管提交报表。 您有5天的持续时间，但您只需要10个小时即可草稿文档。
* 当由于项目经理可以相互独立地估计计划持续时间和计划工作量而将单个资源分配给任务时。

  您可以对相同结果使用计算的工作持续时间类型，但项目经理必须输入资源的百分比分配，才能影响计划小时数的计算值。 这使得项目规划更加困难和费时。

每项资源的分配百分比计算如下：

```
Planned Hours / Duration / Number of Resources = Allocation Percentage for each resource
```

例如，在下面列出的方案中，每个任务的持续时间均为3天。 项目经理人工输入持续时间（3天或24小时）和计划小时数，因此计算分配百分比（或分配百分比）：

![](assets/calcassign-350x80.png)

## 将任务的工期类型更改为计算的分配

有关更改任务的持续时间类型的信息，请参阅[更新任务的持续时间类型](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Assignment</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
