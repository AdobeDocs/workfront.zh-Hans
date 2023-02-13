---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 工作概述
description: 工作概述
author: Alina
feature: Work Management
exl-id: 70f51e4b-43cc-427a-99e4-ebb056bb1070
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1512'
ht-degree: 0%

---

# 工作概述

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the UI >> in the Project/ Template edit box > Tasks area> Learn more) </p>
-->

作为项目经理，您可以决定如何估计任务在项目中完成所需的工作量。 使用下列指标之一估算完成任务所需的工作量：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">计划小时</td> 
   <td> <p> 手动数字输入或Adobe Workfront计算，用于显示分配给任务的资源完成该任务所花费的小时数。 </p> <p>请考虑以下有关计划小时数的事项： </p> 
    <ul> 
     <li>这是默认方法。 </li> 
     <li>您只能为持续时间类型为“计算分配”或“简单”的任务人工更新计划小时数。 </li> 
    </ul> <p>有关计划时数的信息，请参阅 <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">计划时数概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">工作投入 </td> 
   <td> <p>手动标签，用于定义用户完成某项任务所花费的日常工作量是中、小。 <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The level of effort is estimated to be a percentage of the daily amount of working time. (NOTE: keep this drafted. Vazgen said it's not needed, but waiting for feedback from users)
      </MadCap:conditionalText>
     --> </p> <p>请考虑以下有关工作量的信息：</p> 
    <ul> 
     <li>此字段仅适用于具有简单持续时间类型的任务。 </li> 
     <li>您可以启用此标签的使用，并定义在项目级别与其关联的工作时间百分比。 </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

本文介绍了工作量，以及在估算任务的工作量时应如何使用工作量。

>[!NOTE]
>
>计划工时和工作量相互影响。 更新计划工时可以更新工作工时，更新工作工时可以更新任务的计划工时。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目和任务的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目及其任务的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 使用工作量的注意事项

* 当项目任务具有0计划小时数，并且您启用使用工作量以自动计算项目上的任务计划小时数设置时，与它们关联的默认工作量级别将为中。 计划小时数会自动更新为简单持续时间类型任务。 有关更多信息，请参阅  [工作量](#levels-of-work-effort) 在本文中。
* 如果项目任务的计划小时数大于0，并且您启用“使用工作”以自动计算项目上的任务计划小时数设置，则工作量级别会根据计划小时数进行更新，而不会更改“简单持续时间类型”任务的计划小时数。 有关更多信息，请参阅 [Workfront如何根据计划时数计算工作量](#how-workfront-calculates-work-effort-based-on-planned-hours) 在本文中。
* 当项目任务具有0计划小时数，并且您启用“使用工作量”以自动计算项目上的任务计划小时数设置，然后将工作量级别从中到小或大更新时，计划小时数也会更新。 有关更多信息，请参阅 [Workfront如何根据工作量计算计划小时数](#how-workfront-calculates-planned-hours-based-on-work-effort) 在本文中。
* 当您在内联编辑任务并同时修改任务的“计划小时数”和“工作量”字段时，“计划小时数”将更新为您指定的值，而“工作量”值则根据您更新的“计划时数”计算。
* 更新任务的工作量值后，持续时间将不再根据计划小时数自动计算。 有关如何计算简单持续时间任务的持续时间的详细信息，请参阅 [持续时间类型概述：简单](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).
* 将任务的“持续时间类型”从“简单”更改为任何其他类型时，“工作”字段将隐藏在任务上。 计划时间保持不变。
* 您无法更新父任务的“工作”级别。 父任务的“工作量”级别会根据任务的“计划小时数”自动计算，该小时数是所有子任务的汇总。 有关父任务的信息，请参阅 [创建子任务](../../../manage-work/tasks/create-tasks/create-subtasks.md).

## 启用使用工作量而不是计划小时数

1. 转到项目并单击 **更多** 菜单 ![](assets/more-icon.png)，然后单击 **编辑**.
1. 单击 **任务设置**，然后选择选项&#x200B;**使用工作量自动计算任务计划时数**. 默认情况下，此选项处于取消选中状态。

   ![](assets/nwe-work-effort-on-projects-350x182.png)

   有关启用对项目工作的使用的更多信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md) 文章。

1. 单击 **任务** 在左侧面板中，单击任务的名称以访问该任务。
1. 单击 **更多** 菜单 ![](assets/more-icon.png)，然后单击 **编辑**. 确保任务具有简单持续时间类型。

   >[!TIP]
   >
   >您还可以在“任务详细信息”部分中更新任务的工作。

1. 在 **概述** 区域，单击工作工作下拉菜单以更正完成任务所需的工作量。

   ![](assets/work-effort-on-edit-task-page-350x239.png)

   有关更新任务的“工作”字段的详细信息，请参阅以下文章：

   * 中的“概述”部分 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md) 文章
   * [在“任务详细信息概览”区域中管理任务信息](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)

## 工作量 {#levels-of-work-effort}

作为项目经理，您可以为项目确定三个级别的工作量。 每个工作级别等于用户完成任务所需的每日时间的百分比。

在设置工作量时，您必须问自己一个问题：“分配给此任务的用户每天应该花多少时间来完成该任务？” 

下表说明了工作工作量的可能级别及其默认相应百分比。 作为项目经理，您可以更新百分比以满足贵组织的需求。 在编辑项目时执行此操作。 有关编辑项目的信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

作为Workfront管理员，您可以在“设置”的“项目首选项”区域中定义每个工作日的典型小时数。 这是被视为工作时间的每日时间。 有关为Workfront实例配置项目首选项的信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

>[!NOTE]
>
>在以下示例中，我们假定Workfront管理员已将每个工作日的典型小时数设置为8小时。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>工作量</td> 
   <td>百分比值</td> 
  </tr> 
  <tr> 
   <td>小 </td> 
   <td>完成任务所需的小量工作量设置为每天典型小时数的25%。 这意味着分配了此工作量的任务在一天内最多需要2小时才能完成。 <code>(0.25*8=2)</code></td> 
  </tr> 
  <tr> 
   <td>中</td> 
   <td> <p>完成任务所需的中等工作量设置为每天典型小时数的50%。 这意味着分配此工作量级别的任务一天内完成需要超过2小时且少于6小时。 <code>(0.50*80=4)</code> </p> <p>注意：在项目中启用“使用工作量自动计算任务计划时间”设置后，如果任务在启用此设置之前具有0个计划时间，则这是任务的默认设置。 这会导致“计划小时数”任务更新为4小时。 </p> </td> 
  </tr> 
  <tr> 
   <td>大</td> 
   <td>完成任务所需的大量工作量设置为每个工作日典型小时数的75%。 这意味着分配此工作量级别的任务需要6小时或更长的时间才能在一天内完成。 <code>(0.75*8=6)</code></td> 
  </tr> 
 </tbody> 
</table>

## Workfront如何根据工作量计算计划小时数 {#how-workfront-calculates-planned-hours-based-on-work-effort}

启用“使用工作量”以自动计算项目上的任务计划时间设置后，Workfront会使用以下公式计算具有简单持续时间类型的任务的计划时间数：

```
Task Planned Hours = Number of days in task Duration * Work Effort percentage * Typical hours per work day
```

例如，持续时间为3天且工作量为中的任务具有12个计划小时：

```
Planned Hours = 3*4=12
```

其中，每个工作日的典型小时数值为8小时。

>[!TIP]
>
>将任务分配到多个资源后，计划小时数将平均分配到任务持续时间的每一天的每个资源。

## Workfront如何根据计划时数计算工作量 {#how-workfront-calculates-work-effort-based-on-planned-hours}

启用“使用工作量”以自动计算项目上的任务计划小时数设置，并且任务上已有计划小时数，或者编辑任务上的计划小时数时，Workfront会更新工作量值。

Workfront使用以下公式根据计划时间更新工作量级别：

```
Work Effort level = Task Planned Hours / Duration / Typical hours per work day
```

例如，如果您的任务持续时间为2天，并且您将计划时间从8小时更新为20小时，则任务的工作量将从中型更新为大型：

```
Work Effort level = 20 / 2 / 8 = 125 % = Large
```

## 查找任务和项目的工作量

* [项目的工作成果](#work-effort-for-projects)
* [任务的工作量](#work-effort-for-tasks)

### 项目的工作成果 {#work-effort-for-projects}

您可以在以下区域找到项目的“工作”部分：

* “编辑项目”框中的“任务设置”区域

### 任务的工作量 {#work-effort-for-tasks}

您可以在以下区域中找到任务的“工作”字段：

* “编辑任务”框中的“概述”区域
* “任务详细信息”部分的“概述”区域，位于“工作时间”区域
* 任务列表或报表
