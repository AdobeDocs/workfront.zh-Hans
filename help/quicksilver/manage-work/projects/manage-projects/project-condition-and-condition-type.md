---
title: 项目条件和条件类型概述
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: 项目条件是项目进展情况的直观表示。 此为可报告变量，乃按项目计划、预计及估计日期之间之关系厘定。
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# 项目条件和条件类型概述

项目条件是项目进展情况的直观表示。 此为可报告变量，乃按项目计划、预计及估计日期之间之关系厘定。

## 项目条件概述

在了解项目的条件时，请考虑以下事项：

* 作为项目所有者，您可以决定是手动还是自动设置项目的条件。 可以通过以下方式设置项目的条件：

   * 手动（由有权访问“管理”项目的用户以及将项目的“条件类型”设置为“手动”时手动）。
   * 当项目的条件类型设置为进度状态时，由Adobe Workfront自动执行。 项目的进度状态取决于项目任务的进度。 有关项目进度状态的信息，请参阅 [项目进度状态概述](../../../manage-work/projects/planning-a-project/project-progress-status.md).

   有关如何更新项目的条件类型的信息，请参阅 [设置项目的条件类型](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md).

* 当允许Workfront自动估计项目的条件时，我们建议您在任务中使用前置任务，以便任务进度反映项目的实际进度和进度状态。
* 作为项目所有者，您可以通过将条件类型从“进度状态”更改为“手动”，将项目更改为“手动条件类型”，而不是“进度状态”。

   >[!NOTE]
   >
   >无论任务的日期和进度如何，处于以下任一状态的项目始终都会标记为On Target:
   >
   >* 想法
   >* 已请求
   >* 已批准
   >* 被拒绝


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set the Condition Type for a project</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted here and moved it to a separate article: /Content/Manage work/Projects/Manage projects/set-condition-type-for-project.htm)</p>
<ol>
<li value="1">Go to the project for which you want to update the Condition Type. </li>
<li value="2"> <p>  Click the <strong>More</strong> menu <img src="assets/qs-more-menu.png"> to the right of the project name, then click <strong>Edit</strong>.  <br> </p> </li>
<li value="3">In the <strong>Condition Type</strong> field, choose one of the following:
<ul>
<li><p><strong>Manual:</strong> The project owner sets the Condition on the project manually.</p><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In this case, the project owner can update the Condition of the project in the project header, or the Project Details section. </p></li>
<li><p><strong>Progress Status:</strong> Workfront sets the Condition based on the Progress Status of the project. <br></p></li>
</ul></li>
<li value="4">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Workfront如何根据进度状态更新项目条件

当项目的“条件类型”设置为“手动”时，您可以确定项目的“条件”状态与项目的“进度状态”无关。

但是，我们建议您将项目的条件类型设置为“进度状态”，以便您能够根据任务的进度清楚地了解项目的真正进度。 有关Workfront如何计算项目进度状态的信息，请参阅 [项目进度状态概述](../../../manage-work/projects/planning-a-project/project-progress-status.md).

在这种情况下，“项目条件”的值可以是：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>项目条件</td> 
   <td>项目进度状态</td> 
   <td>Workfront条件指示器</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>准时</td> 
   <td> <li>当项目按时进度状态时，项目的条件为 <strong>On Target</strong>.</li> </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>处于风险中</td> 
   <td>项目的进度状态为 <strong>后面</strong> 或 <strong>面临风险</strong>，则项目的条件为 <strong>面临风险</strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>存在问题</td> 
   <td>项目的进度状态为 <strong>延迟</strong>，则项目的条件为 <strong>遇到麻烦</strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>可以针对您的环境自定义条件，因此您可能会在您的环境中找到三个以上的“条件”选项。 “条件”的名称可能与上面所列的名称不同。 有关在中自定义条件的信息，请参阅文章 [创建或编辑自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## 报告项目条件、项目条件更新和最后条件说明

在项目报表的视图中，您可以显示与项目条件相关的以下字段：

* **项目条件：** 显示项目的当前条件。
* **项目条件更新**:显示项目所有者在项目更新流中提供的最新更新以及新条件。\
   在条件更新中做出的注释不会显示在 **条件更新** 列；只显示主更新。

* **最后条件说明**:显示对象所有者上次在对象上输入的更新。 此字段有助于显示所有者在对象上的最新活动或交互。\
   的 **最后条件说明** 列的空值。 当在对象上输入新注释时，该注释将成为最后一个注释，并再次显示在列中。

有关如何创建报表的信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
