---
content-type: reference
navigation-topic: workfront-navigation
title: ' [!DNL Workfront]中的项目、任务和问题日期概述'
description: 本文提供了与 [!DNL Adobe Workfront]中的项目、任务和问题相关的最常见日期的定义。
feature: Get Started with Workfront
author: Alina
exl-id: 3808200f-a573-4c39-8965-b254f69c893c
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '2357'
ht-degree: 3%

---

# [!DNL Workfront]中的项目、任务和问题日期概述

<!-- Audited: 05/2024 -->

<!--consider expanding on this article with ALL dates for PTIs - Hand off dates, Approval Dates, etc-->

<!-- there are dates below that need definition - ask Product-->

本文提供了与[!DNL Adobe Workfront]中的项目、任务和问题相关的最常见日期的定义。 此处包含的图像是日期在Workfront中显示的示例，并非详尽无遗。 还有其他区域显示日期。 所有日期还可在项目、任务和问题报告和列表中可见。

有关报告和列表的信息，请参阅以下文章：

* [开始使用 [!DNL Adobe Workfront]中的列表](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)
* [报告入门](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)

有关项目、任务和问题字段的详细信息，请参阅[术语表 [!DNL Adobe Workfront] ](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。


## [!UICONTROL 实际开始日期]

[!UICONTROL 实际开始日期]是用户实际开始处理项目、任务或问题的日期。 创建项目、任务或问题时，[!UICONTROL 实际开始日期]为空。

您可以手动指示任务或问题的工作何时开始，或者在任务或问题状态从[!UICONTROL 新建]更改为[!UICONTROL 进行中]或[!UICONTROL 完成]时，自动填充[!UICONTROL 实际开始日期]。 项目的[!UICONTROL 实际开始日期]与项目上第一个任务的开始日期一致。

>[!TIP]
>
>[!UICONTROL 实际开始日期]可能与项目、任务或问题的[!UICONTROL 计划开始日期]不匹配，因为用户可能在其计划日期之前或之后开始工作。

有关详细信息，请参阅项目[!UICONTROL 实际开始日期][&#128279;](../../../manage-work/projects/planning-a-project/project-actual-start-date.md)的概述。

>[!NOTE]
>
>[!UICONTROL 必须在]任务开始，或者固定日期约束会影响任务的[!UICONTROL 计划开始日期]，而不是[!UICONTROL 实际开始日期]。 这会将[!UICONTROL 计划开始日期]更新为您指定的日期。 [!UICONTROL 实际开始日期]的更新与[!UICONTROL 计划开始日期]无关，如上所述。

![编辑任务的实际开始日期](assets/actual-start-date-on-edit-task-highlighted-nwe-350x251.png)

![任务的实际开始日期](assets/actual-start-date-on-task-details-highlighted-nwe-350x191.png)

## [!UICONTROL 实际完成日期]

[!UICONTROL 实际完成日期]是用户实际完成项目、任务或问题的日期。 创建项目、任务或问题时，[!UICONTROL 实际完成日期]为空。

您可以手动指示任务或问题的工作何时完成，或者在出现以下任何情况时自动填充[!UICONTROL 实际完成日期]：

* 项目、任务或问题状态更改为[!UICONTROL 完成]、[!UICONTROL 已关闭]或[!UICONTROL 已解决]。
* 任务或项目完成百分比为100%。

项目的[!UICONTROL 实际完成日期]与您在项目上完成最后一个任务的日期重合。

>[!TIP]
>
>[!UICONTROL 实际完成日期]可能与[!UICONTROL 计划完成日期]不匹配。

有关详细信息，请参阅项目[!UICONTROL 实际完成日期][&#128279;](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md)的概述。

![实际完成日期详细信息](assets/actual-completion-date-task-details-highlighted-nwe-350x189.png)

## 审批路径完成日期

批准路径完成日期是授予项目、任务或问题批准并更改项目状态的日期。

批准路径完成日期在项目、任务、问题列表和报告中可见。

## 审批路径开始日期

审批路径开始日期是指将项目、任务或问题状态更改为“未决审批”并将项目审批请求发送给审批者的日期。

批准路径开始日期在项目、任务、问题列表和报告中可见。

<!--## Auto Closure Date -->

## 预算完成日期

这是已弃用的项目字段。 此字段可能在列表或报告中显示的任何信息都与Workfront已移除的功能相关。 无法更新此字段。

该字段在项目报告和列表中可见。

## 预算开始日期

这是已弃用的项目字段。 此字段可能显示的任何信息都与Workfront已删除的功能相关。 无法更新此字段。

该字段在项目报告和列表中可见。

## [!UICONTROL 提交日期]

[!UICONTROL 提交日期]是分配给任务或问题的用户提交完成任务或问题的日期。 这与[!UICONTROL 规划完成日期]不同，因为它是仅由负责工作的用户提供的对完成日期的更现实的估计。 有关详细信息，请参阅[[!UICONTROL 提交日期]概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)。

>[!NOTE]
>
>更改[!UICONTROL 提交日期]将影响[!UICONTROL 预计完成日期]，但不影响任务或问题的[!UICONTROL 计划完成日期]。 项目经理可以使用被分派人在[!UICONTROL 提交日期]所做的更改来更新任务或问题的[!UICONTROL 规划完成日期]。

<!--## Completion Pending Date-->

## 限制日期

如果您使用的是绑定到特定日期的任务限制日期，则该特定日期将成为任务的限制日期。

以下任务约束将更新“约束日期”字段：

* 必须开始时间
* 必须完成时间
* 开始时间不晚于
* 开始时间不早于

>[!TIP]
>
>具有固定日期限制的任务没有限制日期。
>

“限制日期”在任务列表或报告中可见。

## 转换的问题输入日期

转化为项目或任务的问题的创建日期。

转换的问题输入日期在项目、任务列表和报告中可见。

## 到期日期

任务或问题应完成的日期。 任务或问题的到期日期与计划完成日期相同。

任务和问题到期日期显示在任务和问题列表及报告中。

有关信息，请参阅本文中的[规划完成日期](#planned-completion-date)部分。

## 到期于

项目应完成的日期。 项目的到期日期与项目的计划完成日期相同。

项目截止日期显示在项目列表和报告中。

有关信息，请参阅本文中的[规划完成日期](#planned-completion-date)部分。

## [!UICONTROL 输入日期]

[!UICONTROL 进入日期]是在[!DNL Workfront]中创建项目、任务或问题的日期。

[!UICONTROL 进入日期]不会影响项目、任务或问题的时间线，但它对于跟踪和报告很重要。 创建对象时，[!DNL Workfront]会自动生成[!UICONTROL 输入日期]，您无法手动编辑它。

![任务详细信息中的输入日期](assets/entry-date-in-task-details-highlighted-nwe.png)

## 估计到期日期

任务和项目的预计到期日显示项目或任务应完成的更实际日期。

预计日期更符合项目和任务的实际，因为它们考虑了影响项目或任务实际完成的情况。 预计到期日期与预计完成日期相似。

有关详细信息，请参阅[预计日期和预计日期概述](/help/quicksilver/manage-work/tasks/task-information/differentiate-projected-estimated-dates.md)。

项目和任务的预计到期日显示在项目、任务列表和报表中。

## 估计开始日期

任务和项目的预计开始日期显示项目或任务可以开始的更实际日期。

预计日期更符合项目和任务的实际，因为它们考虑到了影响项目或任务实际开始的原因。 预计起始日期与预计起始日期相似。

有关详细信息，请参阅[预计日期和预计日期概述](/help/quicksilver/manage-work/tasks/task-information/differentiate-projected-estimated-dates.md)。

项目和任务的预计开始日期会显示在项目、任务列表和报表中。

<!--## Exchange Rate Date-->

## 固定结束日期

完成业务案例时，项目请求者或所有者标识项目的“固定结束日期”。 这是他们建议项目必须完成的日期。

这是手动估算，未考虑项目任务的任何实际进度。

项目的固定结束日期显示在项目的业务案例部分，以及项目列表和报告中。

![固定结束日期](assets/fixed-end-date-business-case-highlight.png)

## 固定开始日期

完成业务案例时，项目请求者或所有者标识项目的“固定开始日期”。 这是他们建议项目应该开始的日期。

这是手动估算，未考虑项目任务的任何实际进度。

项目的固定开始日期显示在项目的业务案例部分，以及项目列表和报表中。

![固定开始日期](assets/fixed-start-date-business-case-highlight.png)

## 工作交接日期

任务可供工作的日期。 这意味着所有约束、批准和依赖项都已完成，用户可以开始处理该任务。

移交日期是计算日期，不能手动设置。

有关移交日期的详细信息，请参阅[任务移交日期概述](/help/quicksilver/manage-work/tasks/task-information/handoff-task-date.md)。

任务的移交日期显示在任务列表和报告中。

## 上一个财务更新日期

更新项目的任何财务信息的日期。 这包括更新项目“财务”部分或“业务案例”部分中的财务字段。

上次财务更新日期在项目列表和报告中可见。

## 上次更新日期

上次更新项目、任务或问题的日期。 更新被视为触发要保存的项目、任务或问题的任何更改。 这包括状态、条件、时间线、财务或任何其他字段的更改。

上次更新日期在项目、任务、问题列表和报告中可见。

## [!UICONTROL 小时输入日期]

当您为项目、任务和问题记录时间以指示您在项目、任务或问题上花费的实际时间（以小时为单位）时，记录的时间将成为项目、任务或问题的[!UICONTROL 实际小时数]。

您记录时间的日期是小时条目上的[!UICONTROL 小时条目日期]字段。

小时输入日期显示在小时列表和报告中。

>[!TIP]
>
>一小时的[!UICONTROL 输入日期]不同于另一个Workfront对象的[!UICONTROL 输入日期]，因为它不是创建小时日志的日期，而是您希望小时与其关联的日期。
>
>例如，您可以在9月5日记录任务的小时数，并将小时数与9月1日关联。 该小时的输入日期为9月1日。

有关如何在Workfront中记录时间的信息，请参阅[记录时间](../../../timesheets/create-and-manage-timesheets/log-time.md)。

>[!TIP]
>
>我们建议将登录时间用于工作任务和问题，而不是父级任务或项目。 工作任务记录的时间将累计到父任务和项目，作为父任务和项目的[!UICONTROL 实际小时数]。 已登录问题的时间将作为[!UICONTROL 项目实际小时数]汇总到项目中。

## [!UICONTROL 计划完成日期]

[!UICONTROL 计划完成日期]或[!UICONTROL 到期日期]是计划完成项目、任务或问题的日期。

根据[!UICONTROL 任务限制]，您可能无法编辑任务的[!UICONTROL 规划完成日期]。 根据项目的[!UICONTROL 计划模式]，您可能无法编辑项目的[!UICONTROL 计划完成日期]。

[!UICONTROL 计划完成日期]在[!DNL Workfront]的某些区域显示为到期日期。

有关更多信息，请参阅以下文章：

* [任务[!UICONTROL 计划完成日期]的概述](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [设置项目[!UICONTROL 计划完成日期]](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [问题[!UICONTROL 计划完成日期]的概述](../../../manage-work/issues/issue-information/issue-planned-completion-date.md)

标头![&#128279;](assets/project-header-planned-completion-date-highlighted-nwe-350x34.png)中的计划竞争日期

![任务列表中的计划完成日期](assets/planned-completion-date-in-task-list-highlighted-nwe-350x183.png)


## 计划的日期对齐

这是一个自动指示器，表示Workfront分配了项目、任务和问题，以显示相对于其计划完成日期何时完成项目。

计划日期对齐指示器的可能值如下：

* 将在计划的完成日期完成
* 将在计划的完成日期前完成
* 将在计划的完成日期后完成

计划日期对齐在项目、任务、问题列表和报告中可见。

## [!UICONTROL 计划开始日期]

[!UICONTROL 计划开始日期]是项目、任务或问题的计划开始日期。

根据[!UICONTROL 任务限制]，您可能无法编辑任务的[!UICONTROL 计划开始日期]。 根据项目的[!UICONTROL 计划模式]，您可能无法编辑项目的[!UICONTROL 计划开始日期]。

有关详细信息，请参阅项目[!UICONTROL 计划开始日期][&#128279;](../../../manage-work/projects/planning-a-project/project-planned-start-date.md)的概述。

编辑任务的![计划开始日期](assets/planned-start-date-on-edit-task-highlighted-nwe.png)

任务列表中的![计划开始日期](assets/planned-start-date-in-task-list-highlighted-nwe-350x167.png)

## [!UICONTROL 预计完成日期]

[!UICONTROL 预计完成日期]是一个实时计算的指示器，指示项目、任务或问题的完成时间。 将项目、任务或问题标记为完成时，[!UICONTROL 预计完成日期]将更改为[!UICONTROL 实际完成日期]的日期。

如果一切顺利，并按计划进行，[!UICONTROL 预计完成日期]应与[!UICONTROL 计划完成日期]匹配。 否则，由于前置任务延迟，[!UICONTROL 预计完成日期]可能与[!UICONTROL 计划完成日期]不同。

有关详细信息，请参阅项目、任务和问题的[预计完成日期[!UICONTROL 的概述]](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)。

![预计完成日期](assets/projected-completion-date-in-task-details-highlighted-nwe-350x187.png)

## [!UICONTROL 预计开始日期]

[!UICONTROL 预计开始日期]是项目、任务或问题开始的实时日期，该日期会考虑所有延迟。 此项目、任务或问题的开始日期比[!UICONTROL 计划开始日期]更准确。 [!UICONTROL 计划开始日期]不考虑延迟或过去的日期。

当您首次计划项目时，任务和项目的[!UICONTROL 计划开始日期]和[!UICONTROL 预计开始日期]相同。 由于可能会出现延迟或任务可能提前完成，[!UICONTROL 预计开始日期]可能与[!UICONTROL 计划开始日期]不同。

对于任务，当其前置任务之一在计划之后运行时，[!UICONTROL 预计开始日期]可能也不同于其[!UICONTROL 计划开始日期]。

>[!TIP]
>
>您只能在列表或报告中查看问题的[!UICONTROL 预计开始日期]。

有关详细信息，请参阅[项目概述[!UICONTROL 预计开始日期]](../../../manage-work/projects/planning-a-project/project-projected-start-date.md)。

![预计开始日期](assets/projected-start-date-in-task-details-highlighted-nwe-350x188.png)

<!--## Rejection Date-->

## 延期日期

任务有时可以延迟开始和完成，而不会影响项目的完成日期。

Slack日期显示任务肯定会影响项目完成日期的确切日期。

有关任务的Slack日期的信息，请参阅[任务Slack日期概述](/help/quicksilver/manage-work/tasks/task-information/task-slack-date.md)。

任务Slack日期在任务列表和报告中可见。

## 开始于

计划项目开始的日期。 项目的开始日期与项目的计划开始日期相同。

此字段在项目列表和报告中可见。

有关信息，请参阅本文中的[计划开始日期](#planned-start-date)部分。



