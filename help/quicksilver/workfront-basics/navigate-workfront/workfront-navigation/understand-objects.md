---
content-type: overview;reference
navigation-topic: workfront-navigation
title: '[!DNL Adobe Workfront]对象概述'
description: 在 [!DNL Adobe Workfront] 中显示的信息由存储在 [!DNL Workfront] 数据库中的对象表示。 对象是驱动 [!DNL Workfront]中信息的驱动因素。 请参阅本文以了解有关这些对象的更多信息。
feature: Get Started with Workfront
author: Alina
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '2508'
ht-degree: 1%

---

# [!DNL Adobe Workfront]对象概述

<!--Audited: 12/2023-->

<!--
<***Linked to several articles, do not remove/ change. 
-->

您在[!DNL Adobe Workfront]中显示的信息由存储在[!DNL Workfront]数据库中的对象表示。 对象是驱动[!DNL Workfront]中信息的驱动因素。

了解如何在[!DNL Workfront]中定义对象非常重要，这样您就可以使用正确的对象来满足组织内的必要需求。

例如，当您计划大量工作时，您需要使用[!UICONTROL 项目]对象来定义该工作。 若要将此工作划分为较小的计划增量，您可以使用[!UICONTROL 任务]对象。 对于少量未计划且可能意外发生的工作，您可以使用Issue对象。 如果要跟踪一组项目的进度以及是否符合预算和时间表，可以在[!UICONTROL 项目组合]和[!UICONTROL 项目]中组织它们。 要定义帮助您解决工作的其他元素，您需要使用存储在[!UICONTROL 项目]、[!UICONTROL 任务]、[!UICONTROL 问题]或[!UICONTROL 项目组合]下的其他对象，如[!UICONTROL 文档]、[!UICONTROL 更新]、[!UICONTROL 小时]、[!UICONTROL 用户]或[!UICONTROL 工作角色]。

[!UICONTROL 报表]和[!UICONTROL 功能板]是另一个对象示例，它们可帮助您直观地整理[!DNL Workfront]中拥有的数据量，以便所有用户都能轻松访问。

有关[!DNL Workfront]中对象的完整列表，请参阅[API资源管理器](../../../wf-api/general/api-explorer.md)。

## 对象的相互依赖性和层次结构

对象在[!UICONTROL Workfront]中相互链接。 例如，任务或问题永远不能独立于项目之外存在。 [!UICONTROL 任务]和[!UICONTROL 问题]是存储在[!UICONTROL 项目]对象中的对象示例。 [!UICONTROL 任务]和[!UICONTROL 问题]被视为项目的子对象。

以下是[!DNL Workfront]中最常用的对象及其各自的父对象和子对象：

| **对象** | **父对象** | **子对象** |
|---|---|---|
| [!UICONTROL 项目组合] |  | [!UICONTROL 项目群]，[!UICONTROL 项目]，[!UICONTROL 文档]，[!DNL Notes]，[!UICONTROL 用户] |
| [!UICONTROL 程序] | [!UICONTROL 项目组合] | [!UICONTROL 项目]，[!UICONTROL 文档]，[!UICONTROL 注释]，[!UICONTROL 用户] |
| [!UICONTROL 项目] | [!UICONTROL 项目组合]，[!UICONTROL 程序] | [!UICONTROL 任务]，[!UICONTROL 问题]，[!UICONTROL 文档]，[!UICONTROL 备注]，[!UICONTROL 小时]，[!UICONTROL 用户] |
| [!UICONTROL 任务] | [!UICONTROL 项目] | [!UICONTROL 问题]，[!UICONTROL 子任务]，[!UICONTROL 文档]，[!UICONTROL 注释]，[!UICONTROL 小时]，[!UICONTROL 用户] |
| [!UICONTROL 问题] | [!UICONTROL 任务]，[!UICONTROL 项目] | [!UICONTROL 文档]，[!UICONTROL 备注]，[!UICONTROL 小时]，[!UICONTROL 用户] |
| [!UICONTROL 仪表板] |  | [!UICONTROL 报告]，外部页面 |
| [!UICONTROL 报告] | [!UICONTROL 仪表板] |  |
| [!UICONTROL 组] |  | [!UICONTROL 用户] |
| [!UICONTROL 团队] |  | [!UICONTROL 用户] |
| [!UICONTROL 用户] | [!UICONTROL 组]，[!UICONTROL 团队]，[!UICONTROL 公司] | [!UICONTROL 职位角色] |
| [!UICONTROL 公司] |  | [!UICONTROL 用户] |
| [!UICONTROL 文档] | [!UICONTROL 任务]，[!UICONTROL 问题]，[!UICONTROL 项目]，[!UICONTROL 项目组合]，[!UICONTROL 程序]，[!UICONTROL 用户] |  |
| [!UICONTROL 计划]* |  | [!UICONTROL 个计划] |
| [!DNL Goals]* |  | [!UICONTROL 个结果]，[!UICONTROL 个活动] |

有关[!DNL Workfront]中对象的完整列表，请参阅[API资源管理器](../../../wf-api/general/api-explorer.md)。

*计划是[!DNL Adobe Workfront Scenario Planner]的对象。 有关[!DNL Scenario Planner]的信息，请参阅[方案规划器]概述](../../../scenario-planner/scenario-planner-overview.md)。[!UICONTROL 

*[!UICONTROL 目标]是[!DNL Adobe Workfront Goals]的对象。 有关[!DNL Workfront Goals]的信息，请参阅[[!DNL Adobe Workfront Goals] 概述](../../../workfront-goals/goal-management/wf-goals-overview.md)。


## 自定义对象名称

作为[!DNL Workfront]管理员，您可以使用[!UICONTROL 布局模板]自定义[!DNL Workfront]中的对象名称。

有关如何使用[!UICONTROL 布局模板]自定义对象名称的详细信息，请参阅[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

在自定义版面模板并将其分配给用户后，这些用户将看到对象的自定义名称。 已分配给布局模板的用户不再看到Web应用程序中任何位置的对象的缺省名称。

例如，如果组织中较大的工作量称为“参与度”，则可以将名称“[!UICONTROL 项目]”替换为“参与度”。 您的[!DNL Workfront]界面显示“Engagement”而不是“[!UICONTROL Project]”，显示名称为“[!UICONTROL Project]”的所有位置。

>[!NOTE]
>
>要使用户能够看到对象的新名称，用户必须在保存[!UICONTROL 布局模板]后注销并重新登录到[!DNL Workfront]。

>[!IMPORTANT]
>
>[!DNL Workfront]文档始终引用对象的默认名称。 作为[!DNL Workfront]管理员，请确保将对象名称的更改通知用户，以便他们了解如何使用[!DNL Workfront]文档，以及应用程序中没有反映对象名称更改的区域。

* [可以使用[!UICONTROL 布局模板]自定义的对象名称](#object-names-that-can-be-customized-using-a-layout-template)
* [ [!DNL Workfront] 中反映自定义对象名称的区域](#areas-of-workfront-that-reflect-the-customized-object-names)
* [未反映自定义对象名称的 [!DNL Workfront] 区域](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### 可以使用[!UICONTROL 布局模板]自定义的对象名称

作为[!DNL Workfront]管理员，您可以自定义以下对象的名称以匹配组织中的术语：

* [!UICONTROL Portfolio]
* [!UICONTROL 计划]
* [!UICONTROL 项目]
* [!UICONTROL 任务]
* [!UICONTROL 问题]
* [!UICONTROL 目标]*
* [!UICONTROL 结果]*
* [!UICONTROL 活动]*

  *[!UICONTROL 目标]、[!UICONTROL 结果]和[!UICONTROL 活动]仅在您的公司购买了[!DNL Workfront Goals]时才可用。 有关[!DNL Workfront Goals]的信息，请参阅[[!DNL Adobe Workfront Goals] 概述](../../../workfront-goals/goal-management/wf-goals-overview.md)。

* [!UICONTROL 计划]**
* [!UICONTROL 方案]**
* [!UICONTROL 计划]**

  **[!UICONTROL 计划]、[!UICONTROL 方案]和[!UICONTROL 计划]仅在您的公司购买了[!DNL Workfront Scenario Planner]时才可用。 有关[!DNL Scenario Planner]的信息，请参阅[开始使用 [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md)。



有关如何使用[!UICONTROL 布局模板]自定义对象名称的详细信息，请参阅[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

您无法在Workfront中自定义任何其他对象的名称。 有关[!DNL Workfront]中对象的完整列表，请参阅[API资源管理器](../../../wf-api/general/api-explorer.md)。

自定义对象名称时，该对象的新名称将出现在[!DNL Workfront]应用程序显示该对象名称的大部分区域中。

### [!DNL Workfront]中反映自定义对象名称的区域

以下区域显示对象的更新名称：

* 顶端导航
* 左侧面板导航中的所有部分
* 所有菜单
* 应用程序内通知
* Report Builder和报告元素（视图、筛选器和分组）
* [!UICONTROL 保存]按钮
* 导出的文件
* 电子邮件
* 移动应用程序

### 未反映自定义对象名称的[!DNL Workfront]区域

以下区域不显示对象的更新名称：

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook]加载项

### 自定义对象名称的含义

在[!DNL Workfront]中自定义对象名称时，您应了解以下事项：

* 在系统显示中可能会遇到文体或语法错误。 例如，如果将“[!UICONTROL Issue]”重命名为“Request”，并且在系统中的任何位置都看到短语“An request”，则表示这是正常的，不应视为错误。
* 对象的自定义名称不可翻译。 只能将[!DNL Workfront]默认名称翻译为支持的语言。 有关[!DNL Workfront]支持的语言的详细信息，请参阅 [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md)支持的[语言。 自定义对象名称字段支持外字符，因此您可以用任何语言输入术语。
* 当您使用[!UICONTROL 布局模板]自定义对象名称时，我们建议您根据业务部门（团队或组）分配[!UICONTROL 布局模板]。\
   我们建议您使用这些业务部门用户能够清晰理解的名称以避免混淆。
* 电子邮件通知和传送的报告始终包含由生成电子邮件的用户的[!UICONTROL 布局模板]定义的对象名称。 如果您的用户从其他团队和组中的用户收到电子邮件通知，则您应当准备好在其电子邮件中看到与组或团队无关的对象名称。\
   作为[!DNL Workfront]管理员，建议用户注意与每个对象关联的图标。 图标在各种对象名称之间保持一致并与默认对象一致，如显示在数据库中的那样。 有关与对象关联的所有[!DNL Workfront]图标的列表，请参阅[对象图标](#object-icons)。

  >[!TIP]
  >
  >对于组织中的常见任务，请考虑创建自定义文档以反映您的术语。

## 对象图标

[!DNL Workfront]文档始终引用对象的默认名称。 如果您的对象已自定义其名称，您可以依靠与其关联的图标来了解哪个自定义对象对应于哪个[!DNL Workfront]默认对象。

有关哪些对象可在[!DNL Workfront]中具有自定义名称的详细信息，请参阅[可以使用[!UICONTROL 布局模板]](#object-names-that-can-be-customized-using-a-layout-template)自定义的对象名称。

以下是Workfront中的对象及其相应图标的列表。

| **对象** | **图标** | **可自定义的对象名称** |
|---|---|---|
| [!UICONTROL 公司] | ![公司图标](assets/company-icon-nwe.png) ，![公司图标蓝色](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL 仪表板] | ![仪表板图标](assets/dashboard-icon-nwe.png)，![仪表板图标](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL 目标] | ![目标图标](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL 组] | ![组图标](assets/groups-icon-nwe.png)，![组图标](assets/nwe-group-icon.png) |  |
| [!UICONTROL 问题] | ![问题图标](assets/issue-icon-nwe.png) ，![问题图标粉红色](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL 工作角色] | ![job_role_icon.png](assets/job-role-icon-52x50.png)，![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png)，![工作角色图标](assets/job-role-nwe-no-color.png)，![工作角色图标颜色](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL 计划] | ![计划图标](assets/plan-icon.png)，![计划图标蓝色](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL Portfolio] | ![Portfolio](assets/portfolio-icon-nwe.png) ，![Portfolio图标（蓝色）](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL 计划] | ![计划图标](assets/program-icon-nwe.png) ，![计划图标](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL 项目] | ![项目图标](assets/project-icon-nwe.png) ，![紫色项目图标](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL 报告] | ![报告图标](assets/report-icon-nwe.png)，![报告图标绿色](assets/nwe-reports-icon.png) |  |
| [!UICONTROL 任务] | ![任务图标](assets/task-icon-new.png) ，![任务图标绿色](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL 团队] | ![团队图标](assets/team-icon-nwe.png)，![团队图标循环](assets/team-icon-nwe-color.png)，![团队图标](assets/nwe-teams-icon.png) |  |
| [!UICONTROL 模板] | ![模板图标](assets/template-icon-nwe.png) ，![模板图标绿色](assets/nwe-templates-icon.png) |  |
| [!UICONTROL 用户] | ![用户图标灰色](assets/users-icon-gray.png) ，![用户图标蓝色](assets/user-icon-blue.png) ，![带有首字母的用户图标](assets/user-icon-initials.png) ，![头像](assets/user-avatar.png) ，![用户图标主菜单](assets/user-main-menu-area.png) |  |

## 对象的参考编号

在[!DNL Workfront]中创建的每个对象都分配有一个唯一的参考编号。 参考号有助于区分两个在其他方面相似的对象（如同名的任务）。 您可以使用对象的参考编号来搜索对象，也可以在报表中包括参考编号。

有关如何按参考号搜索对象的信息，请参阅[使用对象的参考号](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md)。

## 对象特定的搜索

您可以在[!DNL Workfront]中搜索所有对象，也可以在基本和高级搜索中选择要搜索的特定对象。

并非所有对象都可以在[!DNL Workfront]中搜索。 您可以在[!DNL Workfront]中运行对以下对象的基本和高级搜索：

| **对象** | **基本搜索** | **高级搜索** |
|---|---|---|
| [!UICONTROL 项目] | ✓ | ✓ |
| [!UICONTROL 任务] | ✓ | ✓ |
| [!UICONTROL 问题] | ✓ | ✓ |
| [!UICONTROL 报告] | ✓ | ✓ |
| [!UICONTROL 用户] | ✓ | ✓ |
| [!UICONTROL 模板] | ✓ | ✓ |
| [!UICONTROL 文档] | ✓ | ✓ |
| [!UICONTROL 项目组合] | ✓ | ✓ |
| [!UICONTROL 程序] | ✓ | ✓ |
| [!UICONTROL 仪表板] | ✓ | ✓ |
| [!UICONTROL 公司] | ✓ | ✓ |
| [!UICONTROL 备注]（或[!UICONTROL 更新]） | ✓ |  |

有关在[!DNL Workfront]中运行基本和高级搜索的详细信息，请参阅[搜索 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md)。


## 限制访问对象

当用户无权访问对象时，用户将看到“无权访问”该对象名称显示在Workfront中的任何位置。

可以在访问级别或特定对象的权限中限制对对象的访问。

这适用于本文中[对象相互依赖性和层次结构](#interdependency-and-hierarchy-of-objects)部分中列出的所有对象和子对象。 这不适用于团队和用户对象。

## 对象报表

在[!DNL Workfront]中开始构建报表之前，了解对象的层次和相互依赖关系非常重要。 报告特定于对象。 您必须先为报表选择正确的对象，然后才能显示所需的数据。

>[!IMPORTANT]
>
>您只能在同一个报表中报告所选对象和父对象。 父对象报表中不能包含有关子对象的信息。 例如，您可以在任务报告中显示项目信息，但不能在项目报告中显示任务信息。

您可以使用我们的开放API报告数据库中的所有对象。 有关数据库中所有对象的完整列表，请参阅[API资源管理器](../../../wf-api/general/api-explorer.md)。

>[!NOTE]
>
> * 如果您已使用布局模板自定义了对象名称，则也会自定义Report Builder中的对象名称。 确保您知道哪些对象已自定义，并在Report Builder中查找自定义名称。 有关哪些对象可在[!DNL Workfront]中具有自定义名称的详细信息，请参阅本文中的[可以使用[!UICONTROL 布局模板]](#object-names-that-can-be-customized-using-a-layout-template)自定义的对象名称。
> * 在报表中使用文本模式时，文本模式表达式中的对象名称是[!DNL Workfront]中的标准名称，而不是自定义的对象名称。 有关在报表中使用文本模式的详细信息，请参阅[文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

有关生成报告的详细信息，请参阅[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。\
有关我们的API的详细信息，请参阅[API资源管理器](../../../wf-api/general/api-explorer.md)。

### 可用于报表的对象

在[!DNL Workfront] Web应用程序中使用Report Builder时，可以报告以下对象。 缩进项目符号提供了有关对象的更多信息，而不表示其他对象。

* [!UICONTROL 项目]
* [!UICONTROL 任务]
* [!UICONTROL 小时]
* [!UICONTROL 问题]
* [!UICONTROL 用户]
* [!UICONTROL 访问]级别
* [!UICONTROL 审批]
* [!UICONTROL 审批流程]
* [!UICONTROL 工作]
* [!UICONTROL 基线]
* [!UICONTROL 基线任务]
* [!UICONTROL 开票记录]
* [!UICONTROL 预算小时]
   * 这是[!UICONTROL 预算小时数]，它们显示在已弃用的旧版资源管理工具中。
   * “巴德。 [!UICONTROL 预算小时数]报告中的“小时数”字段引用[!UICONTROL 资源规划程序]中工作角色的预算小时数。 有关详细信息，请参阅[了解项目的[!UICONTROL 预算劳力成本]和[!UICONTROL 预算小时数]](../../../manage-work/projects/project-finances/budgeted-labor-cost.md)。

* [!UICONTROL 日历事件]
* [!UICONTROL 公司]
* [!UICONTROL 自定义表单]
* [!UICONTROL 仪表板]
* [!UICONTROL 文档]
* [!UICONTROL 文档审批]
* [!UICONTROL 文档版本]
   * 您可以查看有关文档版本、与版本关联的文档、版本创建者以及在文档版本上创建验证的用户（验证创建者）的信息。
* [!UICONTROL 电子邮件模板]
* [!UICONTROL 费用]
* [!UICONTROL 费用类型]
* [!UICONTROL 外部页面]
* [!UICONTROL 收藏]
* [!UICONTROL 筛选器]
* [!UICONTROL 目标]
   * 您可以为战略目标构建报告，或者在项目与目标关联作为目标活动时，在项目报告中显示与目标相关的信息。 只有贵组织购买了[!DNL Workfront Goals]许可证，您才能创建战略目标并将项目连接起来。 有关[!DNL Workfront Goals]的信息，请参阅[[!DNL Workfront Goals] 概述](../../../workfront-goals/goal-management/wf-goals-overview.md)。 有关将项目连接到战略目标的信息，请参阅[在Adobe Workfront目标中添加项目](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md)。
*您无法报告与[!UICONTROL 业务案例]关联的项目目标。 有关项目目标与战略目标的信息，请参阅[术语表 [!DNL Adobe Workfront] 术语](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

* [!UICONTROL 组]
* [!UICONTROL 分组]
* [!UICONTROL 小时类型]
* [!UICONTROL 计划]
   * 仅当您的公司购买了[!DNL Workfront Scenario Planner]许可证时，您才能为作为计划子对象的计划生成报告。 有关计划的信息，请参阅 [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md)中的[计划概述。

* 计划工作角色
   * 仅当您的公司购买了[!DNL Workfront Scenario Planner]许可证时，您才能为计划中与计划关联的工作角色生成报告。 有关创建计划并将其与工作角色关联的信息，请参阅[在 [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md)中创建和编辑计划。

* [!UICONTROL 迭代]
* [!UICONTROL 工作角色]
* [!UICONTROL 日志条目]
   * 您可以在[!UICONTROL 更新]对象区域（如任务、项目、问题等）中报告跟踪的系统更新。 有关详细信息，请参阅日志条目报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md)的[更新区域报告。

* [!UICONTROL 布局模板]
* [!UICONTROL 里程碑]
* [!UICONTROL 里程碑路径]
* [!UICONTROL 注释]或[!UICONTROL 更新]
   * 您可以报告单个用户添加的注释。

* [!UICONTROL 参数]（或[!UICONTROL 自定义字段]）
* [!UICONTROL 参数组]（或[!UICONTROL 分区界限]）
* [!UICONTROL Portfolio]
* [!UICONTROL 计划]
* [!UICONTROL 项目（财务数据）]
   * 财务信息仅会在与其关联的数据存在时间少于5年的情况下填充到[!UICONTROL 项目（财务数据）]报表中。 例如，如果某个工作角色在2015年1月分配给任务，而今天是2021年9月，则类似该工作角色的[!UICONTROL 分配日期]的财务文件未填充到[!UICONTROL 项目（财务数据）]报表中。

  >[!CAUTION]
  >
  >运行项目（财务数据）报表会重新计算财务数据，这会覆盖先前的财务数据，并且可能需要相当长的时间。 有关重新计算财务数据结果的详细信息，请参阅[重新计算项目财务](/help/quicksilver/manage-work/projects/project-finances/recalculate-project-finances.md)。

* [!UICONTROL 校对审批]
   * 允许您查看有关验证审批的各种信息，包括：提交以供审批的验证、有关[!UICONTROL 审批者]的信息、有关请求者的信息（如果请求者是已授予许可的[!DNL Workfront]用户）、版本信息、验证ID和验证创建日期。\
      [!UICONTROL 验证审批]报告仅包含在尚未做出决策的用户的“我的工作”区域中可用的验证。\
   * 验证审批在[!DNL Workfront]中分配，如[在 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)内共享验证[将用户添加到验证](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add)中所述。

* [!UICONTROL 队列]
* [!UICONTROL 队列主题]
* [!UICONTROL 费率] （这显示工作角色[!UICONTROL 记帐费率]信息）
* [!UICONTROL 提醒通知]
* [!UICONTROL 报告]
* [!UICONTROL 资源池]
* [!UICONTROL 风险]
* [!UICONTROL 风险类型]
* [!UICONTROL 计划]
* [!UICONTROL 记分卡]
* [!UICONTROL 团队]
* [!UICONTROL 模板]
* [!UICONTROL 模板任务]
* [!UICONTROL 休假]
   * 您可以报告用户在其个人资料中指示的空闲时间。

* [!UICONTROL 时间表]
* [!UICONTROL 周期性工时表]
* [!UICONTROL 主题组]
* [!UICONTROL 用户批准]
* [!UICONTROL 用户委派]

   * 您可以报告被委派在办公室外执行他人任务和问题的用户。 此报表显示外出用户以及在外出时履行职责的用户。

* [!UICONTROL 用户决策]

   * 您可以报告用户在当月对验证和文档做出了多少决策。

* [!UICONTROL 视图]
* [!UICONTROL 工作项] （这将生成任务和问题报告）
