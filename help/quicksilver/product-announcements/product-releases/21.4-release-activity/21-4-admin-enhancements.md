---
title: 21.4管理员增强功能
description: 21.4管理员增强功能
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: fc85b4c2-4a76-4226-9120-11635b03aa4e
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '1891'
ht-degree: 0%

---

# 21.4管理员增强功能

本页介绍了在21.4版本中对“预览”环境所做的所有“管理员”增强。 这些增强功能将在2021年10月4日当周的生产环境中提供。

有关21.4版本可用的所有更改列表，请参阅 [21.4版本概述](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## 对于管理员：查看哪些组与审批流程关联

为了帮助您找出哪些组与系统中的审批流程相关联，我们已在“设置”的“审批”页面的“标准”视图中添加了“组名称”列。 现在，您无需创建自定义视图即可查看此信息。

有关批准流程的信息，请参阅 [审批流程概述](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

有关管理组审批流程的信息，请参阅 [组级别审批流程](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## 管理员的新增功能：组可以配置自己的时间表和小时首选项

>[!NOTE]
>
>最初，在生产环境中，此功能将作为分阶段推出的一部分提供，仅适用于群集4上的客户。 当功能对其他群集可用时，将更新此注释。

在大型组织中，某些组可能需要单独配置时间表和小时首选项以适合其独特的工作流，而不是继承由系统级别管理员配置的首选项。 现在，Workfront管理员可以解锁系统中所有组的时间表和小时首选项，以便他们能够自行配置。

最近还增加了用于项目首选项以及任务和问题首选项的功能。

有关Workfront管理员如何解锁时间表和小时首选项的信息，请参阅部分 [解锁组的工时表和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) 在文章中 [配置时间表和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

有关组管理员如何为组配置解锁的任务和问题首选项的信息，请参见 [配置组的工时表与小时首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Workfront管理员的新增功能：在新的Workfront Experience中为自动配置的用户配置布局模板

现在，您可以在新的Workfront Experience中为自动配置用户配置布局模板。 在用于映射用户属性的Workfront“用户属性”下拉菜单（“设置”>“系统”>“单点登录”）中，现在有新的“新布局模板”菜单项可用于进行此配置。 以前，您只能在Workfront Classic中为自动配置用户配置布局模板。

有关映射用户属性的说明，请参阅 [映射用户属性并自动配置新用户](../../../administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md).

## 新字段显示您的用户所属的组

现在，可以轻松确定您的用户属于哪些组。 在列出用户的报表或视图中，可以使用新的“其他组”字段创建列。 此字段列出每个用户所属的组。

有关使用报告和视图的信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) 和 [Adobe Workfront中的视图概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Blueprint详细信息页面现在显示图像

现在，每个Blueprint的详细信息页面会显示与Blueprint一起安装的项目模板的图像。 图像提供了Blueprint内容的预览，以便您了解将要安装的内容。 您可以选择在浏览器中预览完整图像或下载图像。

有关更多信息，请参阅 [Blueprint概述](../../../administration-and-setup/blueprints/blueprints-overview.md).

![](assets/blueprint-detailspage.png)

## 新问题的Blueprint偏好设置

现在为某些Blueprint提供了新的问题偏好设置。 它们默认安装，但在配置安装详细信息时，可以选择退出安装首选项。

首选项包括队列主题组、队列主题和路由选择规则，用于在提交问题或请求时收集正确的信息，并将问题或请求发送到正确的工作角色或团队。 使用首选项有助于在项目中捕获新问题或请求的方式创建一致性。

请注意，使用这些首选项不会将从模板创建的项目加入请求队列。

有关更多信息，请参阅 [配置Blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## 组管理员的新增功能：查看和管理组最近删除和还原的项目

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用。

我们将继续让您更轻松地在一个位置管理您的组及其关联的对象。 现在，您可以从“组”区域查看和使用组最近删除和还原的项目。 这样，您就不必转至“设置”中的“最近删除”或“最近恢复”区域来管理这些项目。 它会将您正在处理的组项目列表与系统中其他已删除和还原的项目分开。

有关更多信息，请参阅 [查看和管理组最近删除的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) 和 [查看和管理组最近恢复的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).

## 组管理员的新增功能：组首选项现在会影响组模板

现在，可以更轻松地确保您组的项目模板满足您组的需求。 在创建新项目模板时将其分配给组时，该模板会从组的项目和任务首选项中继承以下设置：

* 绩效指数方法
* 完成情况类型
* 时间表开始日期
* 用户空闲时间
* 更新类型
* 访问部分设置

在与组相关联的项目模板中创建新模板任务时，模板任务会继承组任务首选项中的以下设置：

* 持续时间类型
* 收入类型
* 成本类型

以前，项目模板和项目模板任务从系统级别设置的项目和任务首选项继承这些设置。

如果创建没有组的模板或模板任务（例如，从主“模板”页面），则上述设置继承自系统级别的项目和任务首选项。 但是，如果您稍后将组分配给模板或模板任务，则该组的首选项不会影响它。

有关更多信息，请参阅文章中的首选项如何应用于模板和模板任务部分 [创建和修改组的项目模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## 管理员的新增功能：了解哪些自定义表单正在使用自定义字段

现在，更改自定义表单中的自定义字段变得更轻松。 只需在自定义表单中单击，即可了解同时使用该字段的任何其他自定义表单。 请务必评估这些表单是否需要调整，以便在您做出更改后继续正常工作。

有关更多信息，请参阅 [查看使用特定自定义字段或小部件的所有自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md).

## 组管理员的新增功能：锁定和解锁组的项目、任务和问题偏好设置

现在，您可以确保组下的子组中的每个人都使用相同的首选项设置，也可以允许他们为其独特的工作流配置首选项设置。

* Workfront管理员在系统级别解锁首选项后，您可以为组下的所有子组配置并锁定它。 尽管您仍然可以重新配置锁定的首选项，但较低子组的管理员无法为其组执行此操作。

  反过来，您可以解锁组的首选项。 这允许子组管理员根据用户独特的项目、任务或问题工作流需求对其进行配置。

  有关更多信息，请参阅 [锁定或解锁子组的项目、任务或问题偏好设置](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

* 如果您是Workfront管理员，则无需转至“组”区域来配置子组的首选项。 从主项目偏好设置、任务和问题偏好设置或时间表和小时偏好设置区域，您可以使用页面顶部的搜索框查找子组并配置其偏好设置。

  有关更多信息，请参阅 [配置组的项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 和 [配置组的任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## 组管理员的新增功能：从组区域创建和编辑模板

>[!NOTE]
>
>此功能仅在新的Workfront Experience中可用。

我们将继续让您更轻松地在一个位置管理您的组及其关联的对象。 现在，您可以从“设置”的“组”区域查看和使用组的模板。 这样，您就不必转至“模板”区域来管理组的模板。 而且它将您正在处理的组模板列表与整个系统中的其他组模板列表分开。

有关更多信息，请参阅 [创建和修改组的项目模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## 一次在一个附加的自定义表单中输入并保存信息

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用。

现在，在对象的“详细信息”部分提供信息更加容易：在单个自定义字段或可展开区域（例如“概述”和“财务”）中键入并保存信息，即使对象上的其他自定义表单中的必填字段尚未填写。

以前，当您在一个自定义表单或对象的可扩展区域中输入信息时，附加到对象的所有自定义表单都将进入编辑模式，并且必须先完成其所有必填字段，然后才能保存更改。 如果由于必填字段是提供给其他用户而无法完成，则会出现问题。

如果您确实想要编辑对象的“详细信息”部分中的所有自定义表单和可展开区域，可以在我们添加到“编辑”图标的新“编辑”菜单中单击全部编辑。 或者，在同一菜单上，您可以单击名称以滚动到要进行更改的自定义表单或部分

>[!NOTE]
>
>此功能最初发布到21.3版的“预览”中。

为了更便于组织的所有级别独立管理和控制其工作流，我们引入了为子组创建和管理状态的功能。 现在，从“设置”中的“组”部分，您可以为在任何级别上管理的组执行以下操作：

* 创建、编辑、删除和隐藏组的状态
* 锁定任何组的状态，以便其下的所有较低子组可以相同方式使用它
* 解锁任何组的状态，以便较低子组的管理员可以对其进行自定义以满足其独特需求
* 将组状态设置为默认状态
* 重新排序和隐藏对象上组状态的显示

Workfront管理员还可以执行以下操作（针对所有组）。

以前，此功能仅适用于顶级组。

有关更多信息，请参阅 [管理组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md).

## Workfront管理员的新增功能：自行将布局模板从Workfront Classic迁移到新的Workfront Experience

>[!NOTE]
>
>此功能于2021年7月1日发布到“预览”环境。 该版本将于2021年7月15日发布到生产环境。

为了帮助您在用户转为使用新的Workfront Experience时管理布局模板，我们创建了一个按钮，您可以使用它将Workfront Classic中的布局模板迁移到新Experience，而无需依赖Workfront客户支持。

以前，只有Workfront客户支持可以将布局模板从Workfront Classic迁移到新的Workfront Experience。

## 将模板与组关联时，在队列详细信息和队列主题中选择组审批流程

我们在将模板与组关联的过程中添加了一个新选项。 现在，您可以在模板的“队列详细信息”或其中一个队列主题中，为问题选择特定于组的批准流程。

在21.3中，当我们添加了将组模板与组关联的功能时，您可以在模板中选择特定于组的批准流程，但无法在模板的“队列详细信息”或“队列主题”中选择该流程。

有关更多信息，请参阅 [将新的或现有的审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
