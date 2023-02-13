---
title: 21.4管理员增强功能
description: 21.4管理员增强功能
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: fc85b4c2-4a76-4226-9120-11635b03aa4e
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1882'
ht-degree: 0%

---

# 21.4管理员增强功能

本页介绍在“预览”环境的21.4版本中对管理员所做的所有增强。 这些增强功能将于2021年10月4日这一周的生产环境中提供。

有关21.4版本中可用的所有更改的列表，请参阅 [21.4版本概述](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## 对于管理员：查看哪些组与批准流程关联

为了帮助您找出哪些组与系统中的审批流程相关联，我们在“设置”的“审批”页面的“标准”视图中添加了“组名称”列。 现在，您无需创建自定义视图即可查看此信息。

有关审批流程的信息，请参阅 [审批流程概述](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

有关管理组审批流程的信息，请参阅 [组级别的审批流程](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## 管理员的新增功能：组可以配置自己的时间表和小时首选项

>[!NOTE]
>
>最初，在生产环境中，此功能将作为分阶段推出的一部分提供，仅供群集4上的客户使用。 此注释将随着其他群集可以使用该功能而更新。

在大型组织中，某些组可能需要独立配置工时单和小时首选项以适合其独特工作流，而不是继承由系统级别的管理员配置的首选项。 现在，Workfront管理员可以解锁系统中所有组的工时单和小时首选项，以便他们可以自行配置。

最近还为项目首选项以及任务和问题首选项添加了此功能。

有关Workfront管理员如何解锁工时单和小时首选项的信息，请参阅部分 [解锁组的工时单和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) 在文章中 [配置工时单和工时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

有关组管理员如何配置已解锁任务和发布组首选项的信息，请参阅 [为组配置工时单和小时首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Workfront管理员的新增功能：在新的Workfront体验中为自动配置的用户配置布局模板

现在，您可以在新的Workfront体验中为自动配置的用户配置布局模板。 在映射用户属性（设置>系统>单点登录）的Workfront“用户属性”下拉菜单中，现在有一个新的“新布局模板”菜单项可用于进行此配置。 以前，您只能在Workfront Classic中为自动配置用户配置布局模板。

有关映射用户属性的说明，请参阅 [映射用户属性并自动配置新用户](../../../administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md).

## 新字段显示用户所属的组

现在，您可以轻松找到用户所属的组。 在列出用户的报表或视图中，您可以使用新的“其他群组”字段创建列。 此字段列出每个用户是其成员的组。

有关使用报表和视图的信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) 和 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Blueprint详细信息页面现在显示一个图像

现在，每个Blueprint的详细信息页面会显示随Blueprint一起安装的项目模板的图像。 该图像提供了Blueprint内容的预览，以便您了解要安装的内容。 您可以选择在浏览器中预览完整图像或下载图像。

有关更多信息，请参阅 [Blueprint概述](../../../administration-and-setup/blueprints/blueprints-overview.md).

![](assets/blueprint-detailspage.png)

## 新问题的Blueprint首选项

一些Blueprint现在提供了新的问题首选项。 默认情况下会安装这些首选项，但在配置安装详细信息时，您可以选择退出安装这些首选项。

首选项包括队列主题组、队列主题和路由规则，用于在提交问题或请求时收集正确的信息，并将问题或请求发送到正确的作业角色或团队。 使用首选项有助于创建在项目中捕获新问题或请求的一致性。

请注意，使用这些首选项不会将从模板创建的项目放入请求队列。

有关更多信息，请参阅 [配置Blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## 群组管理员的新增功能：查看并管理组最近删除和还原的项目

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用。

我们将继续在一个位置更轻松地管理您的组及其关联对象。 现在，您可以从“组”区域查看和处理组最近删除和还原的项目。 这样，您就无需转到“设置”中的“最近删除”或“最近还原”区域来管理这些项目。 它将您正在处理的组项目列表与系统中其他已删除和还原的项目分开。

有关更多信息，请参阅 [查看并管理群组最近删除的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) 和 [查看和管理组最近还原的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).

## 群组管理员的新增功能：组首选项现在会影响组模板

现在，更容易确保组的项目模板满足组的需求。 在创建新项目模板时，如果将新项目模板分配给某个组，则该模板会从该组的项目和任务首选项继承以下设置：

* 绩效指数方法
* 完成情况类型
* 计划自
* 用户关机时间
* 更新类型
* 访问部分设置

在与组关联的项目模板中创建新模板任务时，模板任务会从组的任务首选项继承以下设置：

* 持续时间类型
* 收入类型
* 成本类型

以前，项目模板和项目模板任务会从系统级别设置的项目和任务首选项中继承这些设置。

如果创建模板或模板任务时没有组（例如，从“模板”主页），则以上设置将从系统级别的项目和任务首选项继承。 但是，如果稍后为模板或模板任务分配组，则组的首选项不会影响该任务。

有关更多信息，请参阅文章中的首选项如何应用于模板和模板任务一节 [创建和修改组的项目模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## 管理员的新增功能：了解使用自定义字段的自定义表单

现在，在自定义表单中更改自定义字段更为容易。 在自定义表单中单击一次，即可了解还使用字段的任何其他自定义表单。 评估这些表单是否需要调整，以便在您进行更改后能够正常工作，这一点很重要。

有关更多信息，请参阅 [查看使用特定自定义字段或小组件的所有自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md).

## 群组管理员的新增功能：锁定和解锁组的项目、任务和问题首选项

现在，您可以确保群组下子群组中的每个人都使用相同的首选项设置，或者允许他们为其唯一的工作流配置首选项设置。

* 在Workfront管理员解锁系统级别的首选项后，您可以配置并锁定组下所有子组的首选项。 虽然您仍可以重新配置锁定的首选项，但下级子组的管理员无法为其组重新配置锁定首选项。

   相反，您可以解锁组的首选项。 这允许子组管理员根据其用户的独特项目、任务或问题工作流需求对其进行配置。

   有关更多信息，请参阅 [锁定或解锁子组的项目、任务或问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

* 如果您是Workfront管理员，则无需转到“组”区域来配置子组的首选项。 在主项目首选项、任务和问题首选项或工时单和小时首选项区域中，可以使用页面顶部的搜索框查找子组并配置其首选项。

   有关更多信息，请参阅 [为组配置项目首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 和 [为组配置任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## 群组管理员的新增功能：从“组”区域创建和编辑模板

>[!NOTE]
>
>此功能仅在新的Workfront体验中可用。

我们继续在一个位置更轻松地管理您的组及其关联对象。 现在，您可以从“设置”的“组”区域查看和使用组的模板。 这样，您就无需转到“模板”区域来管理组的模板。 它将您正在处理的组模板列表与整个系统中其他模板分开。

有关更多信息，请参阅 [创建和修改组的项目模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## 一次在一个附加的自定义表单中输入并保存信息

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用。

现在更容易在对象的“详细信息”部分提供信息：在单个自定义字段或可扩展区域（如“概述”和“财务”）中键入并保存信息，即使对象上其他自定义表单的必填字段尚未填写也是如此。

以前，当您在一个自定义表单或对象的可扩展区域中输入信息时，附加到该对象的所有自定义表单都将进入编辑模式，并且必须填写其所有必填字段，然后才能保存更改。 如果由于必填字段面向其他用户，因此无法完成该字段，则会出现问题。

如果确实要编辑某个对象的“详细信息”部分中的所有自定义表单和可展开区域，则可以在我们添加到“编辑”图标的新“编辑”菜单上单击“全部编辑”。 或者，在同一菜单上，您可以单击名称以滚动到要更改的自定义表单或部分

>[!NOTE]
>
>此功能最初在21.3版本中发布为“预览”。

为了使组织的所有级别都能够更轻松地独立管理和控制其工作流，我们引入了为子组创建和管理状态的功能。 现在，从“设置”的“组”部分中，您可以对任何级别上管理的组执行以下操作：

* 创建、编辑、删除和隐藏群组的状态
* 锁定任何组的状态，以便其下所有较低的子组都能以相同方式使用它
* 解锁任何组的状态，以便下级子组的管理员可以对其进行自定义以满足其独特需求
* 将组状态设置为默认状态
* 对对象上显示的组状态重新排序和隐藏

Workfront管理员还可以执行这些操作（适用于所有组）。

以前，此功能仅适用于顶级组。

有关更多信息，请参阅 [管理组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md).

## Workfront管理员的新增功能：自行将布局模板从Workfront Classic迁移到新的Workfront体验

>[!NOTE]
>
>此功能于2021年7月1日发布到预览环境。 它将于2021年7月15日发布到生产环境。

为了帮助您在用户切换到使用新的Workfront体验时管理布局模板，我们创建了一个按钮，您可以使用该按钮将布局模板从Workfront Classic迁移到新体验，而无需依赖Workfront客户支持。

以前，只有Workfront客户支持可以将您的布局模板从Workfront Classic迁移到新的Workfront体验。

## 在将模板与组关联时，在“队列详细信息”和“队列主题”中选择组批准流程

我们在将模板与群组关联的过程中添加了一个新选项。 现在，您可以为模板的“队列详细信息”或其其中一个“队列主题”中的问题选择特定于组的审批流程。

在21.3中，当我们添加了将组模板与组关联的功能时，您可以在模板中选择特定于组的批准流程，但无法在模板的“队列详细信息”或“队列主题”中选择该流程。

有关更多信息，请参阅 [将新审批流程或现有审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
