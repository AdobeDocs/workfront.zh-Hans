---
product-area: templates
navigation-topic: templates-navigation-topic
title: 项目模板概述
description: 您可以使用项目模板捕获与组织中项目关联的大多数可重复流程、信息和设置。
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
source-git-commit: ca4da5302198d8fffc8b706baa3b3aeaa1f738e3
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 1%

---

# 项目模板概述

<!-- Audited: 12/2023 -->

您可以使用项目模板捕获与组织中项目关联的大多数可重复流程、信息和设置。

您可以在模板中定义任务、队列主题、自定义表单和附加文档。

创建模板后，您可以将其附加到现有项目，或者使用它们构建新项目。 模板上的所有信息将传输到使用它创建的项目。

## 在Adobe Workfront中使用模板的好处

以下是使用模板创建项目的一些好处：

* 在创建重复的新项目时，它可以节省您的时间和精力。
* 您在范围相似的项目间具有一致的信息。
* 在报告项目时，此插件非常有用。 例如，您可以报告共享同一模板的项目，比较其进度并发现改进完成方式的方法。
* 除了定义未来的项目设置外，您还可以为模板上的未来项目添加以下信息：

   * 任务
   * 文档
   * 审批
   * 队列详细信息
   * 队列主题
   * 主题组
   * 路由规则
   * 自定义Forms
   * 公司和组信息

## 创建模板的最佳实践

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

创建模板时，请考虑以下事项：

* 不要将用户分配给模板任务。 虽然您可以保留未分配任务，但我们建议您为任务分配工作角色。 这将让您了解在使用模板创建项目时，可以为任务分配哪些用户。
* 始终为模板任务指定持续时间和已计划小时数值。 项目中的每个任务都应与任务可以保持打开状态的持续时间相关联，并与计划小时值相关联，以说明任务实际完成所需的时间。 在Workfront中使用资源管理工具时，无法正确为没有此信息的任务预算资源。

  有关持续时间的信息，请参阅以下文章：

   * [任务工期和工期类型概览](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [项目持续时间概述](../../../manage-work/projects/planning-a-project/project-duration.md)

  有关计划小时数的信息，请参阅 [计划小时数概述](../../../manage-work/tasks/task-information/planned-hours.md).

* 在任务的最后，当您对未来的项目计划有一个明确的了解时，添加前置任务关系。 将前置任务添加到模板任务与将前置任务添加到项目中的任务类似。

  有关向任务添加前置任务的信息，请参阅 [前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* 指示模板应当与谁共享以供将来使用，以及应当与谁共享将从模板创建的项目。 有关共享模板的信息，请参阅 [共享项目模板](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* 使用全局审批流程，并在可能的情况下将其添加到模板和模板任务。 在任务或未来项目需要经过相同的审批时，这将节省时间。

  有关创建批准的信息，请参阅 [创建工作项的审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  有关将审批流程与工作项关联的信息，请参阅 [将新的或现有的审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 创建模板的方法

您可以通过以下方式创建新模板：

* 从头开始。\
  有关从头开始创建新模板的详细信息，请参阅 [创建项目模板](../../../manage-work/projects/create-and-manage-templates/create-template.md).

* 从现有项目中，通过将项目另存为模板。\
  有关从现有项目创建模板的详细信息，请参阅 [从项目创建模板](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md).

* 通过从另一个模板复制它。\
  有关复制现有模板的详细信息，请参阅 [复制项目模板](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* 使用我们的示例模板。\
  有关使用我们的示例模板构建模板的更多信息，请参阅 [根据示例创建项目模板](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md).
