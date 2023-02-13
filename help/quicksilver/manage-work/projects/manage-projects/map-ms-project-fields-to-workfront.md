---
product-area: projects
navigation-topic: manage-projects
title: 将Microsoft项目字段映射到Adobe Workfront项目
description: Adobe Workfront项目和Microsoft项目的项目大多是兼容的。 本文介绍了两个应用程序中最常见的项目字段如何相互映射。
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: c566eb094e96abca6073554433434822c567bc34
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 3%

---

# 将Microsoft项目字段映射到Adobe Workfront项目

Adobe Workfront项目和Microsoft项目的项目大多是兼容的。 使用这两个应用程序，您可以执行以下操作：

* 从Microsoft项目导出项目并将其导入Workfront
* 将项目从Workfront导出，然后将其导入Microsoft项目。 

有关将项目从Microsoft项目导入Workfront的更多信息，请参阅 [从Microsoft项目导入项目](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

有关将项目从Workfront导出以将其导入Microsoft项目的更多信息，请参阅 [将项目导出到Microsoft项目](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

执行此类数据导入时，务必要了解信息如何从一个应用程序转换到另一个应用程序。 大多数情况下，您必须在完成导入后对项目进行一些手动修改。 

## 字段映射概述

>[!NOTE]
>
>计划日期并不总是对应两个系统。 差异可通过计划和Workfront与Microsoft项目之间系统首选项的差异来解决。 这些日期差异还可能导致工作量、持续时间和完成百分比的差异。

| **Microsoft项目字段** | **Workfront字段** |
|---|---|
| 项目标题 | 项目名称 |
| 开始和结束日期 | 计划起始日期和完成日期 |
| 任务名称 | 任务名称 |
| 任务持续时间 | 任务计划持续时间 |
| 任务工作 | 任务计划时数 |
| 任务完成% | 任务完成百分比（基于任务的持续时间） |
| 任务完成百分比 | 任务完成百分比（基于任务的计划小时数） |
| 计划的开始和结束 | 计划起始日期和完成日期 |
| 实际开始和结束 | 实际开始和完成日期 |
| 资源名称 | 任务分配 |
| 分配单位 | 分配分配百分比 |
| 任务说明 | 任务说明 |
| 前置任务 | 前置任务 |

## 未包含的数据概述

有许多项目字段未导入或导出到Workfront。

这些字段包括但不限于：

* 文档附件
* 自定义字段（在项目或任务级别）
* Workfront说明
* 问题
* 具有开始/完成前置关系的任务具有负滞后（导入的任务没有滞后）
* 分配
* 任务约束

   >[!NOTE]
   由于Microsoft项目与Workfront之间没有映射约束，因此请确保任务之间存在前身关系。 否则，导入项目中任务的计划起始日期和计划完成日期可能不准确。 
