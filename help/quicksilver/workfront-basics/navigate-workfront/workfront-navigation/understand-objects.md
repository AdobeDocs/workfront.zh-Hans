---
content-type: overview;reference
navigation-topic: workfront-navigation
title: 了解中的对象 [!DNL Adobe Workfront]
description: 了解中的对象 [!DNL Adobe Workfront]
feature: Get Started with Workfront
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: a2650ccc3deffd841a7b497e6ff1b5eed6145211
workflow-type: tm+mt
source-wordcount: '2255'
ht-degree: 7%

---

# 了解中的对象 [!DNL Adobe Workfront]

<!--
<***Linked to several articles, do not remove/ change. 
-->

您在中显示的信息 [!DNL Adobe Workfront] 由存储在文件中的对象表示。 [!DNL Workfront] 数据库。 对象是驱动信息的 [!DNL Workfront].

了解在中如何定义对象 [!DNL Workfront] 非常重要，因此，您可以使用正确的对象来满足组织内的必要需求。

例如，当您计划大量工作时，您需要使用 [!UICONTROL 项目] 对象以定义该工作。 要将此工作划分为较小的计划增量，您可以使用 [!UICONTROL 任务] 对象。 对于少量未计划且可能意外发生的工作，您可以使用Issue对象。 如果要跟踪一组项目的进度以及是否遵守预算和时间表，您可以组织这些项目 [!UICONTROL Portfolio] 和 [!UICONTROL 程序]. 要定义有助于您解决工作的其他元素，您需要使用存储在下的其他对象 [!UICONTROL 项目]， [!UICONTROL 任务]， [!UICONTROL 问题]，或 [!UICONTROL Portfolio]，点赞 [!UICONTROL 文档]， [!UICONTROL 更新]， [!UICONTROL 小时]， [!UICONTROL 用户]，或 [!UICONTROL 职位角色].

[!UICONTROL 报表] 和 [!UICONTROL 仪表板] 是另一个对象示例，可帮助您整理其中包含的数据量 [!DNL Workfront] 以可视方式创建，以便所有用户都能轻松访问。

有关中对象的完整列表 [!DNL Workfront]，请参见 [API资源管理器](../../../wf-api/general/api-explorer.md).

## 对象的相互依赖性和层次结构

对象在中相互链接 [!UICONTROL Workfront]. 例如，任务或问题永远不能独立于项目之外存在。 [!UICONTROL 任务] 和 [!UICONTROL 问题] 是存储在中的对象示例 [!UICONTROL 项目] 对象。 [!UICONTROL 任务] 和 [!UICONTROL 问题] 被视为项目的子对象。

以下是中一些最常用的对象 [!DNL Workfront] 以及它们各自的父对象和子对象：

| **对象** | **父对象** | **子对象** |
|---|---|---|
| [!UICONTROL 项目组合] |  | [!UICONTROL 程序]， [!UICONTROL 项目]， [!UICONTROL 文档]， [!DNL Notes]， [!UICONTROL 用户] |
| [!UICONTROL 项目群] | [!UICONTROL 项目组合] | [!UICONTROL 项目]， [!UICONTROL 文档]， [!UICONTROL 注释]， [!UICONTROL 用户] |
| [!UICONTROL 项目] | [!UICONTROL Portfolio]， [!UICONTROL 程序] | [!UICONTROL 任务]， [!UICONTROL 问题]， [!UICONTROL 文档]， [!UICONTROL 注释]， [!UICONTROL 小时]， [!UICONTROL 用户] |
| [!UICONTROL 任务] | [!UICONTROL 项目] | [!UICONTROL 问题]， [!UICONTROL 子任务]， [!UICONTROL 文档]， [!UICONTROL 注释]， [!UICONTROL 小时]， [!UICONTROL 用户] |
| [!UICONTROL 问题] | [!UICONTROL 任务]， [!UICONTROL 项目] | [!UICONTROL 文档]， [!UICONTROL 注释]， [!UICONTROL 小时]， [!UICONTROL 用户] |
| [!UICONTROL 仪表板] |  | [!UICONTROL 报表]，外部页面 |
| [!UICONTROL 报告] | [!UICONTROL 仪表板] |  |
| [!UICONTROL 组] |  | [!UICONTROL 用户] |
| [!UICONTROL 团队] |  | [!UICONTROL 用户] |
| [!UICONTROL 用户] | [!UICONTROL 组]， [!UICONTROL 团队]， [!UICONTROL 公司] | [!UICONTROL 职位角色] |
| [!UICONTROL 公司] |  | [!UICONTROL 用户] |
| [!UICONTROL 文档] | [!UICONTROL 任务]， [!UICONTROL 问题]， [!UICONTROL 项目]， [!UICONTROL Portfolio]， [!UICONTROL 程序]， [!UICONTROL 用户] |  |
| [!UICONTROL 计划]* |  | [!UICONTROL 计划] |
| [!DNL Goals]* |  | [!UICONTROL 结果]， [!UICONTROL 活动] |

有关中对象的完整列表 [!DNL Workfront]，请参见 [API资源管理器](../../../wf-api/general/api-explorer.md).

*计划是 [!DNL Adobe Workfront Scenario Planner]. 欲知关于 [!DNL Scenario Planner]，请参见 [此 [!UICONTROL 场景规划器] 概述](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL 目标] 是以下对象的对象 [!DNL Adobe Workfront Goals]. 有关信息 [!DNL Workfront Goals]，请参见 [[!DNL Adobe Workfront Goals] 概述](../../../workfront-goals/goal-management/wf-goals-overview.md).


## 自定义对象名称

作为 [!DNL Workfront] 管理员，您可以在中自定义对象名称 [!DNL Workfront] 通过使用  [!UICONTROL 布局模板].

有关如何使用自定义对象名称的详细信息  [!UICONTROL 布局模板]，请参见 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

在自定义版面模板并将其分配给用户后，这些用户将看到对象的自定义名称。 已分配给布局模板的用户不再看到Web应用程序中任何位置的对象的缺省名称。

>[!NOTE]
>
>要让用户看到对象的新名称，用户必须注销并重新登录到 [!DNL Workfront] 保存  [!UICONTROL 布局模板].

>[!IMPORTANT]
>
>此 [!DNL Workfront] 文档始终引用对象的默认名称。 作为 [!DNL Workfront] 管理员，确保将对象名称的更改通知用户，以便用户了解如何使用 [!DNL Workfront] 文档以及不反映对象名称更改的应用程序区域。

* [可以使用自定义的对象名称  [!UICONTROL 布局模板]](#object-names-that-can-be-customized-using-a-layout-template)
* [领域 [!DNL Workfront] 反映自定义对象名称的](#areas-of-workfront-that-reflect-the-customized-object-names)
* [领域 [!DNL Workfront] 无法反映自定义对象名称](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### 可以使用自定义的对象名称 [!UICONTROL 布局模板]

作为 [!DNL Workfront] 管理员，您可以自定义以下对象的名称以匹配组织中的术语：

* [!UICONTROL 项目组合]
* [!UICONTROL 项目群]
* [!UICONTROL 项目]
* [!UICONTROL 任务]
* [!UICONTROL 问题]
* [!UICONTROL 目标]*
* [!UICONTROL 结果]*
* [!UICONTROL 活动]*

  *[!UICONTROL 目标]， [!UICONTROL 个结果]、和 [!UICONTROL 活动] 仅在贵公司购买后才可用 [!DNL Workfront Goals]. 有关信息 [!DNL Workfront Goals]，请参见 [[!DNL Adobe Workfront Goals] 概述](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL 计划]**
* [!UICONTROL 方案]**
* [!UICONTROL 计划]**

  **[!UICONTROL 计划]， [!UICONTROL 方案]、和 [!UICONTROL 计划] 仅当您的公司购买了 [!DNL Workfront Scenario Planner]. 欲知关于 [!DNL Scenario Planner]，请参见 [开始使用 [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).


例如，如果贵组织中的大量工作称为“参与”，则可以替换名称“[!UICONTROL 项目]”与“Engagement”。 您的 [!DNL Workfront] 界面显示“Engagement”而不是“[!UICONTROL 项目]&#39;名称处&#39;[!UICONTROL 项目]”将会出现。

有关如何使用自定义对象名称的详细信息  [!UICONTROL 布局模板]，请参见 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

您无法在Workfront中自定义任何其他对象的名称。 有关中对象的完整列表 [!DNL Workfront]，请参见 [API资源管理器](../../../wf-api/general/api-explorer.md).

自定义对象名称时，该对象的新名称会出现在对象的大部分区域中。 [!DNL Workfront] 显示对象名称的应用程序。

### 领域 [!DNL Workfront] 反映自定义对象名称的

以下区域显示对象的更新名称：

* 顶端导航
* 左侧面板导航中的所有部分
* 所有菜单
* 应用程序内通知
* Report Builder和报告元素（视图、筛选器和分组）
* [!UICONTROL 保存] 按钮
* 导出的文件
* 电子邮件
* 移动应用程序

### 领域 [!DNL Workfront] 无法反映自定义对象名称

以下区域不显示对象的更新名称：

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] 加载项

### 自定义对象名称的含义

在中自定义对象名称时，您应了解以下事项 [!DNL Workfront]：

* 在系统显示中可能会遇到文体或语法错误。 例如，如果重命名“[!UICONTROL 问题]”更改为“请求”，并且您在系统中的任何位置看到“请求”短语，则表示这按预期运行，不应被视为错误。
* 对象的自定义名称不可翻译。 仅 [!DNL Workfront] 默认名称可以使用支持的语言进行翻译。 有关支持的语言的详细信息 [!DNL Workfront]，请参见 [中支持的语言 [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). 自定义对象名称字段支持外字符，因此您可以用任何语言输入术语。
* 当您使用自定义对象名称时  [!UICONTROL 布局模板]，我们建议您将  [!UICONTROL 布局模板] 在您的业务部门（团队或组）周围。\
   我们建议您使用这些业务部门用户能够清晰理解的名称以避免混淆。
* 电子邮件通知和传送的报表始终包含由定义的对象名称  [!UICONTROL 布局模板] 生成电子邮件的用户的名称。 如果您的用户从其他团队和组中的用户收到电子邮件通知，则您应当准备好在其电子邮件中看到与组或团队无关的对象名称。\
   作为 [!DNL Workfront] 管理员，建议用户注意与每个对象关联的图标。 图标在各种对象名称之间保持一致并与默认对象一致，如显示在数据库中的那样。 用于所有内容的列表 [!DNL Workfront] 与对象关联的图标，请参阅 [对象图标](#object-icons).

  >[!TIP]
  >
  >对于组织中的常见任务，请考虑创建自定义文档以反映您的术语。

## 对象图标

此 [!DNL Workfront] 文档始终引用对象的默认名称。 如果您的对象已自定义其名称，您可以依靠与其关联的图标来了解哪个自定义对象对应于哪个自定义对象 [!DNL Workfront] 默认对象。

有关哪些对象可以具有自定义名称的详细信息 [!DNL Workfront]，请参见 [可以使用自定义的对象名称  [!UICONTROL 布局模板]](#object-names-that-can-be-customized-using-a-layout-template).

以下是Workfront中的对象及其相应图标的列表。

| **对象** | **图标** | **可自定义的对象名称** |
|---|---|---|
| [!UICONTROL 公司] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL 仪表板] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL 目标] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL 组] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL 问题] | ![](assets/issue-icon-nwe.png)  , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL 工作角色] | ![job_role_icon.png](assets/job-role-icon-52x50.png)， ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png)， ![](assets/job-role-nwe-no-color.png)， ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL 计划] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL 项目组合] | ![](assets/portfolio-icon-nwe.png)  , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL 项目群] | ![](assets/program-icon-nwe.png)  , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL 项目] | ![](assets/project-icon-nwe.png)  , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL 报告] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL 任务] | ![](assets/task-icon-new.png)  , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL 团队] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL 模板] | ![](assets/template-icon-nwe.png)  , ![](assets/nwe-templates-icon.png) |  |

## 对象的参考编号

在中创建的每个对象 [!DNL Workfront] 分配了唯一参考编号。 参考号有助于区分两个在其他方面相似的对象（如同名的任务）。 您可以使用对象的参考编号来搜索对象，也可以在报表中包括参考编号。

有关如何按参考号搜索对象的信息，请参见 [使用对象的参考编号](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## 对象特定的搜索

您可以搜索所有可在中搜索的对象 [!DNL Workfront]，或者，您可以选择要在基本和高级搜索中搜索的特定对象。

并非所有对象都可在中搜索 [!DNL Workfront]. 您可以在中运行对以下对象的基本和高级搜索 [!DNL Workfront]：

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
| [!UICONTROL 项目群] | ✓ | ✓ |
| [!UICONTROL 仪表板] | ✓ | ✓ |
| [!UICONTROL 公司] | ✓ | ✓ |
| [!UICONTROL 注释] (或 [!UICONTROL 更新]) | ✓ |  |

有关在中运行基本搜索和高级搜索的详细信息 [!DNL Workfront]，请参见 [Search [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

## 对象报表

在您开始在中构建报表之前，了解对象的层次和相互依赖关系非常重要 [!DNL Workfront]. 报告特定于对象。 您必须先为报表选择正确的对象，然后才能显示所需的数据。

根据您为报表选择的对象，您只能访问直接链接到报表对象的对象。

>[!IMPORTANT]
>
>您只能在同一个报表中报告所选对象和父对象。 父对象报表中不能包含有关子对象的信息。 例如，您可以在任务报告中显示项目信息，但不能在项目报告中显示任务信息。

您可以使用我们的开放API报告数据库中的所有对象。 有关数据库中所有对象的完整列表，请参见 [API资源管理器](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>如果您已使用布局模板自定义了对象名称，则也会自定义Report Builder中的对象名称。 确保您知道哪些对象已自定义，并在Report Builder中查找自定义名称。 有关哪些对象可以具有自定义名称的详细信息 [!DNL Workfront]，请参见 *[可以使用自定义的对象名称  [!UICONTROL 布局模板]](#object-names-that-can-be-customized-using-a-layout-template).*
>在报表中使用文本模式时，文本模式表达式中的对象名称是中的标准名称。 [!DNL Workfront]，而不是自定义的对象名称。 有关在报表中使用文本模式的详细信息，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

有关构建报表的更多信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
有关我们的API的更多信息，请参阅 [API资源管理器](../../../wf-api/general/api-explorer.md).

在中使用报表生成器时，您可以报告以下对象 [!DNL Workfront] Web应用程序：

* [!UICONTROL 项目]
* [!UICONTROL 任务]
* [!UICONTROL 小时]
* [!UICONTROL 问题]
* [!UICONTROL 用户]
* [!UICONTROL 访问级别]
* [!UICONTROL 审批]
* [!UICONTROL 批准流程]
* [!UICONTROL 分配]
<!--this is no longer available: * [!UICONTROL Backlog Work Item]\
   Displays tasks or issues on the agile backlog. For more information about the agile backlog, see [Manage the agile backlog](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).-->

* [!UICONTROL 基线]
* [!UICONTROL 基线任务]
* [!UICONTROL 开票记录]
* [!UICONTROL 预算小时]

  这是 [!UICONTROL 预算小时数]，如在已弃用的旧版资源管理工具中所示。

  “巴德。 “小时”字段 [!UICONTROL 预算小时] 报告是指为工作角色预算的小时数，在 [!UICONTROL 资源规划者]. 有关更多信息，请参阅 [了解 [!UICONTROL 预算劳力成本] 和 [!UICONTROL 预算小时数] 用于项目](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL 日历事件]
* [!UICONTROL 公司]
* [!UICONTROL 自定义表单]
* [!UICONTROL 仪表板]
* [!UICONTROL 文档]
* [!UICONTROL 文档审批]
* [!UICONTROL 文档版本]\
   您可以查看有关文档版本、与版本关联的文档、版本创建者以及在文档版本上创建验证的用户（验证创建者）的信息。
* [!UICONTROL 电子邮件模板]
* [!UICONTROL 费用]
* [!UICONTROL 费用类型]
* [!UICONTROL 外部页面]
* [!UICONTROL 收藏夹]
* [!UICONTROL 筛选]
* [!UICONTROL 目标]

  您可以为战略目标构建报告，或者在项目与目标关联作为目标活动时，在项目报告中显示与目标相关的信息。 只有贵组织购买了，您才能创建战略目标并将项目联系起来 [!DNL Workfront Goals] 许可证。 有关信息 [!DNL Workfront Goals]，请参见 [[!DNL Workfront Goals] 概述](../../../workfront-goals/goal-management/wf-goals-overview.md). 有关将项目连接到战略目标的信息，请参阅 [将项目添加到Adobe Workfront目标中的目标](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

  >[!TIP]
  >
  >您无法报告与关联的项目目标 [!UICONTROL 商业论证]. 有关项目目标与战略目标的信息，请参阅 [术语表 [!DNL Adobe Workfront] 术语](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL 组]
* [!UICONTROL 分组]
* [!UICONTROL 小时数类型]
* [!UICONTROL 计划]

  仅当您的公司已购买计划时，您才可以为作为计划子对象的计划构建报告 [!DNL Workfront Scenario Planner] 许可证。 有关计划的信息，请参阅 [中的计划概述 [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md).


* 计划工作角色

  仅当您的公司已购买计划时，您才能为与计划中的计划关联的工作角色构建报告 [!DNL Workfront Scenario Planner] 许可证。 有关创建方案并将其与工作角色关联的信息，请参阅 [在中创建和编辑计划 [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md).


* [!UICONTROL 迭代]
* [!UICONTROL 工作角色]
* [!UICONTROL 日志条目]

  您可以在中报告跟踪的系统更新 [!UICONTROL 更新] 诸如任务、项目、问题等对象的区域。 要了解更多信息，请参阅 [报告 [!UICONTROL 更新] 区域](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL 布局模板]
* [!UICONTROL 里程碑]
* [!UICONTROL 里程碑路径]
* [!UICONTROL 注意] 或 [!UICONTROL 更新]

  >[!NOTE]
  >
  >您可以报告单个用户添加的注释。

* [!UICONTROL 参数] (或 [!UICONTROL 自定义字段])
* [!UICONTROL 参数组] (或 [!UICONTROL 分节符])
  <!--this is no longer in the UI: * [!UICONTROL Portal Profile] (this displays information that has been deprecated)-->
* [!UICONTROL 项目组合]
* [!UICONTROL 项目群]
* [!UICONTROL 项目] ([!UICONTROL 财务数据])

  >[!NOTE]
  >
  >财务信息填充于 [!UICONTROL 项目] ([!UICONTROL 财务数据])仅当与其关联的数据的保留时间少于5年时才报告。 例如，如果某个工作角色在2015年1月分配给某个任务，而今天是2021年9月，则类似于 [!UICONTROL 分配日期] 因为工作角色不会填充到 [!UICONTROL 项目（财务数据）] 报告。

* [!UICONTROL 校对审批]\
   允许您查看有关验证审批的各种信息，包括：提交以供审批的验证、关于 [!UICONTROL 审批者]，有关请求者的信息（如果请求者已获得许可） [!DNL Workfront] 用户)、版本信息、验证ID和验证创建日期。\
   [!UICONTROL 校对审批] 报告仅包含在尚未做出决策的用户的“我的工作”区域中可用的验证。\
   验证审批分配于 [!DNL Workfront] 如所述 [将用户添加到验证](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) 在 [在中共享验证 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL 队列]
* [!UICONTROL 队列主题]
* [!UICONTROL 费率] (此设置将显示工作角色 [!UICONTROL 记帐费率] 信息)
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
* [!UICONTROL 空闲时间]

  您可以报告用户在其个人资料中指示的空闲时间。

* [!UICONTROL 时间表]
* [!UICONTROL 时间表配置文件]
* [!UICONTROL 主题组]
* [!UICONTROL 用户审批]
* [!UICONTROL 用户委托]

  您可以报告被委派在办公室外执行他人任务和问题的用户。 此报表显示外出用户以及在外出时履行职责的用户。

* [!UICONTROL 用户决策]

  您可以报告用户在当月对验证和文档做出了多少决策。

* [!UICONTROL 查看]
* [!UICONTROL 工作项] （这将生成任务和问题报告）
