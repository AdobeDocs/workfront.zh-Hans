---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 安装Blueprint后要执行的操作
description: 本文概述了在中安装Blueprint后，您应该执行的操作 [!DNL Adobe Workfront] 将Blueprint完全部署到系统用户。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# 安装Blueprint后要执行的操作

本文概述了在中安装Blueprint后，您应该执行的操作 [!DNL Adobe Workfront] 将Blueprint完全部署到系统用户。

* [项目模板建议](#project-template-recommendations)
* [组织结构建议](#organizational-structure-recommendations)
* [功能板推荐](#dashboard-recommendations)

## 项目模板建议 {#project-template-recommendations}

本节包含有关随Blueprint一起安装的项目模板的建议。

### 将用户分配给新创建的角色和团队 {#assign-users-to-newly-created-roles-and-teams}

在Blueprint安装过程中创建的角色和/或团队不会自动将用户与其关联。 如果不将用户分配给新添加的角色或团队，您将为无人承担的功能创建工作。 在某些情况下，您可能需要创建新用户以填充这些角色和团队。 有关创建新用户的信息，请参阅 [添加用户](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### 将自定义表单应用到模板和模板任务 {#apply-a-custom-form-to-the-template-and-the-template-tasks}

安装过程不会将项目模板与任何自定义表单相关联。 如果您的项目或任务需要填充特定的表单或字段以创建报表一致性，或者如果您的数字请求表单包含需要在项目级别保留的字段，我们建议您将模板或模板任务与这些表单相关联。 有关信息，请参阅 [将自定义表单添加到对象](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### 更新模板任务持续时间和工作估计 {#update-template-task-duration-and-effort-estimates}

模板中的每个任务都包含计划的持续时间和计划的工作量估计。 这些估计值用作这些活动持续时间和逗留时间的起点。 但是，贵组织的能力、技能和步伐是独一无二的。 您应查看每项任务的预计持续时间和工作量，以调整它以反映贵组织的需求。 有关信息，请参阅 [在 [!UICONTROL 任务详细信息概述] 面积](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### 关联里程碑路径和里程碑 {#associate-a-milestone-path-and-milestones}

安装过程不会将项目模板与里程碑路径相关联。 将里程碑路径应用到模板，并将里程碑应用到模板中的关键任务，以支持您的里程碑报告需求。 有关信息，请参阅 [将里程碑与任务关联](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### 将模板转出给您的团队 {#roll-out-the-template-to-your-team}

为将使用此模板的工作经理和将在项目模板中执行工作的各个参与者准备培训材料。

### 创建或更新报表和功能板 {#create-or-update-reports-and-dashboards}

如果解决方案代表一种贵组织以前未在 [!DNL Workfront]，则您可能需要创建新报表和功能板以支持工作。 有关信息，请参阅 [创建自定义报表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) 和 [创建功能板](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

如果解决方案与您已在中执行的工作类似 [!DNL Workfront]，则您应该验证工作信息源是否按预期发送到现有报表和功能板。 如果它没有馈送到您的现有报表中，请采取操作来更新过滤器或创建新报表。

## 组织结构建议 {#organizational-structure-recommendations}

本节包含有关随Blueprint一起安装的组织结构元素的建议。

### 公司

安装包含公司的蓝图后：

* 添加自定义表单，以使用有用的详细信息（表单及其详细信息对您而言是唯一的）来扩充公司记录。 有关信息，请参阅 [将自定义表单添加到对象](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* 如果公司代表客户，请查看与公司关联的覆盖率。 有关信息，请参阅 [在公司层改写职务职责开单费率](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* 如果公司代表客户，并且存在其他特定于该组织的项目模板，请首先将项目模板与新添加的公司预关联。 有关信息，请参阅 [编辑项目模板](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* 如果公司代表客户或供应商，请关联外部组织中可能已位于您环境中的现有用户。 有关信息，请参阅 [创建和编辑公司](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* 如果公司代表客户或供应商，请为外部组织创建其他协作者用户，您可能需要这些用户来在环境中简化通信、工作执行和批准。 有关创建新用户的信息，请参阅 [添加用户](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* 为当前与新添加的公司关联的任何用户更新组织图关系。 有关信息，请参阅 [创建直接报表](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) 和 [查看组织图](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

有关公司的其他信息，请参阅 [创建和编辑公司](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## 功能板推荐 {#dashboard-recommendations}

此部分包含与Blueprint一起安装的功能板和报表的建议。

### 更新新创建的功能板以添加/删除报表

从Blueprint添加的功能板具有一个或多个报表、外部页面或日历。 您可能不需要所有报表和其他功能板元素，或者需要先使用现有报表、外部页面和日历来扩充功能板，然后才能与他人员共享。 有关信息，请参阅 [将报表添加到功能板](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### 更新新创建的报表以添加/删除列或筛选条件

通过功能板Blueprint分发的报表并没有支持您配置的所有列或筛选条件 [!DNL Workfront]. 预计您会对报表进行一些调整，以符合您的标准。 为了与环境中的其他报表保持一致，您可能需要为所列对象的所有报表添加一个包含的列，或添加一些筛选条件，以将结果限制到特定项目类型或用户组。 有关信息，请参阅 [创建或编辑视图](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) 和 [创建或编辑过滤器](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### 与用户共享功能板或报表

如果您不打算将功能板放置在布局模板上，则应该将功能板与那些发现该功能板有用的人员共享。 有关信息，请参阅 [共享功能板](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) 和 [共享报表](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### 将功能板添加到布局模板

向其他人提供信息的最佳方式是向布局模板添加功能板。 确定定期查看功能板从中受益最多的人员的布局模板，并将新创建的功能板添加到这些布局模板中。 有关信息，请参阅 [创建和管理布局模板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### 更新其他功能板和报表

新功能板及其报表的引入，可能会使其报废并调整其他现有功能板和报表。 请花时间查看现有报告，以确定任何冗余且相互矛盾的报告。

### 将自定义数据分发到相关表单

功能板Blueprint中包含的某些报表在报表的查看、过滤或分组中具有自定义数据字段。 在某些情况下，Blueprint还将具有与这些字段关联的表单。 但是，自定义字段通常不会应用于自定义表单。 为了使列、过滤器或分组正常工作，这些字段必须与连接到用户、项目、任务或其他对象记录的表单相关联。 有关信息，请参阅 [将自定义字段添加到自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
