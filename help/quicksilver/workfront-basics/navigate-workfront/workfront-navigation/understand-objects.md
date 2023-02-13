---
content-type: overview;reference
navigation-topic: workfront-navigation
title: 了解中的对象 [!DNL Adobe Workfront]
description: 了解中的对象 [!DNL Adobe Workfront]
feature: Get Started with Workfront
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 9c78d8e08e62c86a4e1340644ed76c61ce7f2674
workflow-type: tm+mt
source-wordcount: '2308'
ht-degree: 6%

---

# 了解中的对象 [!DNL Adobe Workfront]

<!--
<***Linked to several articles, do not remove/ change. 
-->

您在中显示的信息 [!DNL Adobe Workfront] 由存储在 [!DNL Workfront] 数据库。 对象是驱动信息的 [!DNL Workfront].

了解对象在 [!DNL Workfront] 非常重要，因此您可以根据组织中的需要使用正确的对象。

例如，当您计划大量工作时，您需要使用 [!UICONTROL 项目] 对象来定义该工作。 要将此工作划分为较小的计划增量，您可以使用 [!UICONTROL 任务] 对象。 对于未计划且可能意外发生的工作量较小的工作，您可以使用问题对象。 如果要跟踪一组项目的进度以及对预算和时间表的遵守情况，可以在 [!UICONTROL Portfolio] 和 [!UICONTROL 程序]. 要定义有助于解析工作的其他元素，您需要使用存储在 [!UICONTROL 项目], [!UICONTROL 任务], [!UICONTROL 问题]或 [!UICONTROL Portfolio]，如 [!UICONTROL 文档], [!UICONTROL 注释], [!UICONTROL 小时], [!UICONTROL 用户]或 [!UICONTROL 作业角色].

[!UICONTROL 报表] 和 [!UICONTROL 功能板] 对象的另一个示例可帮助您组织中的数据量 [!DNL Workfront] 以便所有用户都能轻松访问。

有关 [!DNL Workfront]，请参阅 [API Explorer](../../../wf-api/general/api-explorer.md).

## 对象的相互依赖和层次结构

对象在 [!UICONTROL Workfront]. 例如，任务或问题永远不能独立于项目之外存在。 [!UICONTROL 任务] 和 [!UICONTROL 问题] 是存储在 [!UICONTROL 项目] 对象。 [!UICONTROL 任务] 和 [!UICONTROL 问题] 被视为项目的子对象。

以下是 [!DNL Workfront] 及其各自的父项和子项对象：

| **对象** | **父对象** | **子对象** |
|---|---|---|
| [!UICONTROL 项目组合] |  | [!UICONTROL 程序], [!UICONTROL 项目], [!UICONTROL 文档], [!DNL Notes], [!UICONTROL 用户] |
| [!UICONTROL 项目群] | [!UICONTROL 项目组合] | [!UICONTROL 项目], [!UICONTROL 文档], [!UICONTROL 注释], [!UICONTROL 用户] |
| [!UICONTROL 项目] | [!UICONTROL Portfolio], [!UICONTROL 程序] | [!UICONTROL 任务], [!UICONTROL 问题], [!UICONTROL 文档], [!UICONTROL 注释], [!UICONTROL 小时], [!UICONTROL 用户] |
| [!UICONTROL 任务] | [!UICONTROL 项目] | [!UICONTROL 问题], [!UICONTROL 子任务], [!UICONTROL 文档], [!UICONTROL 注释], [!UICONTROL 小时], [!UICONTROL 用户] |
| [!UICONTROL 问题] | [!UICONTROL 任务], [!UICONTROL 项目] | [!UICONTROL 文档], [!UICONTROL 注释], [!UICONTROL 小时], [!UICONTROL 用户] |
| [!UICONTROL 仪表板] |  | [!UICONTROL 报表]，外部页面 |
| [!UICONTROL 报告] | [!UICONTROL 仪表板] |  |
| [!UICONTROL 组] |  | [!UICONTROL 用户] |
| [!UICONTROL 团队] |  | [!UICONTROL 用户] |
| [!UICONTROL 用户] | [!UICONTROL 群组], [!UICONTROL 团队], [!UICONTROL 公司] | [!UICONTROL 职位角色] |
| [!UICONTROL 公司] |  | [!UICONTROL 用户] |
| [!UICONTROL 文档] | [!UICONTROL 任务], [!UICONTROL 问题], [!UICONTROL 项目], [!UICONTROL Portfolio], [!UICONTROL 程序], [!UICONTROL 用户] |  |
| [!UICONTROL 计划]* |  | [!UICONTROL 计划] |
| [!DNL Goals]* |  | [!UICONTROL 结果], [!UICONTROL 活动] |

有关 [!DNL Workfront]，请参阅 [API Explorer](../../../wf-api/general/api-explorer.md).

*计划是 [!DNL Workfront Scenario Planner]. 有关 [!DNL Scenario Planner]，请参阅 [的 [!UICONTROL 方案规划器] 概述](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL 目标] 是 [!DNL Workfront Goals]. 有关 [!DNL Workfront Goals]，请参阅 [[!DNL Adobe Workfront Goals] 概述](../../../workfront-goals/goal-management/wf-goals-overview.md).


## 自定义对象名称

As a [!DNL Workfront] 管理员，可以在 [!DNL Workfront] 使用  [!UICONTROL 布局模板].

有关如何使用  [!UICONTROL 布局模板]，请参阅 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

在自定义布局模板并将其分配给用户后，这些用户将看到对象的自定义名称。 已分配到布局模板的用户不再在Web应用程序中的任意位置看到对象的默认名称。

>[!NOTE]
>
>要使用户能够看到对象的新名称，用户必须注销并重新登录到 [!DNL Workfront] 保存  [!UICONTROL 布局模板].

>[!IMPORTANT]
>
>的 [!DNL Workfront] 文档始终指对象的默认名称。 As a [!DNL Workfront] 管理员，请确保您通知用户对象名称的更改，以便他们了解如何使用 [!DNL Workfront] 文档，以及不反映对象名称更改的应用程序区域。

* [可使用  [!UICONTROL 布局模板]](#object-names-that-can-be-customized-using-a-layout-template)
* [区域 [!DNL Workfront] 反映自定义对象名称](#areas-of-workfront-that-reflect-the-customized-object-names)
* [区域 [!DNL Workfront] 不反映自定义对象名称](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### 可使用 [!UICONTROL 布局模板]

As a [!DNL Workfront] 管理员，您可以自定义以下对象的名称，以匹配您组织中的术语：

* [!UICONTROL 项目组合]
* [!UICONTROL 项目群]
* [!UICONTROL 项目]
* [!UICONTROL 任务]
* [!UICONTROL 问题]
* [!UICONTROL 目标]*
* [!UICONTROL 结果]*
* [!UICONTROL 活动]*

   *[!UICONTROL 目标], [!UICONTROL 结果]和 [!UICONTROL 活动] 仅当您的公司已购买时才可用 [!DNL Workfront Goals]. 有关 [!DNL Workfront Goals]，请参阅 [[!DNL Adobe Workfront Goals] 概述](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL 计划]**
* [!UICONTROL 方案]**
* [!UICONTROL 计划]**

   **[!UICONTROL 倡议], [!UICONTROL 情景]和 [!UICONTROL 计划] 仅当您的公司购买了 [!DNL Workfront Scenario Planner]. 有关 [!DNL Scenario Planner]，请参阅 [开始使用 [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).


例如，如果贵组织中的较大工作量称为“参与”，则可以替换名称“[!UICONTROL 项目]“参与度”。 您的 [!DNL Workfront] 界面显示“参与度”而不是“[!UICONTROL 项目]名称“”的任意位置[!UICONTROL 项目]将显示“ ”。

有关如何使用自定义对象名称的详细信息  [!UICONTROL 布局模板]，请参阅 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

您无法在Workfront中自定义任何其他对象的名称。 有关 [!DNL Workfront]，请参阅 [API Explorer](../../../wf-api/general/api-explorer.md).

自定义对象名称时，该对象的新名称会显示在 [!DNL Workfront] 显示对象名称的应用程序。

### 区域 [!DNL Workfront] 反映自定义对象名称

以下区域显示对象的更新名称：

* 顶端导航
* 左侧面板导航中的所有部分
* 所有菜单
* 应用程序内通知
* 报表生成器和报表元素（视图、过滤器和分组）
* [!UICONTROL 保存] 按钮
* 导出的文件
* 电子邮件
* 移动设备应用程序

### 区域 [!DNL Workfront] 不反映自定义对象名称

以下区域不显示对象的更新名称：

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] 插件

## 自定义对象名称的含义

在中自定义对象名称时，您应注意以下事项 [!DNL Workfront]:

* 在系统显示中，您可能会遇到文体或语法错误。 例如，如果重命名“[!UICONTROL 问题]“”到“Request”，您会在系统中的任意位置看到短语“An request”，该短语按预期运行，不应被视为错误。
* 对象的自定义名称不可翻译。 仅 [!DNL Workfront] 默认名称可以使用支持的语言进行翻译。 有关 [!DNL Workfront]，请参阅 [支持的语言 [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). 自定义对象名称字段支持外国字符，因此您可以输入任何语言的术语。
* 使用  [!UICONTROL 布局模板]，我们建议您将  [!UICONTROL 布局模板] 团队或组)的相关信息。\
   我们建议您使用这些业务部门的用户清楚了解的名称，以避免混淆。
* 电子邮件通知和传送的报表始终包含由  [!UICONTROL 布局模板] 生成电子邮件的用户。 如果用户收到来自其他团队和组中的用户的电子邮件通知，则应准备在其电子邮件中看到与其组或团队无关的对象名称。\
   As a [!DNL Workfront] 管理员建议用户注意与每个对象关联的图标。 图标在各种对象名称之间保持一致，并且与默认对象一致，因为它显示在数据库中。 要获取所有 [!DNL Workfront] 与对象关联的图标，请参阅 [对象图标](#object-icons).

   >[!TIP]
   >
   >有关组织中的常见任务，请考虑创建自定义文档以反映您的术语。

## 对象图标

的 [!DNL Workfront] 文档始终指对象的默认名称。 如果对象已自定义其名称，则您可以依赖与其关联的图标来了解与哪个自定义对象对应的自定义对象 [!DNL Workfront] 默认对象。

有关哪些对象在中可以具有自定义名称的详细信息 [!DNL Workfront]，请参阅 [可使用  [!UICONTROL 布局模板]](#object-names-that-can-be-customized-using-a-layout-template).

以下是Workfront中的对象及其相应图标的列表。

| **对象** | **图标** | **可自定义的对象名称** |
|---|---|---|
| [!UICONTROL 公司] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL 仪表板] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL 目标] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL 组] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL 问题] | ![](assets/issue-icon-nwe.png)  , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL 工作角色] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL 计划] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL 项目组合] | ![](assets/portfolio-icon-nwe.png)  , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL 项目群] | ![](assets/program-icon-nwe.png)  , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL 项目] | ![](assets/project-icon-nwe.png)  , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL 报告] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL 任务] | ![](assets/task-icon-new.png)  , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL 团队] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL 模板] | ![](assets/template-icon-nwe.png)  , ![](assets/nwe-templates-icon.png) |  |

## 对象的参考编号

在中创建的每个对象 [!DNL Workfront] 分配了一个唯一的引用编号。 在区分两个其他相似对象（例如具有相同名称的任务）时，引用编号非常有用。 您可以使用对象的参考编号来搜索对象，并可以在报表中包含参考编号。

有关如何按参考编号搜索对象的信息，请参阅 [使用对象的引用数](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## 特定于对象的搜索

您可以搜索 [!DNL Workfront]，或者也可以选择要在基本和高级搜索中搜索的特定对象。

并非所有对象都可以在 [!DNL Workfront]. 您可以在 [!DNL Workfront]:

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
| [!UICONTROL 注释] | ✓ |  |

有关在中运行基本搜索和高级搜索的详细信息 [!DNL Workfront]，请参阅 [搜索 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

## 对象报告

在开始在中构建报表之前，了解对象的层次结构和相互依赖关系非常重要 [!DNL Workfront]. 报表特定于对象。 您必须为报表选择正确的对象，然后才能显示所需的数据。

根据您为报表选择的对象，您只能访问直接链接到报表对象的对象。

>[!IMPORTANT]
>
>您只能报告所选对象以及同一报表中的父对象。 不能在父对象报表中包含有关子对象的信息。 例如，您可以在任务报表中显示项目信息，但不能在项目报表中显示任务信息。

您可以使用我们的打开API报告数据库中的所有对象。 有关数据库中所有对象的完整列表，请参阅 [API Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>如果您已使用布局模板自定义了对象的名称，则Report Builder中对象的名称也已自定义。 确保您知道哪些对象已自定义，并在报表生成器中查找自定义名称。 有关哪些对象在中可以具有自定义名称的详细信息 [!DNL Workfront]，请参阅 *[可使用  [!UICONTROL 布局模板]](#object-names-that-can-be-customized-using-a-layout-template).*
>在报表中使用文本模式时，文本模式表达式中对象的名称是 [!DNL Workfront]，而不是自定义对象名称。 有关在报表中使用文本模式的更多信息，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

有关构建报表的更多信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
有关我们的API的更多信息，请参阅 [API Explorer](../../../wf-api/general/api-explorer.md).

在 [!DNL Workfront] web应用程序：

* [!UICONTROL 项目]
* [!UICONTROL 任务]
* [!UICONTROL 小时]
* [!UICONTROL 问题]
* [!UICONTROL 用户]
* [!UICONTROL 访问级别]
* [!UICONTROL 审批]
* [!UICONTROL 批准流程]
* [!UICONTROL 分配]
* [!UICONTROL 积压工作项]\
   显示敏捷积压工作的任务或问题。 有关敏捷积压的详细信息，请参阅 [管理敏捷积压](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

* [!UICONTROL 基线]
* [!UICONTROL 基线任务]
* [!UICONTROL 开票记录]
* [!UICONTROL 预算小时]

   这是 [!UICONTROL 预算小时数]，它们显示在已弃用的旧资源管理工具中。

   &quot;巴德&quot; “小时”字段 [!UICONTROL 预算小时数] 报表是指 [!UICONTROL 资源计划员]. 有关更多信息，请参阅 [了解 [!UICONTROL 预算人工成本] 和 [!UICONTROL 预算小时数] 用于项目](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL 日历事件]
* [!UICONTROL 类别] (或 [!UICONTROL 自定义表单])
* [!UICONTROL 公司]
* [!UICONTROL 仪表板]
* [!UICONTROL 文档]
* [!UICONTROL 文档审批]
* [!UICONTROL 文档版本]\
   允许您查看有关文档版本、与版本关联的文档、创建版本的人员以及文档版本上创建校样（如果存在）的用户的各种信息（校样创建者）。
* [!UICONTROL 电子邮件模板]
* [!UICONTROL 费用]
* [!UICONTROL 费用类型]
* [!UICONTROL 外部页面]
* [!UICONTROL 收藏夹]
* [!UICONTROL 筛选]
* [!UICONTROL 目标]

   您可以为战略目标构建报表，或者在项目与目标关联作为目标活动时，在项目报表中显示与目标相关的信息。 您只能在贵组织购买了 [!DNL Workfront Goals] 许可证。 有关 [!DNL Workfront Goals]，请参阅 [[!DNL Workfront Goals] 概述](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWorkfront_Goals%2FGoal_management%2Fwf-goals-overview.htm&amp;_LANG=en). 有关将项目与战略目标连接的信息，请参阅 [将项目添加到Adobe Workfront目标中的目标](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWorkfront_Goals%2FResults_and_activities%2Fconnect-projects-to-goals-overview.htm&amp;_LANG=en).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: hardcoded links in this paragraph)
  </MadCap:conditionalText>
  -->

   >[!TIP]
   >
   >您无法报告与 [!UICONTROL 商业案例]. 有关项目目标与战略目标的信息，请参阅 [术语表 [!DNL Adobe Workfront] 术语](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL 组]
* [!UICONTROL 分组]
* [!UICONTROL 小时数类型]
* [!UICONTROL 计划]

   只有在您的公司购买了 [!DNL Workfront Scenario Planner] 许可证。 有关计划的信息，请参阅 [中的计划概述 [!DNL Workfront Scenario Planner]](https://one.workfront.com/s/csh?context=2066&amp;pubname=the-new-workfront-experience).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this link is hardcoded)
  </MadCap:conditionalText>
  -->

* 计划工作角色

   仅当您的公司购买了 [!DNL Workfront Scenario Planner] 许可证。 有关创建方案并将其与职务角色关联的信息，请参阅 [在 [!DNL Workfront Scenario Planner]](https://one.workfront.com/s/csh?context=2061&amp;pubname=the-new-workfront-experience).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this link is hardcoded)
  </MadCap:conditionalText>
  -->

* [!UICONTROL 迭代]
* [!UICONTROL 工作角色]
* [!UICONTROL 日志条目]

   您可以在 [!UICONTROL 更新] 任务、项目、问题等对象的区域。 要了解更多信息，请参阅 [报告 [!UICONTROL 更新] 面积](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL 布局模板]
* [!UICONTROL 里程碑]
* [!UICONTROL 里程碑路径]
* [!UICONTROL 注释]

   >[!NOTE]
   >
   >您可以报告由个人用户添加的评论。

* [!UICONTROL 参数] (或 [!UICONTROL 自定义字段])
* [!UICONTROL 参数组] (或 [!UICONTROL 区域划分])
* [!UICONTROL 门户配置文件] （这会显示已弃用的信息）
* [!UICONTROL 项目组合]
* [!UICONTROL 项目群]
* [!UICONTROL 项目] ([!UICONTROL 财务数据])

   >[!NOTE]
   >
   >财务信息填充于 [!UICONTROL 项目] ([!UICONTROL 财务数据])报表。 例如，如果在2015年1月为某项任务分配了工作角色，而今天是2021年9月，则会有类似 [!UICONTROL 分配日期] 对于作业角色，不会在 [!UICONTROL 项目（财务数据）] 报表。

* [!UICONTROL 校对审批]\
   允许您查看有关校样批准的各种信息，包括：提交审批的证明，关于 [!UICONTROL 审批者]，有关请求者的信息（如果请求者是许可的） [!DNL Workfront] 用户)、版本信息、校样ID和校样创建日期。\
   [!UICONTROL 校样批准] 报表只包含用户“我的工作”区域中可用的校样，这些区域尚未做出决策。\
   校样批准在 [!DNL Workfront] 如所述 [将用户添加到校样](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [在中共享校样 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL 队列]
* [!UICONTROL 队列主题]
* [!UICONTROL 比率] （显示作业角色） [!UICONTROL 计费费率] 信息)
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

   您可以报告用户在其配置文件中指示的休息时间。

* [!UICONTROL 时间表]
* [!UICONTROL 时间表配置文件]
* [!UICONTROL 主题组]
* [!UICONTROL 用户委托]

   您可以报告已委派用户在他人不在办公室时执行其任务和问题的用户。 此报表显示不在办公室的用户以及在外出时履行职责的用户。

* [!UICONTROL 查看]
* [!UICONTROL 工作项] （这是指任务和问题）
