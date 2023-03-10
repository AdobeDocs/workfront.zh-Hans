---
product-area: templates
navigation-topic: templates-navigation-topic
title: 模板中的开始和完成天数概述
description: 您可以使用项目模板来捕获与组织中的项目关联的大多数可重复流程、信息和设置。 虽然项目具有特定的开始和结束日期，但模板具有通用的开始和结束日期，以根据项目的总体时间表指示这些日期在项目中的哪个位置。
author: Alina
feature: Work Management
exl-id: caa0e7b1-37c3-4973-92ce-cc93df4e4186
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---

# 模板中的开始和完成天数概述

您可以使用项目模板来捕获与组织中的项目关联的大多数可重复流程、信息和设置。 虽然项目具有特定的开始和结束日期，但模板具有通用的开始和结束日期，以根据项目的总体时间表指示这些日期在项目中的哪个位置。

**示例：** 如果项目的开始日期是4月1日，并且您希望任务从4月3日（项目开始后两天）开始，则用于创建项目的模板上的相应任务应从模板的第2天开始，在第2天，模板的第一天被视为第0天。

## 开始日

使用模板和模板任务时，请考虑以下事项：

* 默认情况下，模板的开始日期为0，模板任务和模板的开始日期为0。 模板任务的开始日期可以更改，但不会更改模板的开始日期。
* 模板任务的开始日期表示在从模板创建项目时，Workfront会向任务的计划开始日期添加的工作天数。 例如，您可以有一个模板，其中只包含一个任务，而模板任务的“开始日”为4。 模板的开始日期仍为0。 当您从此模板创建项目时，如果项目的计划模式为开始日期，而项目的计划开始日期为2019年11月1日，则新创建的任务会向此日期添加4天，并将其计划开始日期值设置为2019年11月5日。

以下是一些操作可能会更改模板任务的开始日期：

* 更新前置模板任务的持续时间
* 更新任务约束

   使用基于日期的任务约束时，您可以手动更新模板任务的开始日。 基于日期的任务约束的一些示例包括固定日期、不早于、不迟于、必须开始。

* 更新模板任务前置任务

## 完成日期

模板的完成日期是完成最后一个模板任务的日期。 默认情况下，所有模板任务和模板都显示完成日期为1，因为Workfront假定任何模板任务的持续时间为1天。 模板任务的完成日可能会发生更改，这也会更改模板的完成日。 模板的完成日将变为未来项目的计划完成日期，模板任务的完成日将变为未来项目任务的计划完成日期。

以下是一些可能更改模板任务完成日的操作：

* 更新模板任务的持续时间
* 更新任务约束

   使用基于日期的任务约束时，您可以手动更新模板任务的完成日。 基于日期的任务约束的一些示例包括固定日期、不早于完成、不迟于完成、必须完成。

* 更新模板任务前置任务

## 使用计划完成的模板

您可以从完成日计划模板。 有关更多信息，请参阅 [编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

使用从完成日期开始计划的模板时，请考虑以下事项：

* 更改“开始日”会将任务约束设置为必须开始。
* 更改完成日期会将任务约束设置为必须完成。
* 从完成日开始计划模板时，任务约束日将从完成日计算。

   **示例：** 模板的持续时间为285天，并且模板任务的持续时间为60天。 如果将任务约束设置为必须开始于，将约束日设置为120，则开始日为165(285 - 120)，完成日为225(165 + 60)。 因此，编辑开始日时，它实际上被解释为约束日。
