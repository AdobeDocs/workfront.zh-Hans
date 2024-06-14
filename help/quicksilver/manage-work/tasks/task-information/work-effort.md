---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 工作投入概述
description: 工作投入概述
author: Alina
feature: Work Management
exl-id: 70f51e4b-43cc-427a-99e4-ebb056bb1070
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 0%

---

# 工作投入概述

<!--Audited: 01/2024-->

<!--
(NOTE: Linked to the UI >> in the Project/ Template edit box > Tasks area> Learn more)
-->

作为项目经理，您可以决定如何估计要在项目中完成任务所需的工作量。 使用以下指标之一估计完成任务所需的工作量：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">规划小时数</td> 
   <td> <p> 手动数字输入或Adobe Workfront计算，显示分配给任务的资源完成任务所需的小时数。 </p> <p>考虑以下有关计划小时数的说明： </p> 
    <ul> 
     <li>这是默认方法。 </li> 
     <li>您只能为持续时间类型为“已计算分配”或“简单”的任务手动更新已计划小时数。 </li> 
    </ul> <p>有关计划小时数的信息，请参阅 <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">计划小时数概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">工作投入 </td> 
   <td> <p>手动标签，定义用户完成一项任务需要花费少量、中量还是大量日常工作。 <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The level of effort is estimated to be a percentage of the daily amount of working time. (NOTE: keep this drafted. Vazgen said it's not needed, but waiting for feedback from users)
      </MadCap:conditionalText>
     --> </p> <p>关于工作投入，请考虑以下事项：</p> 
    <ul> 
     <li>此字段仅适用于具有简单持续时间类型的任务。 </li> 
     <li>您可以启用此标签的使用，并在项目级别定义与其关联的工作时间百分比。 </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

本文介绍了什么是工作投入，以及在估计任务的工作量时应如何使用它。

>[!NOTE]
>
>计划小时数和工作投入会相互影响。 更新已计划小时数可以更新工作投入，更新工作投入可以更新任务的已计划小时数。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前：计划 </p>
   或
   <p>新增：标准 </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目和任务的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目及其任务的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关更多信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 使用工作投入的注意事项

* 当项目任务的计划小时数为0并且您启用使用工作投入以自动计算项目上的任务计划小时数设置时，与其关联的工作投入的默认级别将为中。 计划小时数会自动更新简单持续时间类型的任务。 有关更多信息，请参阅部分  [工作投入级别](#levels-of-work-effort) 本文章中。
* 当项目任务的计划小时数大于0并且您启用使用工作投入自动计算项目上的任务计划小时数设置时，工作投入级别根据计划小时数更新，而不更改简单持续时间类型任务的计划小时数。 有关更多信息，请参阅部分 [Workfront如何根据计划小时数计算工作投入](#how-workfront-calculates-work-effort-based-on-planned-hours) 本文章中。
* 当项目任务具有0个计划小时数，并且您启用使用工作投入以自动计算项目中的任务计划小时数设置，然后将工作投入级别从中更新为小或大时，计划小时数也会更新。 有关更多信息，请参阅部分 [Workfront如何根据工作投入计算已计划小时数](#how-workfront-calculates-planned-hours-based-on-work-effort) 本文章中。
* 当您内联编辑任务并同时修改任务的计划小时数和工作投入字段时，将使用您指定的值更新计划小时数，而工作投入值则根据您更新的计划小时数来计算。
* 当您更新任务的工作投入值时，持续时间不再基于计划小时数自动计算。 有关持续时间如何计算简单持续时间任务的详细信息，请参阅 [持续时间类型概述：简单](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).
* 当您将任务的持续时间类型从简单更改为任何其他类型时，任务上的工作投入字段会隐藏。 计划小时数保持不变。
* 您无法更新父任务的工作投入级别。 系统会根据任务的“已计划小时数”（所有子任务的汇总）自动计算父任务的工作投入级别。 有关父任务的信息，请参阅 [创建子任务](../../../manage-work/tasks/create-tasks/create-subtasks.md).

## 允许使用工作投入而不是计划小时数

1. 转到项目，然后单击 **更多** 菜单 ![](assets/more-icon.png)，然后单击 **编辑**.
1. 单击 **任务设置**，然后选择选项&#x200B;**使用工作投入以自动计算任务已计划小时数**. 默认情况下，该选项处于取消选中状态。

   ![](assets/nwe-work-effort-on-projects-350x182.png)

   有关在项目上启用工作投入使用的更多信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md) 文章。

1. 单击 **任务** ，然后单击任务的名称以访问它。
1. 单击 **更多** 菜单 ![](assets/more-icon.png)，然后单击 **编辑**. 确保任务具有简单的持续时间类型。

   >[!TIP]
   >
   >您也可以在任务详细信息部分中更新任务的工作投入。

1. 在 **概述** 区域，单击工作投入下拉菜单以更正完成任务所需的工作量。

   ![](assets/work-effort-on-edit-task-page-350x239.png)

   有关更新任务的工作投入字段的更多信息，请参阅以下文章：

   * 中的“概述”部分 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md) 文章
   * [在任务详细信息概述区域管理任务信息](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)

## 工作投入级别 {#levels-of-work-effort}

作为项目经理，您可以为项目确定三个级别的工作投入。 每个级别的工作量相当于用户完成任务所需的每日时间的百分比。

在设置工作投入级别时，您必须问自己以下问题：“分配给此任务的用户每天应花费多少时间才能按时完成任务？”

下表说明了工作投入的可能级别及其默认对应百分比。 作为项目经理，您可以更新百分比以满足组织的需求。 您可以在编辑项目时执行此操作。 有关编辑项目的信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

作为Workfront管理员，您可以在设置的项目偏好设置区域中定义每天的典型小时数。 这是视为工作时间的每日时间。 有关为Workfront实例配置项目首选项的信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

>[!NOTE]
>
>在下面的示例中，我们假设Workfront管理员已将每个工作日的典型小时数设置为8小时。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>工作投入级别</td> 
   <td>百分比值</td> 
  </tr> 
  <tr> 
   <td>小 </td> 
   <td>将完成任务的少量工作量设置为每天典型小时数的25%。 这意味着分配了此级别工作投入的任务应在一天内最多需要2小时才能完成。 <code>(0.25*8=2)</code></td> 
  </tr> 
  <tr> 
   <td>中</td> 
   <td> <p>完成任务的中等工作量设置为每天典型小时数的50%。 这意味着分配了此级别工作投入的任务应在一天内完成2个小时以上6个小时以内。 <code>(0.50*80=4)</code> </p> <p>注意：在项目上启用使用工作投入以自动计算任务计划小时数设置时，如果任务在启用此设置之前具有0个计划小时数，则此设置为任务的默认设置。 这会导致任务计划小时数更新为4小时。 </p> </td> 
  </tr> 
  <tr> 
   <td>大</td> 
   <td>将完成一项任务所需的大量工作量设置为每天典型小时数的75%。 这意味着分配了此级别工作投入的任务应需要6小时或更多时间才能在一天内完成。 <code>(0.75*8=6)</code></td> 
  </tr> 
 </tbody> 
</table>

## Workfront如何根据工作投入计算已计划小时数 {#how-workfront-calculates-planned-hours-based-on-work-effort}

当您启用使用工作投入以自动计算项目中的任务计划小时数设置时，Workfront使用以下公式计算具有简单持续时间类型的任务的计划小时数：

```
Task Planned Hours = Number of days in task Duration * Work Effort percentage * Typical hours per work day
```

例如，一项任务工期为3天，工作投入为中，其计划小时数为12：

```
Planned Hours = 3*4=12
```

其中，“每工作日典型小时数”值为8小时。

>[!TIP]
>
>当任务被分配给多个资源时，计划小时数会平均分配给每个资源任务持续时间的每一天。

## Workfront如何根据计划小时数计算工作投入 {#how-workfront-calculates-work-effort-based-on-planned-hours}

当您启用使用工作投入以自动计算项目上的任务已计划小时数设置并且您已有该任务的已计划小时数或者编辑该任务的已计划小时数时，Workfront会更新工作投入值。

Workfront使用以下公式根据计划小时数更新工作投入级别：

```
Work Effort level = Task Planned Hours / Duration / Typical hours per work day
```

例如，如果您的任务工期为2天，而您又将计划小时数从8小时更新为20小时，则该任务的工作量会从中等更新为大等：

```
Work Effort level = 20 / 2 / 8 = 125 % = Large
```

## 查找任务和项目的工作投入

* [项目的工作量](#work-effort-for-projects)
* [任务的工作投入](#work-effort-for-tasks)

### 项目的工作量 {#work-effort-for-projects}

您可以在以下区域找到项目上的工作投入部分：

* 编辑项目框中的任务设置区域

### 任务的工作投入 {#work-effort-for-tasks}

您可以在以下区域找到任务的工作投入字段：

* “编辑任务”框中的“概述”区域
* “任务详细信息”部分的“概述”区域，在工作时间区域
* 任务列表或报告
