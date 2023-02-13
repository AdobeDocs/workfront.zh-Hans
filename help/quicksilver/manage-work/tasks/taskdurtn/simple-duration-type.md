---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: “持续时间类型概述：简单'
description: “简单持续时间类型”是可在Adobe Workfront中为任务设置的持续时间类型。 有关Workfront中持续时间类型的常规信息，请参阅任务持续时间和持续时间类型概述。
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# 持续时间类型概述：简单

“简单持续时间类型”是可在Adobe Workfront中为任务设置的持续时间类型。 有关Workfront中持续时间类型的常规信息，请参阅 [任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## 简单持续时间类型概述

您的Workfront或组管理员可以将系统或组的默认持续时间类型设置为简单。 在这种情况下，将使用此持续时间类型创建所有新任务。 有关更改任务和发布首选项作为系统级别或组级别项目首选项的一部分的信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

当任务的“持续时间”类型为“简单”时，会发生以下情况：

* 当修改任务分配给受分配者的时间时间时，项目经理可以修改任务的持续时间和计划时间。

   有关信息，请参阅 [使用简单持续时间类型更新任务的计划小时数和持续时间](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md).

   >[!IMPORTANT]
   >
   >当您首次创建任务并为其分配“简单持续时间类型”而未指定持续时间时，Workfront会根据您为任务指定的计划小时数来计算任务的持续时间。 如果您手动修改简单持续时间任务的持续时间，则Workfront会停止将计划小时数与持续时间匹配，因为它假定您要自行手动定义它们。

* 分配百分比处于隐藏状态，分配小时数可供编辑。
* 所有新客户的系统级别持续时间类型都设置为简单。

## 将任务的持续时间类型更改为简单

有关更改任务的持续时间类型的信息，请参阅 [更新任务的持续时间类型](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

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
