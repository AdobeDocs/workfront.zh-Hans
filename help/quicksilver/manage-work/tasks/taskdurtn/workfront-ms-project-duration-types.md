---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Adobe Workfront和Microsoft项目中的持续时间类型
description: Adobe Workfront中可用的持续时间类型与Microsoft项目中的相应任务类型不同，后者称为任务类型。 在Workfront和Microsoft项目之间导出或导入项目时，这有时可能会造成混淆。
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 2%

---

# Adobe Workfront和Microsoft项目中的持续时间类型

Adobe Workfront中可用的持续时间类型与Microsoft项目中的相应任务类型不同，后者称为任务类型。 在Workfront和Microsoft项目之间导出或导入项目时，这有时可能会造成混淆。

有关在Workfront和Microsoft项目之间导入和导出项目的信息，请参阅以下文章：

* [将项目导出到Microsoft项目](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [从Microsoft项目导入项目](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Workfront和Microsoft项目中的持续时间类型

Workfront有四种任务持续时间类型：

* 简单
* 投入比导向
* 计算的工作量
* 计算的分配量

有关信息，请参阅 [任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Microsoft项目无法识别这些持续时间类型。 目前，Microsoft项目有三种与Workfront中的持续时间类型类似的任务类型：

* 固定件数
* 固定工作
* 固定持续时间

## 持续时间类型在从Workfront导出到MS项目时发生更改

将项目从Workfront导出到Microsoft项目时，“工作驱动”任务将变为固定工作。 简单、计算的工作和计算分配变为固定单位。

## 持续时间类型在从MS项目导入到Workfront时发生更改

将项目从Microsoft项目导入Workfront时，固定单位会变得努力。 “固定工作”和“固定持续时间”接收Workfront管理员为您的系统选择的默认持续时间类型。 有关信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
