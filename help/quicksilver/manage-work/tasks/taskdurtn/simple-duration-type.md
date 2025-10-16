---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 持续时间类型概述：简单
description: 简单持续时间类型是一种持续时间类型，您可以在Adobe Workfront中为任务设置此类型。
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# 持续时间类型概述：简单

<!-- Audited: 5/2025 -->

简单持续时间类型是一种持续时间类型，您可以在Adobe Workfront中为任务设置此类型。 有关Workfront中持续时间类型的详细信息，请参阅[任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

## 简单持续时间类型概述

您的Workfront或组管理员可以将系统或组的默认持续时间类型设置为“简单”。 在这种情况下，将使用此持续时间类型创建所有新任务。

有关将任务和问题首选项作为系统级或组级项目首选项的一部分进行更改的信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

当任务的持续时间类型为简单时，会发生以下情况：

* 项目经理在修改任务工期和计划小时数在任务接受者之间的分配方式时，可以修改这些小时数。

  有关信息，请参阅[更新具有简单持续时间类型的任务的计划小时数和持续时间](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md)。

  >[!IMPORTANT]
  >
  >首次创建任务并为其分配简单持续时间类型但未指定持续时间时，Workfront会根据您为任务指定的已计划小时数计算任务的持续时间。 如果您手动修改简单持续时间任务的持续时间，Workfront将停止将计划小时数与持续时间匹配，因为它假定您要手动定义它们。
  >
  >Workfront使用以下公式计算未手动修改持续时间的任务持续时间：
  >
  > `Task Duration = Task Planned Hours / Typical hours per work day`
  >
  >您的Workfront管理员在实例设置的项目偏好设置区域中定义`Typical hours per work day`。

* 分配百分比已隐藏，但分配小时数可供编辑。
* 所有新客户的系统级别持续时间类型均设置为“简单”。

## 将任务的持续时间类型更改为简单

有关更改任务的持续时间类型的信息，请参阅[更新任务的持续时间类型](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Simple</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong><strong>.</strong></li>
</ol>
-->
