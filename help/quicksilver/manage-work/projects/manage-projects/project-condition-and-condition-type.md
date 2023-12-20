---
title: 项目完成情况和完成情况类型概览
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: 项目完成情况以可视化形式表示项目的进展情况。 此为可报告变数，由项目计划、预测及估计日期之间的关系厘定。
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: e4de185f172b173dcc3ad966afa69ffb3bc479eb
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# 项目完成情况和完成情况类型概览

<!-- Audited: 12/2023 -->

项目完成情况以可视化形式表示项目的进展情况。 此为可报告变数，由项目计划、预测及估计日期之间的关系厘定。

## 项目完成情况概述

在了解项目条件时，请考虑以下事项：

* 作为项目所有者，您可以决定是手动还是自动设置项目条件。 可通过以下方式设置项目的条件：

   * 由有权管理项目的用户手动执行，并且当项目的条件类型设置为手动时。
   * 当项目的“完成情况类型”设置为“进度状态”时，由Adobe Workfront自动执行。 项目的进度状态由项目上的任务进度决定。 有关项目进度状态的信息，请参阅 [项目进度状态概述](../../../manage-work/projects/planning-a-project/project-progress-status.md).

  有关如何更新项目条件类型的信息，请参阅 [设置项目的完成情况类型](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md).

* 当允许Workfront自动评估项目完成情况时，我们建议您在任务中使用前置任务，以便任务进度反映在实际进度和项目进度状态中。
* 作为项目所有者，您可以通过将条件类型从进度状态更改为手动来将项目更改为使用手动条件类型，而不是使用进度状态。

  >[!NOTE]
  >
  >无论任务的日期和进度如何，处于以下任意状态的项目始终被标记为On Target：
  >
  >* 想法
  >* 请求时间
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

## Workfront如何根据进度状态更新项目完成情况

当项目的条件类型设置为手动时，您可以确定项目的条件与项目的进度状态无关。

但是，我们建议您将项目的条件类型设置为进度状态，以便根据任务的进度，清楚地指示项目的真正进度。 有关Workfront如何计算项目进度状态的信息，请参阅 [项目进度状态概述](../../../manage-work/projects/planning-a-project/project-progress-status.md).

在这种情况下，项目条件的值可以是：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>项目完成情况</strong></td> 
   <td><strong>项目进度状态</strong></td> 
   <td><strong>Workfront条件指示器</strong></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>准时</td> 
   <td>当项目的进度状态为“按时”时，项目的完成条件为 <strong>准时</strong>. </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>处于风险中</td> 
   <td>当项目的进度状态为 <strong>滞后</strong> 或 <strong>处于风险</strong>，则项目的条件为 <strong>处于风险</strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>存在问题</td> 
   <td>当项目的进度状态为 <strong>晚的</strong>，则项目的条件为 <strong>存在问题</strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>可以为您的环境自定义条件，因此您可能会在环境中找到三个以上的条件选项。 条件的名称可能与上面列出的名称不同。 有关在中自定义条件的信息，请参阅文章 [创建或编辑自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## 项目完成情况报告、项目完成情况更新和上次完成情况说明

在项目报告的视图中，您可以显示与项目条件相关的以下字段：

* **项目完成情况：** 显示项目的当前完成情况。
* **项目完成情况更新**：显示项目所有者在项目的更新流中提供的最新更新以及新条件。\
  对条件更新所做的评论不会显示在 **完成情况更新** 列；仅显示主更新。

* **上次条件注释**：显示对象所有者上次在对象上输入的更新。 此字段有助于显示所有者对对象的最新活动或交互。\
  此 **上次条件注释** 如果删除了对象的最后一个注释的注释文本，则列为空。 在对象上输入新注解后，它将变成最后一个注解，并再次显示在列中。

有关如何创建报告的信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
