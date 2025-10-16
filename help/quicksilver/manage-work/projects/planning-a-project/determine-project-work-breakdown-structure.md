---
product-area: projects
navigation-topic: plan-a-project
title: 确定项目中的工作分解结构
description: 为项目定义工作分解结构(WBS)是一组最终概述项目计划的活动。 WBS将项目的结果划分为可管理的工作元素，这些工作元素可用于定义里程碑和组织工作分派。
author: Alina
feature: Work Management
exl-id: a76c468d-6373-4dab-93ff-a0b3734f368c
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '1750'
ht-degree: 1%

---

# 确定项目中的工作分解结构

为项目定义工作分解结构(WBS)是一组最终概述项目计划的活动。 WBS将项目的结果划分为可管理的工作元素，这些工作元素可用于定义里程碑和组织工作分派。

您必须拥有对项目具有编辑访问权限的计划许可证才能构建项目的工作细分结构。 根据构建WBS时执行的活动数量，可能需要额外访问Adobe Workfront的其他区域。

我们建议您在更改工作细分结构时保持项目处于“计划”状态，以避免向项目团队中的用户触发通知。

## 定义项目交付项

项目的目的是向内部和外部利益攸关方提供切实的交付成果。 项目的交付项是指希望通过完成项目而获得的结果。 结果几乎总是与至少一个交付项关联，并且所有交付项都应与项目关联。

项目交付项可以是消费品、智能输出（如报告）或服务。 例如，如果您的项目范围是构建一个房子，则一些交付项可能包括：

* 创建体系结构计划
* 正在完成管道
* 电气工时
* 正在浇筑基础
* 构架工作
* 关闭了房屋的出售。

根据其大小和范围，一个项目可以由多个交付项组成。

标识交付项后，您就可以开始将其划分为任务。 任务是指为了交付项目的整体结果而获得的输出。 在定义任务时，您会考虑以下参数：

* 完成所需的时间。
* 完成工作所需的预算。
* 完成工作所需的资源。
* 根据任务的逻辑时间线安排资源。

在定义任务时，请确保不要为一个单独的任务计划太多工作。 如果一项任务所需的工作超过40小时（典型的一周工作），则您可能需要在子任务中细分该工作量。 然后，完成所有子任务即可完成主任务。

要在Workfront中定义WBS结果和交付项，我们建议您执行以下活动以创建项目任务的分层视图：

* 如果您尚未这样做，请创建一个新项目。\
  有关创建项目的信息，请参阅文章[创建项目](../../../manage-work/projects/create-projects/create-project.md)。

* 为完成每个结果和交付项所需的所有措施项创建任务。\
  有关创建任务的信息，请参阅文章[在项目中创建任务](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) 。

* 从您刚刚创建的任务中，确定哪些是主要结果，并将它们与里程碑相关联。\
  有关创建里程碑任务的信息，请参阅文章[创建里程碑路径](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md)和[将里程碑与任务关联](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)。

* 将范围过大的任务划分为子任务。 将它们与定义交付项的父项关联。\
  有关创建子任务的信息，请参阅文章[创建子任务](../../../manage-work/tasks/create-tasks/create-subtasks.md)。

* 确定子任务之间和里程碑之间的依赖关系。\
  在依赖关系中，任务的开始取决于另一个任务或一组任务的完成。\
  有关任务依赖性的信息，请参阅文章[任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)和[在任务列表中创建前置任务关系](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md)。

* 确定在项目生命周期的任何时间点，是否需要批准和审查。 创建批准流程以满足此需求。\
  有关审批的信息，请参阅文章[为工作项创建审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

## 估计工作计划和计划约束

创建项目的基本里程碑和任务结构后，您可以通过定义任务限制和持续时间来估计完成整个项目所需的时间。

请考虑以下事项：

* 任务约束定义任务工作必须开始或结束的时间。

  有关定义任务约束的信息，请参阅文章[任务约束概述](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)。

* 任务的持续时间是指完成任务所需的时间范围。 在估计持续时间时，您可能希望输入一个考虑延迟可能性的值。 如果以前完成了类似项目，您可能会知道在何处设置此值。

  由于持续时间是估计值，请务必设置乐观的时间值以考虑可能影响任务的因素，如天气、停电、供应商困难或其他不可预见的事件。 此外，请务必考虑是否存在任何关联的前置任务或依赖项任务，以及它们如何对工作施加限制并影响任务完成。

  根据任务的持续时间类型，您可以在项目生命周期中修改任务的持续时间，但这也会影响项目的时间表。 有关任务持续时间的信息，请参阅文章[任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) 。

## 分配任务

在定义每个任务的持续时间和限制后，您可以确定谁有时间和技能完成工作。 您可以在Workfront中将任务分配给以下实体：

* 用户\
  只有具有“规划者”或“工作人员”访问级别的用户才能分配给任务。 虽然您可以将任务分配给请求者和查看者，但他们无法完成任务。 因此，我们不建议为他们分配任务。

  有关访问级别以及访问级别如何定义用户可以对Workfront对象执行操作的信息，请参阅[访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)。

* 职位角色
* 团队

有关分配任务的信息，请参阅[分配任务](../../../manage-work/tasks/assign-tasks/assign-tasks-1.md)部分中的文章。

## 管理资源

Workfront中的资源管理允许您确定是否有足够的员工完成项目。 将用户添加到项目时，Workfront会显示每个用户的使用情况。 资源经理可以查看在项目时间范围内人员分配给其他项目的总小时数。

>[!NOTE]
>
>只要项目的状态为Planning，分配给用户的任务就不会出现在用户的任务列表中。

在会计年度或季度初时，您可能希望跨多个项目在更高级别管理您的资源，而无需了解特定的工作细分结构。\
有关在更高级别规划资源使用的信息，请参阅文章[资源规划入门](../../../resource-mgmt/resource-planning/get-started-resource-planning.md)。

在建立项目的工作细分结构，并确保每个任务都分配给正确的资源的情况下管理资源时，您已经为需要完成的工作准备好了资源计划。\
有关计划资源的信息，请参阅[工作负载均衡器：文章索引](../../../resource-mgmt/workload-balancer/workload-balancer.md)部分中的文章。

## 估计项目财务

Workfront将计算每个任务的计划成本以及项目的整体成本。 任务的计划成本包括任务的所有费用以及分配给任务的员工或角色的成本。 任务、角色和员工的小时费率在任务、角色和用户创建期间分配。

有关项目财务的信息，请参阅[项目财务：文章索引](../../../manage-work/projects/project-finances/project-finances-overview.md)部分。

## 确定项目的批准点

通过在Workfront中创建批准流程，您可以为项目建立审查点，以监控进展和潜在问题领域。 通过审批流程，项目所有者可以辨别哪些任务延迟和提前，查看列出谁更改了任务状态的审核跟踪，并查看问题历史记录，包括问题解决方式和关闭时间。 在审阅项目时，项目所有者可以确定要执行的步骤并更新项目计划（如有必要）。

有关审批的信息，请参阅文章[为工作项创建审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

## 查看您的WBS

要了解项目的WBS，您需要查看以下任务元素：

* 任务序列和时间线（计划的开始和完成日期以及任务持续时间）
* 前置任务依赖项
* 子关系和父关系
* 任务

完成WBS后，您可以在项目级别的任务列表或报表中查看它。

* [在任务列表中查看WBS](#view-the-wbs-in-a-task-list)
* [在任务报告中查看WBS](#view-the-wbs-in-a-task-report)

### 在任务列表中查看WBS {#view-the-wbs-in-a-task-list}

您可以在项目级别查看任务列表。

1. 转到要查看其工作细分结构的项目。
1. 选择&#x200B;**任务**&#x200B;选项卡。
1. （可选）在&#x200B;**分组**&#x200B;下拉菜单中选择&#x200B;**无**。

   工作分解结构不显示WBS中任务的缩进。

1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**工作划分**&#x200B;视图。

   工作划分结构将显示在选定视图的第二列中。

   ![任务列表中的工作分解结构](assets/work-breakdown-structure.png)

### 在任务报告中查看WBS {#view-the-wbs-in-a-task-report}

通过执行以下操作之一，可以生成任务报告并显示任务的WBS：

* 将现有的工作划分结构视图应用于报表。
* 将工作细分结构列添加到任何自定义报表。

>[!TIP]
>
>我们建议添加一个项目分组，以明确说明任务属于哪些项目。 任务的缩进不显示在任务报告中。

有关生成报表的信息，请参阅文章[创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

## 将项目的WBS另存为模板

如果您处理其他遵循与刚刚创建的WBS类似的工作计划的项目，则可能需要将该项目另存为模板。 在创建未来的相关项目时，模板将节省时间和精力。

如果贵组织的人员调整很少，请考虑等到完成用户分配后再保存模板。 无论项目何时另存为模板，都可以在将模板附加到新项目期间删除用户工作分配或特定任务。

工作分解结构的以下元素可以保存在模板中，以供将来与其他项目一起使用：

* 前置任务依赖项
* 工作（包括项目所有者、发起人和资源管理器）
* 审批流程
* 任务限制
* 文档
* 开支及其他财务资料
* 目标
* 小时类型
* 请求队列结构
* 提醒通知
* 风险
* 记帐费率
* 共享信息
* 自定义表单

有关将项目另存为模板的信息，请参阅文章[从项目创建模板](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md) 。
