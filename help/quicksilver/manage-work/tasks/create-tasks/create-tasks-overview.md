---
product-area: projects
navigation-topic: create-tasks
title: 创建任务概述
description: 只有在创建项目后，才可以在项目中创建任务。
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# 创建任务概述

只有在创建项目后，才可以在项目中创建任务。

例如，在创建项目后，您可能需要添加任务并对其进行修改以组织项目计划。 有关创建项目的更多信息，请参阅 [创建项目](../../../manage-work/projects/create-projects/create-project.md). 有关创建任务的信息，请参阅 [在项目中创建任务](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

本文介绍了创建任务时应用的注意事项、限制和默认值。

## 在项目中创建任务的方法

您可以通过以下方式在项目上创建任务：

* 从头开始，如 [在项目中创建任务](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).
* 将任务复制到同一项目或新项目或在同一项目上复制任务，如 [复制和复制任务](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* 将任务从项目移动到另一个项目，如 [移动任务](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## 创建任务时的限制

拥有正确的访问权限和权限后，您便可以在项目中创建任务。 但是，在以下情况下，您可能无法创建任务：

* 您的Adobe Workfront管理员或组管理员必须允许向项目首选项区域中处于“完成”或“无效”状态的项目添加任务。 有关设置项目首选项的信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* 不能向处于“待批准”状态的项目添加任务。

## 项目上允许的最大任务数

一个项目最多可包含5,000项任务。 当您接近限制时、达到限制时以及尝试超出限制时，项目上会显示一条警告消息。

根据实施此限制时项目中的任务数，Workfront实例可能允许在单个项目中执行5,000多项任务。

如果您能够在单个项目中包含5,000多项任务，请注意以下事项：

* 您的Workfront环境的任务限制设置为最大项目中的当前任务数，外加10%的额外任务。

   例如，如果Workfront实例中的项目包含10,000项任务，则整个Workfront实例中每个项目的限制为11,000项任务。

* 较小的项目可提高性能，并最大限度地减少大型项目带来的管理挑战。

## 向项目添加任务时，任务默认值

有两种类型的默认信息，在您创建任务时，Workfront会自动更新它们：

* 系统级别的默认信息

   您的Workfront管理员或组管理员在“项目首选项”的“任务和问题”区域为任务建立系统级别的默认值。 有关任务和问题首选项的信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) 或 [为组配置任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

* 项目级别的默认信息

   本节的其余部分将介绍作为项目经理的项目级别默认值，您可以为添加到项目的所有新任务定义默认值

在向项目添加任务时，根据项目的设置方式，Workfront可能会自动将批准流程或自定义表单附加到该任务。

有关配置项目以默认添加这些任务的信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md) 文章。

在定义要与项目级别添加到项目的任务关联的默认信息时，请考虑以下事项：

* 您必须拥有项目的“管理”权限，才能定义任务批准流程和自定义表单的默认设置。
* 在编辑项目时，所有新任务都会使用批准流程和定义的自定义表单来创建。
* 在使用“编辑任务”框添加任务时，您可以修改这些默认设置，但在内联编辑中添加任务时，不能修改这些默认设置。
* 您可以在模板中为任务定义批准流程和自定义表单。

   * 使用此模板创建项目时，审批流程和自定义表单会自动应用于该项目。
   * 将模板附加到现有项目后，项目将保留原始任务批准流程和自定义表单设置（如果已定义）。 如果未定义这些设置，则模板中的设置将成为项目的设置。
   * 将模板附加到现有项目后，从模板添加到项目的任务将保留模板中拥有的批准流程和自定义表单设置，而不考虑项目中的任务设置。

   有关将模板附加到项目的信息，请参阅 [将模板附加到项目](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* 复制项目时，任务默认设置会转移到新项目。

   有关复制项目的信息，请参阅 [复制项目](../../../manage-work/projects/manage-projects/copy-project.md).

* 将任务从一个项目复制到另一个项目，并且目标项目具有不同的任务默认设置时，复制的任务将保留原始项目中的默认设置，除非在复制过程中清除这些设置。
* 在同一项目上复制任务时，自定义表单和审批流程将转移到复制的任务中。

   有关复制和复制任务的信息，请参阅[ [复制和复制任务](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

* 将任务移动到其他项目时，会保存原始项目中任务的默认任务设置，而不考虑新项目中的任务默认设置。

   有关移动任务的信息，请参阅 [移动任务](../../../manage-work/tasks/manage-tasks/move-tasks.md).
