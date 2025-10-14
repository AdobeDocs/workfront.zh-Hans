---
content-type: overview
navigation-topic: the-new-workfront-experience
title: 对象标题概述
description: 查看对象标题时，可以一目了然地查看 [!DNL Adobe Workfront] 中的对象信息。 标题中的信息可以包括对象的所有者、状态或完成百分比。
feature: Get Started with Workfront
author: Courtney
exl-id: 76e21df0-9272-4bfb-8a97-c16ae5f4b5dc
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '3697'
ht-degree: 0%

---

# 对象标题概述

查看对象标题时，可以一眼查看[!DNL Adobe Workfront]中的对象信息。

除了对象名称之外，标题还可以包含对象的所有者、状态或完成百分比。

[!DNL Workfront]为对象名称赋予优先权，在标题中为其分配尽可能多的空间。 当对象名称太长时，该对象名称会被截断。 要显示对象的全名，您可以将鼠标悬停在该对象上。

## 访问对象的标头

访问[!DNL Workfront]中对象的标头对于具有该标头的所有对象都是相同的。

例如，要访问项目的标头，请执行以下操作：

1. 转到项目。\
   标题显示在页面顶部，并包含项目的名称。

   ![](assets/project-header-350x18.png)

<!--## [!UICONTROL Home] header overview 

The following headers are available in Home:

* Task: For more information on how you can use this header, see the [Task header overview](#task-header-overview) in this article.
* Issue: For more information on how you can use this header, see the [Issue header overview](#issue-header-overview) in this article.-->

## 可自定义的标题

您的[!DNL Workfront]或组管理员可以使用布局模板自定义项目、任务和问题的标题。

本文介绍了所有对象的默认标头，包括项目、任务和问题。

有关自定义对象标题的信息，请参阅[使用布局模板自定义对象标题](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。


## 项目标题概述

![](assets/project-header-350x18.png)

默认情况下，项目标题会显示以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>标题信息</th> 
   <th>注释</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">具有父对象的痕迹导航</td> 
   <td>如果项目与项目群或项目组合关联，则它们会显示在标题左上角的痕迹导航中。 单击父对象的名称将打开该父对象。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">对象图标 </td> 
   <td> <p>紫色的[!UICONTROL 项目]图标<img src="assets/nwe-projects-icon.png">显示在项目名称的左侧。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">项目名称</td> 
   <td>您可以在标题中编辑项目名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象类型的名称</td> 
   <td> <p>文本“[!UICONTROL PROJECT]”显示在标题中项目名称上方。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">项目的操作区域</td> 
   <td> <p>在项目名称旁边，将显示包含<b>共享</b>选项的操作区域。</p> <p> <img src="assets/actions-area-icons-with-share-button.png"> </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 完成百分比]</td> 
   <td>您无法在标题中编辑项目完成百分比。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 项目所有者]</td> 
   <td> <p>您可以在标题中编辑[!UICONTROL 项目所有者] 。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 计划完成日期] </td> 
   <td> <p>如果项目计划开始于[!UICONTROL 完成日期]，您可以在标题中编辑项目[!UICONTROL 规划完成日期]和时间。 如果从[!UICONTROL 开始日期]开始计划项目，则会从项目中的任务更新此信息。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 条件] </td> 
   <td> <p>将项目的[!UICONTROL Condition Type]设置为“手动”时，可以在标题中更新项目[!UICONTROL Condition]。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 状态]</td> 
   <td>您可以在标题中编辑项目[!UICONTROL 状态] 。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Approvals]区域</td> 
   <td> <p>如果您是批准者之一，请使用以下图标管理项目的批准：</p> <p> <img src="assets/nwe-approvals-approve-16x18.png" style="width: 16;height: 18;"> </img> [!UICONTROL 批准]</p> <p> <img src="assets/nwe-approvals-reject-16x19.png" style="width: 16;height: 19;"> </img> [!UICONTROL 拒绝]</p> <p> <img src="assets/nwe-approvals-recall-16x16.png" style="width: 16;height: 16;"> </img> [!UICONTROL 撤消]</p> <p>如果您不是审批者，请单击[!UICONTROL 更多]图标<img src="assets/more-icon-for-approvals-area.png">查看有关当前审批步骤的信息。</p> <p>要了解有关审批的更多信息，请参阅<a href="../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">审批流程概述</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 任务标题概述

![](assets/task-header-350x18.png)

默认情况下，任务标题包括以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>标题信息</th> 
   <th>注释</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">具有父对象的痕迹导航</td> 
   <td> <p>任务的父对象显示在痕迹导航中。 单击父对象的名称将打开该父对象。</p> <p>有关详细信息，请参阅<a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">痕迹导航概述</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">对象图标 </td> 
   <td> <p>任务名称的左侧将显示绿色的[!UICONTROL 任务]图标<img src="assets/nwe-tasks-icon.png">。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">任务名称</td> 
   <td>您可以在标题中编辑任务名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象类型的名称</td> 
   <td> <p>文本“[!UICONTROL TASK]”显示在标题中任务名称的上方。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">任务的操作区域</td> 
   <td> <p>在任务名称旁边，将显示包含<b>共享</b>选项的操作区域。</p> <p> <img src="assets/actions-area-icons-with-share-button.png"> </p> <p>如果显示“依赖项”图标，您可以单击该图标查看任务的任何前置任务或后续任务。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 完成百分比]</td> 
   <td>您可以在标题中编辑任务完成百分比。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 分配]</td> 
   <td>您可以从标题中编辑任务的被分配人。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Work on It]、[!UICONTROL Done]或[!UICONTROL Start Task]按钮</p> </td> 
   <td> <p>如果任务分配给您，则可以单击[!UICONTROL 处理该任务] <span>或[!UICONTROL 开始任务]</span>按钮指示您正在处理该任务，或单击[!UICONTROL 完成]按钮指示您完成了任务。</p> <p><span>有关将[!UICONTROL 处理此项工作]按钮替换为[!UICONTROL 开始任务]按钮的信息，请参阅<a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">将[!UICONTROL 处理此项工作]按钮替换为[!UICONTROL 开始]按钮</a></span>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 计划完成日期]</td> 
   <td> <p>您可以在标题中编辑任务[!UICONTROL 规划完成日期] <span>和时间</span>。</p> <p>提示：请注意，[!UICONTROL 提交日期]在标头中不可见。 您可以在[!UICONTROL 详细信息]页面上查看它。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 状态]</td> 
   <td>您可以在标题中编辑任务[!UICONTROL 状态] 。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Approvals]区域</td> 
   <td> <p>如果您是批准者之一，请使用以下图标管理任务的批准：</p> <p> <img src="assets/nwe-approvals-approve-16x18.png" style="width: 16;height: 18;"> </img> [!UICONTROL 批准]</p> <p> <img src="assets/nwe-approvals-reject-16x19.png" style="width: 16;height: 19;"> </img> [!UICONTROL 拒绝]</p> <p> <img src="assets/nwe-approvals-recall-16x16.png" style="width: 16;height: 16;"> </img> [!UICONTROL 撤消]</p> <p>如果您不是审批者，请单击[!UICONTROL 更多]图标<img src="assets/more-icon-for-approvals-area.png">查看有关当前审批步骤的信息。</p> <p>要了解有关审批的更多信息，请参阅<a href="../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">审批流程概述</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 问题标题概述

![](assets/issue-header-350x19.png)

默认情况下，问题标题包含以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>标题信息</th> 
   <th>注释</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">具有父对象的痕迹导航</td> 
   <td> <p>问题的父对象显示在痕迹导航中。 单击父对象的名称将打开该父对象。</p> <p>有关详细信息，请参阅<a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">痕迹导航概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象图标 </td> 
   <td> <p>问题名称的左侧将显示粉红色[!UICONTROL 问题]图标<img src="assets/nwe-issues-icon.png">。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">问题名称</td> 
   <td>您可以在标题中编辑问题名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象类型的名称</td> 
   <td> <p>文本“[!UICONTROL ISSUE]”显示在标题中问题名称上方。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">问题的操作区域</td> 
   <td> <p>在问题名称旁边，将显示包含<b>共享</b>选项的操作区域。</p> <p> <img src="assets/actions-area-icons-with-share-button.png"> <p>如果显示[!UICONTROL 依赖项]图标，您可以单击该图标以查看该问题的任何前置任务或后续任务。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 完成百分比]</td> 
   <td> <p>您可以从标题编辑问题的完成百分比。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 分配]</td> 
   <td>您可以从标题中编辑问题的被分配人。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 处理它]、[!UICONTROL 完成]、<span>或[!UICONTROL 开始问题]按钮</span></td> 
   <td>如果问题分配给您，则可以单击[!UICONTROL 处理问题] <span>或[!UICONTROL 开始问题]</span>按钮指示您正在处理问题，或单击[!UICONTROL 完成]按钮指示您已完成问题。<span>有关将[!UICONTROL 处理此项工作]按钮替换为[!UICONTROL 开始任务]按钮的信息，请参阅</span> <span href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">将[!UICONTROL 处理此项工作]按钮替换为[!UICONTROL 开始]按钮</a></span><span>。</span></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 计划完成日期]</td> 
   <td> <p>您可以在标题中编辑问题[!UICONTROL 规划完成日期] <span>和时间</span>。</p> <p>提示：请注意，[!UICONTROL 提交日期]在标头中不可见。 您可以在[!UICONTROL 详细信息]页面上查看它。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 状态]</td> 
   <td>您可以在标题中编辑问题[!UICONTROL 状态]。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Approvals]区域</td> 
   <td> <p>如果您是批准者之一，请使用以下图标管理问题的批准：</p> <p> <img src="assets/nwe-approvals-approve-16x18.png" style="width: 16;height: 18;"> [!UICONTROL 批准]</p> <p> <img src="assets/nwe-approvals-reject-16x19.png" style="width: 16;height: 19;"> [!UICONTROL 拒绝]</p> <p> <img src="assets/nwe-approvals-recall-16x16.png" style="width: 16;height: 16;"> [!UICONTROL 召回]</p> <p>如果您不是审批者，请单击[!UICONTROL 更多]图标<img src="assets/more-icon-for-approvals-area.png">查看有关当前审批步骤的信息。</p> <p>要了解有关审批的更多信息，请参阅<a href="../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">审批流程概述</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 项目标题概述

![](assets/program-header-350x18.png)

项目群标题显示以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>标题信息</th> 
   <th>注释</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Portfolio名称的痕迹导航</td> 
   <td> <p>您可以从[!UICONTROL Program]的标头访问[!UICONTROL Portfolio]。 单击父对象的名称将打开该父对象。</p> <p>有关详细信息，请参阅<a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">痕迹导航概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象图标 </td> 
   <td> <p>橙色[!UICONTROL 项目]图标<img src="assets/nwe-programs-icon.png">显示在项目名称的左侧。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">项目的名称</td> 
   <td>您可以在标题中编辑项目名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象类型的名称</td> 
   <td> <p>如果程序标记为[!UICONTROL 活动]，则文本“[!UICONTROL PROGRAM]”将显示在标题中程序名称上方。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">激活状态</td> 
   <td> <p>如果项目已停用，则标题中项目名称上方会显示文本“[!UICONTROL PROGRAM DEACTIVATED]”。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">计划的操作区域</td> 
   <td> <p>在程序名旁边，将显示包含<b>共享</b>选项的操作区域。</p> <p> <img src="assets/actions-area-icons-with-share-button.png"> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 完成百分比]</td> 
   <td> <p>您无法在标题中编辑项目的[!UICONTROL 完成百分比]。 将从项目群的项目中更新此信息。</p> <p>提示：默认情况下，项目的完成百分比是属于该项目的[!UICONTROL 当前]或[!UICONTROL 批准状态]中项目的完成百分比值的平均值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 项目管理器]</td> 
   <td> <p>您可以在标题中编辑[!UICONTROL 项目管理器]。 这与[!UICONTROL 项目所有者]相同。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 计划完成日期]</td> 
   <td>您无法在标题中编辑项目[!UICONTROL 规划完成日期]。 此信息更新自项目群中项目的[!UICONTROL 规划完成日期]。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 活动项目条件]</td> 
   <td>这是计算将[!UICONTROL Condition]设置为[!UICONTROL On Target]、[!UICONTROL At Risk]或[!UICONTROL In Trouble]的程序中活动项目的百分比。</td> 
  </tr> 
 </tbody> 
</table>

## Portfolio标题概述 {#portfolio-header-overview}

![](assets/portfolio-header-350x19.png)

项目组合标题包括以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>标题信息</th> 
   <th>注释</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">对象图标 </td> 
   <td> <p>项目组合名称的左侧将显示蓝色的[!UICONTROL Portfolio]图标<img src="assets/nwe-portfolios-icon.png">。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">项目组合的名称</td> 
   <td>您可以在标题中编辑项目组合名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象类型的名称</td> 
   <td> <p>如果项目组合标记为活动，则标题中的项目组合名称上方会显示文本“[!UICONTROL PORTFOLIO]”。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">激活状态</td> 
   <td> <p>如果项目组合已停用，则标题中的项目组合名称上方会显示文本“[!UICONTROL PORTFOLIO DEACTIVATED]”。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">项目组合的操作区域</td> 
   <td> <p>在项目组合名称的旁边，将显示[!UICONTROL actions]区域。</p> <p> <img src="assets/actions-area-icons-with-share-button.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Portfolio Manager]</td> 
   <td>您可以在标题中编辑[!UICONTROL Portfolio Manager] 。 这与[!UICONTROL Portfolio Owner]相同。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL On Time]</td> 
   <td>这是计算项目组合中项目当前准时的百分比。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL On Budget]</td> 
   <td>这是计算项目组合中目前预算内的项目百分比。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 对齐]</td> 
   <td>这是计算项目组合中项目与项目组合一致的百分比。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ROI]</td> 
   <td>这是对项目组合中所有项目的[!UICONTROL 投资回报率]的计算。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 净值]</td> 
   <td>这是项目组合中所有项目的[!UICONTROL 净值]计算。</td> 
  </tr> 
 </tbody> 
</table>

## 模板标题概述 {#template-header-overview}

![](assets/template-header-350x18.png)

模板标题显示以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>标题信息</th> 
   <th>注释</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">对象图标 </td> 
   <td> <p>绿色的[!UICONTROL 模板]图标<img src="assets/nwe-templates-icon.png">将显示在模板名称的左侧。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">模板的名称</td> 
   <td>您可以在标题中编辑模板名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象类型的名称</td> 
   <td> <p>如果模板标记为活动，则在标题中的模板名称上方将显示文本“[!UICONTROL TEMPLATE]”。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">激活状态</td> 
   <td> <p>如果模板已停用，则标题中模板名称上方会显示文本“[!UICONTROL TEMPLATE DEACTIVATED]”。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">模板的操作区域</td> 
   <td> <p>在模板名称旁边，将显示操作区域。</p> <p> <img src="assets/actions-area-icons-without-share-button.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 模板所有者]</td> 
   <td>您可以编辑标题中的[!UICONTROL 模板所有者]字段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 持续时间]</td> 
   <td>模板的持续时间。 无法在标题中编辑此字段。</td> 
  </tr> 
 </tbody> 
</table>

## 模板任务标题概述

![](assets/template-task-header-350x18.png)

模板任务标题显示以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>标题信息</th> 
   <th>注释</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">到父对象的痕迹导航</td> 
   <td> <p>模板任务的父对象显示在痕迹导航中。 单击父对象的名称将打开该父对象。</p> <p>有关详细信息，请参阅<a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">痕迹导航概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象图标 </td> 
   <td> <p>绿色的[!UICONTROL 任务]图标<img src="assets/nwe-tasks-icon.png">将显示在模板任务名称的左侧。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">模板任务的名称</td> 
   <td>您可以在标题中编辑模板任务名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象类型的名称</td> 
   <td> <p>文本“[!UICONTROL TEMPLATE TASK]”显示在标题中模板任务名称上方。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">模板任务的操作区域</td> 
   <td> <p>在模板任务的名称旁边，将显示操作区域。</p> <p> <img src="assets/actions-area-icons-without-share-button.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 分配]</td> 
   <td>您可以在标题中编辑模板任务的[!UICONTROL 分配]。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 完成日]</td> 
   <td>这是应完成模板任务的模板持续时间的天数。</td> 
  </tr> 
 </tbody> 
</table>

## 开票记录题头概览

![](assets/billing-record-header-nwe-350x19.png)

开单记录题头显示以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>标题信息</th> 
   <th>注释</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">到父对象的痕迹导航</td> 
   <td> <p>计费记录的父对象显示在痕迹导航中。 单击父对象的名称将打开该父对象。</p> <p>有关详细信息，请参阅<a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">痕迹导航概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象图标 </td> 
   <td> <p>计费记录名称左侧显示蓝色的[!UICONTROL 计费记录]图标<img src="assets/nwe-billing-record-icon-57x55.png" style="width: 57;height: 55;">。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">开票记录的名称</td> 
   <td>您可以在标题中编辑开票记录的名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象类型的名称</td> 
   <td> <p>文本“[!UICONTROL BILLING RECORD]”显示在标头中的开票记录名称上方。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">计费记录的“更多”菜单</td> 
   <td> <p>在开票记录的名称旁边，将显示[!UICONTROL 更多]菜单<img src="assets/more-menu.png">，该菜单允许您选择以下选项：</p> 
    <ul> 
     <li> <p>[!UICONTROL 编辑]</p> </li> 
     <li> <p> 删除 </p> </li> 
    </ul>
    <p><b>注释</b></p>
    <p>对于记帐状态为“已记帐”的记帐记录，不会显示“更多”菜单。 您无法编辑或删除已记帐记录。</p>
     </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 开票记录总数]</td> 
   <td>这是开票记录的总金额。 您无法编辑此字段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 计费日期]</td> 
   <td>这是创建开票记录的日期，除非在创建开票记录时手动对其进行更改。 您可以在标题中编辑[!UICONTROL 计费日期]。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 状态]</td> 
   <td> <p>当开票记录的状态为[!UICONTROL Billed]时，您无法再编辑它。</p> <p>您可以在标题中编辑开票记录的状态。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 用户标题概述

![](assets/user-header-350x20.png)

用户标题显示以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>标题信息</th> 
   <th>注释</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">用户个人资料图片</td> 
   <td>无法更新标题中的配置文件图片。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">用户名称和标题</td> 
   <td> <p> 用户标题会以名称上方的所有大写字母显示。 无法在标题中编辑用户的名称。</p> </td> 
  </tr> <!--
   <tr> 
    <td role="rowheader">Name of the object type</td> 
    <td> <p>The name of the object type does not display.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">激活状态</td> 
   <td> <p>如果用户已停用，标题中的所有文本和配置文件图片将灰显。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">用户的操作区域</td> 
   <td> <p>在用户名旁边，将显示操作区域。</p> <p> <img src="assets/actions-area-icons-without-share-button.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">电子邮件地址</td> 
   <td>无法编辑标头中的电子邮件地址。 这通常是用户名。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">电话号码</td> 
   <td>您不能在标题中编辑电话号码。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">团队</td> 
   <td> <p>您可以查看用户所属的团队。 将鼠标悬停在团队头像上以显示团队名称。 您无法编辑标题中的团队。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 团队标题概述

![](assets/team-header-350x23.png)

团队标题显示以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>标题信息</th> 
   <th>注释</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">对象图标 </td> 
   <td> <p>紫色的[!UICONTROL 团队]图标<img src="assets/nwe-teams-icon.png">显示在团队名称的左侧。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">团队名称</td> 
   <td>您可以在标题中编辑团队名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象类型的名称</td> 
   <td> <p>文本“[!UICONTROL TEAM]”显示在标题中的团队名称上方。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">团队的操作区域</td> 
   <td> <p>在团队名称旁边，将显示操作区域。</p> <p> <img src="assets/actions-area-icons-for-a-team.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">团队成员个人资料图片</td> 
   <td>团队成员的个人资料图片。 将鼠标悬停在图片上可显示用户名。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">描述</td> 
   <td>这是对团队成员的简短描述。 您无法在标题中编辑团队描述。</td> 
  </tr> 
 </tbody> 
</table>

## 迭代标题概述

![](assets/iteration-header-350x19.png)

小版本标题显示以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>标题信息</th> 
   <th>注释</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">对象图标 </td> 
   <td> <p>橙色[!UICONTROL 迭代]图标<img src="assets/nwe-iteration-icon-58x58.png" style="width: 58;height: 58;">显示在迭代名称的左侧。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">迭代的名称</td> 
   <td>可在标题中编辑迭代名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象类型的名称</td> 
   <td> <p>文本“[!UICONTROL ITERATION]”显示在标头中的迭代名称上方。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">迭代的操作区域</td> 
   <td> <p>在迭代的名称旁边，将显示操作区域。</p> <p> <img src="assets/actions-area-icons-for-an-iteration.png">
  <tr> 
   <td role="rowheader">所有者</td> 
   <td>这是迭代的[!UICONTROL 所有者]。 您不能在标头中编辑[!UICONTROL Owner]。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 时间轴]</td> 
   <td>[!UICONTROL 时间轴]显示迭代的开始日期和结束日期。 您无法在标题中编辑[!UICONTROL 时间轴]。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 团队]</td> 
   <td>无法在标题中编辑迭代的团队。 单击团队名称将转到团队页面。</td> 
  </tr> 
 </tbody> 
</table>

## 组标题概述

![](assets/nwe-group-header-350x20.png)

组标题显示以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>标题信息</th> 
   <th>注释</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">对象图标 </td> 
   <td> <p>橙色[!UICONTROL 组]图标<img src="assets/nwe-group-icon.png">显示在组名的左侧。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">组的名称</td> 
   <td>您可以在标题中编辑组名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象类型的名称</td> 
   <td> <p>文本“[!UICONTROL GROUP]”显示在标头中的组名称上方。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">组的[!UICONTROL actions]区域</td> 
   <td> <p>在组名旁边，将显示[!UICONTROL 更多]菜单<img src="assets/more-menu.png">，该菜单允许您选择以下选项：</p> 
    <ul> 
     <li> <p>[!UICONTROL 编辑]</p> </li> 
     <li> <p>[!UICONTROL 副本]</p> </li> 
     <li> <p>[!UICONTROL Delete]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Business Leader]</td> 
   <td>您可以在标题中编辑[!UICONTROL Business Leader] 。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 许可证正在使用中] </td> 
   <td> <p>[!UICONTROL 正在使用的许可证]框显示组及其子组中[!UICONTROL 计划]和[!UICONTROL 工作]许可证用户的数量。 您可以单击编号查看所有5种许可证类型的此信息。</p> <p>有关详细信息，请参阅<a href="../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md" class="MCXref xref">查看新[!DNL Adobe Workfront]体验</a>中组内分配和使用许可证的数量。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 组管理员]</td> 
   <td>您可以在标题中编辑组管理员。</td> 
  </tr> 
 </tbody> 
</table>

## 文档标题概述

![](assets/document-header-350x19.png)

文档标题显示以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>标题信息</th> 
   <th>注释</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">具有父对象的痕迹导航</td> 
   <td> <p>文档的父对象显示在痕迹导航中。 单击父对象的名称将打开该父对象。</p> <p>有关详细信息，请参阅<a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">痕迹导航概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象图标 </td> 
   <td> <p>蓝色的[!UICONTROL Document]图标<img src="assets/nwe-documents-icon-53x50.png" style="width: 53;height: 50;">将显示在文档名称的左侧。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">文档的名称</td> 
   <td>您可以在标题中编辑文档名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象类型的名称</td> 
   <td> <p>文本“[!UICONTROL DOCUMENT]”显示在标题中文档名称的上方。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">文档的操作区域</td> 
   <td> <p>在文档名称旁边，将显示操作区域。</p> <p> <img src="assets/actions-area-icons-for-a-document.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">审批[!UICONTROL 决策]区域</td> 
   <td> [!UICONTROL Decisions]区域显示在文档标题的右上角。此区域因审批阶段以及您是审批者、审阅者还是既非审批者而有所不同。 <ul><li> <p>如果您是批准者，则可以使用以下图标管理文档的批准：</p> <p> <img src="assets/nwe-approvals-approve-16x18.png" style="width: 16;height: 18;"> [!UICONTROL 批准]</p> <p> <img src="assets/nwe-approvals-recall-16x16.png" style="width: 16;height: 16;"> [!UICONTROL 召回]</p> <p> <img src="assets/nwe-approvals-reject-16x19.png" style="width: 16;height: 19;"> [!UICONTROL 拒绝]</p> <p>有关批准决定的详细信息，请参阅<a href="../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">批准工作</a>。</li><li><p>如果您是审阅人，则可以单击“完成我的审阅”按钮以指示您已审阅文档。</p><p>有关审阅文档的更多信息，请参阅<a href="../../review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/review-a-document.md" class="MCXref xref">审阅文档</a>。</p></li><li>否则，此区域显示文档的当前审阅和审批状态。</li><ul></p> </td> 
  </tr> 
 </tbody> 
</table>

## 公司标题概述 {#company-header-overview}

![](assets/company-header-350x20.png)

公司标题显示以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>标题信息</th> 
   <th>注释</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">对象图标 </td> 
   <td> <p>公司名称左侧显示蓝色的[!UICONTROL 公司]图标<img src="assets/nwe-company-icon.png">。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">公司名称</td> 
   <td>您可以在标题中编辑公司的名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象类型的名称</td> 
   <td> <p>文本“[!UICONTROL COMPANY]”显示在标题中公司名称上方。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">公司的“更多”菜单</td> 
   <td> <p>在公司名称旁边，将显示[!UICONTROL More]菜单<img src="assets/more-menu.png">，该菜单允许您选择以下选项：</p> 
    <ul> 
     <li> <p>[!UICONTROL 编辑]</p> </li> 
     <li> <p>[!UICONTROL 删除公司]</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 计划题头概览

![](assets/nwe-plan-header-350x34.png)

计划是[!DNL Workfront Scenario Planner]的对象。 有关[!DNL Scenario Planner]的信息，请参阅[概述 [!DNL Scenario Planner] &#x200B;](../../scenario-planner/scenario-planner-overview.md)。

计划题头显示以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>标题信息</th> 
   <th>注释</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">返回至计划</td> 
   <td>单击此链接将会转到[!UICONTROL Plans]列表。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象图标 </td> 
   <td> <p>计划名称的左侧将显示蓝色的[!UICONTROL 计划]图标<img src="assets/nwe-plan-icon-65x62.png" style="width: 65;height: 62;">。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">计划的名称</td> 
   <td>您可以在标题中编辑计划名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象类型的名称</td> 
   <td> <p>文本“[!UICONTROL PLAN]”显示在标题中计划名称上方。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">计划的操作区域</td> 
   <td> <p>在计划名称旁边，将显示操作区域。</p> <p> <img src="assets/actions-area-icons-without-share-button.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他计划操作</td> 
   <td> <p>在计划名称和操作区域下，您可以完成以下操作：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 显示冲突]</strong>：单击此切换可显示或隐藏计划中的冲突。</p> </li> 
     <li> <p><strong>[!UICONTROL 比较方案]</strong>：单击此链接可显示您已创建的方案的并排比较。</p> </li> 
     <li> <p><strong>[!UICONTROL 方案选择]</strong>：在此下拉菜单中，您可以复制方案或选择查看其他方案。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">工作角色信息</td> 
   <td>在[!UICONTROL 工作角色]框中，您可以查看与所需职位角色数量相比，计划中有多少职位角色可用。 单击该框可调整可用的工作角色。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Financial]信息</td> 
   <td>在[!UICONTROL Financial]框中，您可以查看计划的预算、成本和利用率百分比。 单击该框可调整预算金额并确定人员成本是否包括在计划中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 净值]</td> 
   <td>在[!UICONTROL 净值]框中，您可以根据为计划输入的预算和成本查看计划的净值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 共享对象]信息</td> 
   <td>有权查看或管理计划的用户显示在标题的右上角。 将鼠标悬停在个人资料图片上会显示他们的姓名。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 转至发布]</td> 
   <td>单击[!UICONTROL 转到发布]后，您可以在查看的方案中创建或更新链接到方案的项目。</td> 
  </tr> 
 </tbody> 
</table>


## 目标标题概述

![](assets/goal-header.png)

当您的公司有权访问Workfront目标时，您可以创建战略目标。 有关[!DNL Workfront Goals]的详细信息，请参阅[开始使用 [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md)。

目标标题显示以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>标题信息</th> 
   <th>注释</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">对象图标 </td> 
   <td> <p>紫色[!UICONTROL 目标]图标<img src="assets/goal-icon.png" >将显示在目标名称的左侧。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">目标的名称</td> 
   <td>您可以在标题中编辑目标名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象类型的名称</td> 
   <td> <p>文本“[!UICONTROL GOAL]”显示在标题中目标名称上方。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">目标的“更多”菜单</td> 
   <td> <p>在目标名称旁边，显示更多菜单<img src="assets/more-icon.png">。</p> </p>
   您可以从目标的更多菜单执行以下操作：
   <ul><li>[!UICONTROL 编辑]</li>
   <li>[!UICONTROL 复制目标]</li>
   <li>[!UICONTROL 删除目标]</li>
   <li>[!UICONTROL 共享]</li>
   <li>[!UICONTROL Activate]或[!UICONTROL Deactivate]</li>
   <li>[!UICONTROL Close]或[!UICONTROL Reopen]</li>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 进度]</td> 
   <td>进度目标的百分比，指示已完成目标的程度。 您无法更新目标进度。 Workfront根据目标上每个进度指示器的进度计算此值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 所有者]</td> 
   <td>这是目标的所有者。 您可以手动更新目标所有者。 用户、团队、组或您的组织可以是目标所有者。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 句点]</td> 
   <td>必须完成目标的时间范围。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 条件]</td> 
   <td>目标条件指示目标是否按计划按时完成，还是落后 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 状态]</td> 
   <td>指示目标处于活动状态、新建状态还是关闭状态。 您无法手动更新目标状态。 有关详细信息，请参阅[!DNL Adobe Workfront Goals]</a>中的<a href="../../workfront-goals/goal-management/goal-status-overview.md" class="MCXref xref">目标状态概述</td> 
  </tr> 
 </tbody> 
</table>
