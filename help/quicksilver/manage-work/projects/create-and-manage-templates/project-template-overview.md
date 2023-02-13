---
product-area: templates
navigation-topic: templates-navigation-topic
title: 项目模板概述
description: 您可以使用项目模板来捕获与组织中的项目关联的大多数可重复流程、信息和设置。
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 1%

---

# 项目模板概述

您可以使用项目模板来捕获与组织中的项目关联的大多数可重复流程、信息和设置。

您可以定义任务、队列主题、自定义表单、在模板中附加文档。

创建模板后，您可以将它们附加到现有项目，也可以使用它们构建新项目。 有关模板的所有信息都会传输到使用该模板创建的项目。

## 在Adobe Workfront中使用模板的好处

以下是使用模板创建项目的一些好处：

* 在创建重复的新项目时，这样可节省您的时间和精力。
* 您在项目范围中具有一致的信息，这些信息是相似的。
* 在报告项目时，此功能非常有用。 例如，您可以报告共享同一模板的项目，以比较其进度并查找完成方式的改进。
* 除了定义将来的项目设置之外，您还可以在模板上为将来的项目添加以下信息：

   * 任务
   * 文档
   * 审批
   * 队列详细信息
   * 队列主题
   * 主题组
   * 路由规则
   * 自定义Forms
   * 公司和集团信息

## 创建模板的最佳实践

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

创建模板时，请考虑以下事项：

* 不要将用户分配给模板任务。 虽然您可以将任务保留为未分配状态，但我们建议您将作业角色分配给任务。 这样，您就可以在使用模板创建项目时，为用户分配哪些任务。
* 始终为模板任务指定“持续时间”和“计划小时数”值。 项目中的每个任务都应与任务保持打开状态的持续时间相关联，并且与“计划小时”值关联，以了解任务实际完成所花费的时间。 在Workfront中使用资源管理工具时，无法为资源正确编入没有此信息的任务预算。

   有关持续时间的信息，请参阅以下文章：

   * [任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [项目持续时间概述](../../../manage-work/projects/planning-a-project/project-duration.md)

   有关计划时数的信息，请参阅 [计划时数概述](../../../manage-work/tasks/task-information/planned-hours.md).

* 当您对未来项目计划的整个内容有清晰的了解时，请在最后添加任务之间的前置任务关系。 向模板任务添加前置任务与向项目任务添加前置任务类似。

   有关将前置任务添加到任务的信息，请参阅 [任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* 指示应将模板与谁共享以供将来使用，以及应将从模板创建的项目与谁共享。 有关共享模板的信息，请参阅 [共享项目模板](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* 使用全局批准流程，并尽可能将其添加到您的模板和模板任务中。 当任务或未来项目需要完成相同的批准时，这将节省时间。

   有关创建审批的信息，请参阅 [为工作项创建审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   有关将审批流程与工作项关联的信息，请参阅 [将新审批流程或现有审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 模板的创建方法

您可以通过以下方式创建新模板：

* 白手起家。\
   有关从头开始创建新模板的更多信息，请参阅 [创建项目模板](../../../manage-work/projects/create-and-manage-templates/create-template.md).

* 从现有项目，将项目另存为模板。\
   有关从现有项目创建模板的更多信息，请参阅 [从项目创建模板](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md).

* 从其他模板复制模板。\
   有关复制现有模板的更多信息，请参阅 [复制项目模板](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* 使用示例模板。\
   有关使用示例模板构建模板的更多信息，请参阅 [根据示例创建项目模板](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md).
