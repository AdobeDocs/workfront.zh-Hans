---
product-area: projects
navigation-topic: create-tasks
title: 创建任务概述
description: 只有在创建项目后，您才能在项目中创建任务。
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

# 创建任务概述

只有在创建项目后，您才能在项目中创建任务。

例如，在创建项目后，您可能需要添加任务并修改这些任务以组织项目计划。 有关创建项目的详细信息，请参阅[创建项目](../../../manage-work/projects/create-projects/create-project.md)。 有关创建任务的信息，请参阅[在项目中创建任务](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)。

本文介绍了在创建任务时应用的注意事项、限制和默认值。

## 在项目中创建任务的方法

您可以通过以下方式在项目中创建任务：

* 从头开始，如[在项目中创建任务](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)中所述。
* 将任务复制到同一项目或新项目，或者复制同一项目上的任务，如[复制和复制任务](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)中所述。
* 将任务从一个项目移动到另一个项目，如[移动任务](../../../manage-work/tasks/manage-tasks/move-tasks.md)中所述。

## 创建任务的限制

当您拥有正确的访问权限时，您可以在项目上创建任务。 但是，在下列情况下，您可能无法创建任务：

* 您的Adobe Workfront管理员或组管理员必须将任务添加到项目偏好设置区域中处于“完成”或“终止”状态的项目中。 有关设置项目首选项的信息，请参阅[配置系统范围项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。
* 您无法将任务添加到未决批准中的项目。

## 项目允许的最大任务数

一个项目最多可包含5,000个任务。 当您接近限制、已达到限制以及如果您尝试超过限制，项目上会显示警告消息。

根据施加此限制时项目中任务的数量，您的Workfront实例可能会在单个项目中允许5,000多个任务。

如果您能够在单个项目中包含超过5,000个任务，请注意以下事项：

* Workfront环境的任务限制设置为最大项目中当前的任务数量，外加10%。

  例如，如果Workfront实例中的某个项目包含10,000个任务，则您在整个Workfront实例中的每个项目限制为11,000个任务。

* 较小的项目可提高性能并最大程度地减少大型项目带来的管理挑战。

## 将任务添加到项目时的任务默认值

在创建任务时，Workfront会自动更新两种类型的默认信息：

* 系统级默认信息

  您的Workfront管理员或组管理员在“项目首选项”的“任务和问题”区域中为任务建立系统级别的默认值。 有关任务和问题首选项的信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)或[配置组的任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

* 项目级默认信息

  本节的其余部分介绍作为项目经理，您可以为添加到项目的所有新任务定义项目级别的默认值

在将任务添加到项目时，Workfront可能会将批准流程或自定义表单自动附加到该任务，具体取决于项目的设置方式。

有关配置项目以默认添加这些项目的信息，请参阅[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)文章中的“任务”部分。

在项目级别定义要与添加到项目的任务关联的默认信息时，请考虑以下事项：

* 您必须具有项目的管理权限才能定义任务审批流程和自定义表单的默认设置。
* 所有新任务都是使用编辑项目时定义的批准流程和自定义表单创建的。
* 在使用“编辑任务”框添加任务时，可以修改这些默认设置，但在内联编辑中添加任务时则不能修改。
* 您可以为模板中的任务定义审批流程和自定义表单。

   * 从此模板创建项目时，审批流程和自定义表单会自动应用于该项目。
   * 将模板附加到现有项目时，如果定义了原始任务审批流程和自定义表单设置，则项目会保留这些设置。 如果未定义这些设置，则模板中的设置将成为项目的设置。
   * 当模板附加到现有项目时，从模板添加到项目的任务会保留其在模板中的审批流程和自定义表单设置，而不管项目上的任务设置。

  有关将模板附加到项目的信息，请参阅[将模板附加到项目](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)。

* 复制项目时，任务默认设置将转移到新项目。

  有关复制项目的信息，请参阅[复制项目](../../../manage-work/projects/manage-projects/copy-project.md)。

* 当您将任务从一个项目复制到另一个项目，并且目标项目的任务具有不同的默认设置时，复制的任务将保留原始项目的默认设置，除非在复制过程中清除这些设置。
* 在同一项目上复制任务时，自定义表单和审批流程将转移到复制任务。

  有关复制和复制任务的信息，请参阅[&#128279;](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) [复制和复制任务](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

* 当您将任务移动到另一个项目时，默认任务设置保存在原始项目的任务上，而不管新项目的任务默认设置如何。

  有关移动任务的信息，请参阅[移动任务](../../../manage-work/tasks/manage-tasks/move-tasks.md)。
