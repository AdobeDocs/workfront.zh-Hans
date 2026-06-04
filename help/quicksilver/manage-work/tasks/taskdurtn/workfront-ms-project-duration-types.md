---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Adobe Workfront和Microsoft项目中的持续时间类型
description: Adobe Workfront中可用的持续时间类型与其Microsoft项目中的对应持续时间类型不同，后者称为任务类型。 在Workfront和Microsoft项目之间导出或导入项目时，这有时可能会混淆。
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
TQID: https://experienceleague.adobe.com/avh0ZuYJpsf7Ed5HiWuLkxEA-0PD-1iFvzHmWvpDZiI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 257
ht-degree: 2%

---

# Adobe Workfront和Microsoft项目中的持续时间类型

Adobe Workfront中可用的持续时间类型与其Microsoft项目中的对应持续时间类型不同，后者称为任务类型。 在Workfront和Microsoft项目之间导出或导入项目时，这有时可能会混淆。

有关在Workfront和Microsoft Project之间导入和导出项目的信息，请参阅以下文章：

* [将项目导出到Microsoft项目](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [从Microsoft项目导入项目](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Workfront和Microsoft项目中的持续时间类型

Workfront有四种任务持续时间类型：

* 简单
* 投入比导向
* 计算的工作量
* 计算的分配量

有关信息，请参阅[任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)。

Microsoft项目无法识别这些持续时间类型。 目前，Microsoft项目具有三种与Workfront中的持续时间类型类似的任务类型：

* 固定单位
* 固定工时
* 固定持续时间

## 从Workfront导出到MS Project时，持续时间类型发生更改

将项目从Workfront导出到Microsoft项目时，投入比导向的任务变为固定工作。 简单、计算的工作量和计算的分配量会变为固定单位。

## 从MS Project导入到Workfront时持续时间类型发生更改

将项目从Microsoft项目导入Workfront时，固定单位将变为投入比导向。 固定工作和固定持续时间接收Workfront管理员为您的系统选择的默认持续时间类型。 有关信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
 
(drafting this because it is misleading)
 
</note>
-->
