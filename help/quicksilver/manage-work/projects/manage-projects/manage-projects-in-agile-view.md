---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: 在Agile视图中管理项目
description: 您可以利用项目的Agile功能，而无需Agile实践通常伴随的管理挑战（例如管理团队积压或创建迭代）。
author: Alina and Lisa
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1423'
ht-degree: 0%

---

# 在Agile视图中管理项目

<!-- Audited: 2/2024 -->

您可以利用项目的Agile功能，而无需Agile实践通常伴随的管理挑战（例如管理团队积压或创建迭代）。

如果要在使用团队积压工作的Agile环境中工作，并允许您从积压工作上的任务创建迭代，请按照[在Agile环境中工作](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md)中的说明操作。

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
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>当前：审阅或更高版本</p> 
   <p>新文档：参与者或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对以下区域的访问权限：</p> 
    <ul> 
     <li> <p>项目</p> </li> 
     <li> <p>报告、功能板、日历</p> </li> 
     <li> <p>筛选器、视图、分组</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 了解Agile项目

>[!NOTE]
>
>本节仅适用于旧版Agile视图，不适用于项目的展示板视图。

* [项目中的Agile功能](#agile-functionality-in-a-project)
* [在项目上使用敏捷视图与在开发周期上使用敏捷视图时的差异](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### 项目中的敏捷功能 {#agile-functionality-in-a-project}

在Agile视图中管理项目时，可以使用以下Agile功能：

* 完成状态\
  有关完成状态的更多详细信息，请参阅[迭代完成状态概述](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md)。

* 故事板\
  有关故事板的更多详细信息，请参阅[Scrum板](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md)部分。

在项目上使用Agile视图与在纯Agile环境（包含积压和迭代）中工作有一些差异。 有关详细信息，请参阅本文中[在项目上使用Agile视图与迭代](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)上使用Agile视图的区别。

### 在项目上使用敏捷视图与在开发周期上使用敏捷视图时的差异 {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [任务和子任务在项目Agile视图和开发周期故事板上遵循不同的显示规则](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [Agile视图中未使用积压和迭代](#backlogs-and-iterations-are-not-used)
* [任务顺序在Agile视图中维护，无法重新排序](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [任务仅在项目列表](#tasks-are-measured-only-in-planned-hours)上的计划小时数中测量
* [Agile团队未在Agile视图中使用](#the-agile-team-is-not-used)
* [项目中的每个用户都可以在不同的Agile视图中查看项目](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### 任务和子任务遵循项目“敏捷”视图和开发周期故事板上的不同显示规则 {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* 没有父任务和子任务的任务始终在敏捷视图的故事板中显示为单个故事卡。\
  例如，这些任务在项目列表视图中如下所示：

  ![Agile项目列表 — 无父任务或子任务的任务](assets/agile-project-single-list-nwe.png)

  这些任务在项目Agile视图中如下所示：

  ![项目Agile视图 — 无父任务或子任务的任务](assets/agile-project-singlecard-nwe.png)

* 具有子任务的父任务始终显示在敏捷视图故事板的&#x200B;**故事**&#x200B;列中。 子任务显示在父任务的泳道中。\
  例如，这些任务在项目列表视图中如下所示：

  ![Agile项目列表 — 具有父任务和子任务的任务](assets/agile-project-parent-list-nwe.png)\
  这些任务在项目Agile视图中如下所示：

  ![Agile项目视图 — 具有父任务和子任务的任务](assets/agile-project-parent-nwe.png)

* 第二级子任务（子任务的子任务）在直接父任务中显示为悬挂的灰色卡片。
* Agile视图中永远不会显示第三级子任务（子任务的子任务）。

#### 在Agile视图中不使用积压和迭代 {#backlogs-and-iterations-are-not-used}

在Agile视图中查看项目时，不使用以下Agile组件：

* **积压：**&#x200B;未使用积压，因为项目中的任何任务都会自动显示为故事。
* **迭代：**&#x200B;不是创建迭代来定义完成工作的日期，而是将项目时间轴上当前指定的日期变为工作日。

#### 任务顺序在Agile视图中维护，无法重新排序 {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

在敏捷故事板中查看项目时，将保持任务在项目中的显示顺序。

在Agile视图中查看项目时，无法对项目中的任务重新排序。 由于修改任务顺序可能会影响其他可能具有依赖关系的任务，因此必须在标准视图中查看项目才能修改任务顺序。

#### 任务仅在项目列表上的计划小时数中进行测量 {#tasks-are-measured-only-in-planned-hours}

项目中的任务始终按计划小时数测量。

在迭代中，任务（故事）可以用小时或点来测量。

#### Agile团队未在Agile视图中使用 {#the-agile-team-is-not-used}

由于Agile团队完成分配给他们的迭代工作，因此Agile团队在Agile视图中查看项目时不使用。

反之，项目中的任何用户实质上是该项目的Agile团队。

#### 项目中的每个用户都可以在不同的Agile视图中查看项目 {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

与敏捷开发周期不同，项目中的用户可以自定义自己的敏捷视图，而其他用户使用不同的敏捷视图。

在敏捷开发周期中，敏捷故事板上可用的信息（例如可用的状态列）由团队级别确定。

有关如何自定义Agile视图的信息，请参阅[在Adobe Workfront中创建或编辑视图](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md)中的[创建或自定义Agile视图](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view)。

## 在Agile视图中查看项目

1. 转到任务列表或问题列表中的要在Agile视图中查看的项目。
1. 单击&#x200B;**展示板视图**&#x200B;图标![展示板图标](assets/board-icon-for-agile-view.png)。

   默认情况下，将显示项目的讨论区视图。

   ![讨论区项目视图](assets/project-agile-board-view.png)

   <!--(Legacy agile view only) If you previously viewed the project in a custom agile view, the project is displayed in that view rather than in the default agile view.-->

1. （可选）单击&#x200B;**配置**&#x200B;以设置列和卡片的选项。

   有关详细信息，请参阅[管理展示板列](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)和[自定义信息卡上显示的字段](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md)。 请注意，您无法在项目的展示板视图中定义列策略。

1. （可选）单击&#x200B;**使用旧版Agile**&#x200B;以使用旧版Agile视图而不是展示板视图。

1. （可选 — 仅限旧版Agile视图）如果您已创建自定义Agile视图，或者如果其他用户已创建自定义Agile视图并与您共享，则可以查看它，而不是默认的Agile视图。

   单击&#x200B;**视图**&#x200B;下拉菜单，然后单击要查看的自定义敏捷视图。

   下次单击&#x200B;**Agile**&#x200B;图标时将使用自定义Agile视图。

   有关如何创建新的Agile视图的信息，请参阅下面的[创建和自定义Agile视图](#create-and-customize-agile-views)。

   项目显示在自定义Agile视图中。

1. （视情况而定 — 仅限旧版敏捷视图）如果您的项目中的任务使用的状态不是“新建”、“进行中”或“完成”（敏捷视图的默认状态），则必须将其他状态添加到敏捷视图，才能显示这些状态的任何任务。

   如果任务处于未显示在敏捷故事板上的状态，则任务本身未显示在敏捷故事板上（但是，这些任务的完成百分比仍然构成任何父任务的完成百分比和整个项目的完成百分比）。

   要向Agile视图添加状态，请创建新的Agile视图或自定义现有的Agile视图，如下面[创建和自定义Agile视图](#create-and-customize-agile-views)中所述。

1. （可选）要返回到列表视图，请单击&#x200B;**列表**&#x200B;图标。

## 创建和自定义Agile视图 {#create-and-customize-agile-views}

>[!NOTE]
>
>本节仅适用于旧版Agile视图，不适用于项目的展示板视图。

与Workfront中的标准视图一样，您可以自定义现有Agile视图或从头开始创建新的Agile视图。 与标准视图不同，您不能根据现有Agile视图创建新的Agile视图。

有关创建和自定义Agile视图的更多信息，请参阅[在Adobe Workfront中创建或编辑视图](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md)一文中的[创建或自定义Agile视图](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view)部分。

## 共享现有Agile视图

>[!NOTE]
>
>本节仅适用于旧版Agile视图，不适用于项目的展示板视图。

您可以共享您创建的Agile视图，或者以共享任何其他视图、过滤器或分组的相同方式拥有对的权限。

有关详细信息，请参阅[共享筛选器、视图或分组](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md)。

## 删除现有Agile视图

>[!NOTE]
>
>本节仅适用于旧版Agile视图，不适用于项目的展示板视图。

删除Agile视图的方式与删除任何其他视图、过滤器或分组的方式相同。

有关详细信息，请参阅[删除筛选器、视图和分组](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md)。
