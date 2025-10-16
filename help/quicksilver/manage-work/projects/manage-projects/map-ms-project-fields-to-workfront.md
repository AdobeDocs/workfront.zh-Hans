---
product-area: projects
navigation-topic: manage-projects
title: 将Microsoft项目字段映射到Adobe Workfront项目
description: Adobe Workfront中的项目与Microsoft项目中的项目通常兼容。 本文介绍了这两个应用程序中最常见的项目字段如何相互映射。
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 4%

---

# 将Microsoft项目字段映射到Adobe Workfront项目

Adobe Workfront中的项目与Microsoft项目中的项目通常兼容。 使用这两个应用程序，您可以执行以下操作：

* 从Microsoft项目导出项目并将它们导入Workfront
* 从Workfront导出项目并将它们导入Microsoft项目。 

有关将项目从Microsoft项目导入到Workfront的更多信息，请参阅[从Microsoft项目导入项目](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)。

有关从Workfront导出项目以将其导入Microsoft项目的详细信息，请参阅[将项目导出到Microsoft项目](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)。

在执行此类数据导入时，了解信息如何从一个应用程序转换为另一个应用程序非常重要。 大多数情况下，在完成导入后，您需要对项目进行一些手动修改。 

## 字段映射概述

>[!NOTE]
>
>两个系统之间的计划日期并不总是对应。 差异可以通过时间表以及Workfront和Microsoft项目之间的系统偏好设置差异来解释。 这些日期差异还可能导致工作量、持续时间和完成百分比方面的差异。

| **Microsoft项目字段** | **Workfront字段** |
|---|---|
| 项目标题 | 项目名称 |
| 开始日期和完成日期 | 计划的开始日期和完成日期 |
| 任务名称 | 任务名称 |
| 任务持续时间 | 任务计划持续时间 |
| 任务工时 | 任务已计划小时数 |
| 任务%完成 | 任务完成百分比（基于任务的持续时间） |
| 任务工作完成百分比 | 任务完成百分比（基于任务的计划小时数） |
| 计划的开始和结束 | 计划的开始日期和完成日期 |
| 实际开始日期和结束日期 | 实际开始日期和完成日期 |
| 资源名称 | 任务分派 |
| 工作单位 | 分配分配百分比 |
| 任务注释 | 任务说明 |
| 前置任务 | 前置任务 |

## 未包括的数据概述

有许多项目字段未导入或从Workfront导出。

这些字段包括但不限于：

* 文档附件
* 自定义字段（在项目或任务级别）
* Workfront注释
* 问题
* 具有开始/完成前置任务关系的任务中的负延迟（导入的任务没有延迟）
* 任务
* 任务限制

  >[!NOTE]
  >
  >由于约束不会在Microsoft项目和Workfront之间映射，因此请确保任务之间具有前置任务关系。 否则，任务的计划开始日期和计划完成日期在导入项目中可能不准确。 
