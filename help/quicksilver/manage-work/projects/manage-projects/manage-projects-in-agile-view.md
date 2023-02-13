---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: 在敏捷视图中管理项目
description: 所需的计划、许可类型和访问Adobe Workfront计划团队、专业、企业或企业Workfront许可证类型在访问模型中审核、工作或计划权限编辑访问权限和创建报表、功能板和日历的功能
author: Alina
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1311'
ht-degree: 0%

---

# 在敏捷视图中管理项目

所需的计划、许可证类型和访问权限

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront计划</a> </p> </td> 
   <td> <p>Team、Pro、Business或Enterprise </p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="https://one.workfront.com/s/article/Understanding-License-Types-906212506?language=en_US&amp;r=16&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank">Workfront许可证类型</a> </p> </td> 
   <td> <p>审核、工作或计划 </p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Permissions in the access model</p> </td> 
    <td> <li>Edit access and ability to create reports, dashboards, and calendars</li> </td> 
   </tr>
  --> 
 </tbody> 
</table>

您可以在项目中利用灵活的功能

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(such as story boards and burndown charts)
</MadCap:conditionalText>
-->

 无需应对通常伴随敏捷实践的管理挑战（例如管理团队积压或创建迭代）。

如果要在使用团队积压的工作的敏捷环境中工作，并允许您根据积压工作的任务创建迭代，请按照 [在灵活的环境中工作](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

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
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对以下区域的访问：</p> 
    <ul> 
     <li> <p>项目</p> </li> 
     <li> <p>报表、功能板、日历</p> </li> 
     <li> <p>过滤器、视图、分组</p> </li> 
    </ul> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 了解敏捷项目

* [项目中的灵活功能](#agile-functionality-in-a-project)
* [在项目上使用敏捷视图与在迭代上使用敏捷视图时的差异](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### 项目中的灵活功能 {#agile-functionality-in-a-project}

在敏捷视图中管理项目时，可以使用以下灵活功能：

* 完成状态\
   有关完成状态的更多详细信息，请参阅 [迭代完成状态概述](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* 文章板\
   有关文章展示板的更多详细信息，请参阅 [洗涤板](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md) 中。

在项目上使用敏捷视图与在纯敏捷环境（具有积压工和迭代版本）中工作存在一些差异。 有关更多信息，请参阅 [在项目上使用敏捷视图与在迭代上使用敏捷视图时的差异](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) 在本文中。

### 在项目上使用敏捷视图与在迭代上使用敏捷视图时的差异 {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [任务和子任务遵循文章展示板上的不同显示规则](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [不使用积压日志和迭代](#backlogs-and-iterations-are-not-used)
* [任务顺序在Agile视图中进行维护，无法重新排序](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [任务仅以计划小时计量](#tasks-are-measured-only-in-planned-hours)
* [未使用Agile Team](#the-agile-team-is-not-used)
* [项目中的每个用户都可以以不同的敏捷视图查看项目](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### 任务和子任务遵循文章展示板上的不同显示规则 {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* 既没有父任务也没有子任务的任务始终在文章板上显示为单个文章卡片。\
   例如，这些任务在项目列表视图中如下所示：

   ![敏捷项目列表 — 没有父项或子任务的任务](assets/agile-project-single-list-nwe.png) 这些任务在项目敏捷视图中如下所示：

   ![项目敏捷视图 — 没有父项或子任务的任务](assets/agile-project-singlecard-nwe.png)

* 具有子任务的父任务始终显示在 **故事** 栏。 子任务显示在父任务的泳道中。\
   例如，这些任务在项目列表视图中如下所示：

   ![敏捷项目列表 — 具有父项和子任务的任务](assets/agile-project-parent-list-nwe.png)\
   这些任务在项目敏捷视图中如下所示：

   ![敏捷项目视图 — 包含父项和子任务的任务](assets/agile-project-parent-nwe.png)

* 二级子任务（子任务的子任务）显示为直接父任务的挂灰卡。
* 文章展示板上从不显示第三级子任务（子任务子任务的子任务）。

#### 不使用积压日志和迭代 {#backlogs-and-iterations-are-not-used}

在敏捷视图中查看项目时，不会使用以下敏捷组件：

* **积压：** 没有使用积压工作，因为项目中的任何任务都会自动显示为文章。
* **迭代：** 项目时间轴上当前指定的日期不是创建迭代来定义完成工作的日期，而是变为工作日。

#### 任务顺序在Agile视图中进行维护，无法重新排序 {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

在敏捷文章展示板中查看项目时，将保持任务在项目中显示的顺序。

在敏捷视图中查看项目时，无法重新排序项目中的任务。 由于修改任务顺序会影响可能具有依赖关系的其他任务，因此您必须在标准视图中查看项目才能修改任务顺序。

#### 任务仅以计划小时计量 {#tasks-are-measured-only-in-planned-hours}

项目中的任务始终以计划时间进行测量。

在迭代中，任务（文章）可以以小时或点为单位进行测量。

#### 未使用Agile Team {#the-agile-team-is-not-used}

由于敏捷团队完成了分配给他们的迭代工作，因此在敏捷视图中查看项目时，不会使用敏捷团队。

相反，项目中的任何用户实际上都会成为该项目的敏捷团队。

#### 项目中的每个用户都可以以不同的敏捷视图查看项目 {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

与敏捷迭代不同，项目用户可以为自己自定义敏捷视图，而其他用户则使用不同的敏捷视图。

在敏捷迭代中，在团队级别上确定可在敏捷故事板上使用的信息（如可用的状态列）。

有关如何自定义敏捷视图的信息，请参阅  [创建或自定义敏捷视图](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in  [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 

## 在敏捷视图中查看项目

1. 转到要在敏捷视图中查看的项目。
1. 单击 **敏捷** 图标。\
   ![Agile图标](assets/agile-icon-nwe.png)\
   项目显示在默认敏捷视图中。\
   如果您之前在自定义敏捷视图中查看了项目，则该项目将显示在该视图中，而不是默认敏捷视图中。

1. （可选）如果您已创建自定义敏捷视图，或者如果其他用户创建了自定义敏捷视图并与您共享该视图，则可以查看该视图，而不是默认的敏捷视图。\
   单击 **查看** 下拉菜单，然后单击要查看的自定义敏捷视图。

   下次单击 **敏捷** 图标。\
   有关如何创建新的敏捷视图的信息，请参阅 [创建和自定义敏捷视图](#create-and-customize-agile-views).\
   项目在自定义敏捷视图中显示。

1. （视情况而定）如果项目中的任务使用的状态不是“新”、“进行中”或“完成”（敏捷视图的默认状态），则必须向敏捷视图添加其他状态，才能显示处于这些状态的任何任务。\
   如果任务处于未在敏捷文章展示板中显示的状态，则任务本身不会显示在敏捷文章展示板中（但是，这些任务的完成百分比仍会导致任何父任务的完成百分比和整个项目的完成百分比）。\
   要向敏捷视图添加状态，请创建新的敏捷视图或自定义现有的敏捷视图，如文章的“创建或自定义敏捷视图”部分所述 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. （可选）要返回到列表视图，请单击 **列表** 图标。\
   ![](assets/list-icon.png)

## 创建和自定义敏捷视图 {#create-and-customize-agile-views}

与Workfront中的标准视图一样，您可以自定义现有的敏捷视图或从头开始创建新的敏捷视图。 与标准视图不同，您不能基于现有的敏捷视图创建新的敏捷视图。

有关创建和自定义敏捷视图的更多信息，请参阅文章中的“创建或自定义敏捷视图”部分 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 

## 共享现有Agile视图

有关如何共享敏捷视图的信息，请参阅 [共享过滤器、查看或分组](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## 删除现有的Agile视图

有关如何删除视图的信息，请参阅文章中的“删除视图”部分 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 
