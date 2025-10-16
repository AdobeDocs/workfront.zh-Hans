---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 项目更新类型概述
description: 项目的更新类型指示Adobe Workfront计算项目时间线的方式。 项目计划的更改可能会触发项目时间线的更改。 必须自动或手动重新计算项目的时间表，以确保它及时反映这些更改。
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# 项目更新类型概述

项目的更新类型指示Adobe Workfront计算项目时间线的方式。 项目计划的更改可能会触发项目时间线的更改。 必须自动或手动重新计算项目的时间表，以确保它及时反映这些更改。

有关重新计算项目时间表的信息，请参阅[重新计算项目时间表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)。

## 项目更新类型

项目有四种更新类型，具体取决于您希望Workfront重新计算项目时间线的时间。 从下面的列表中选择一个更新类型。

有关如何更新项目的更新类型的信息，请参阅[选择项目更新类型](../../../manage-work/projects/manage-projects/select-project-update-type.md)。

>[!IMPORTANT]
>
>如果项目的时间表超过15年，Workfront不会自动计算时间表或在发生更改时计算时间表。 超过15年的项目的更新类型始终为手动。

* **更改时自动更新：**&#x200B;这是默认设置。 每次在项目或时间线所依赖的其他项目中发生更改时，项目时间线都会更新。 项目的时间表每晚也会更新。 \
  这是推荐的设置，因为它可确保项目时间线始终保持最新。

  当您更新任务或项目并触发时间表重新计算时，所有可用日期都会立即显示，让您能够继续工作。 在具有100个以上任务的项目中，需要更长时间计算的日期将灰显。

  ![](assets/dates-dimmed-when-insline-editing-350x146.png)

  这表示重新计算尚未完成，并且日期可能会发生更改。

* **仅更改：**&#x200B;每次在项目或时间线所依赖的其他项目中发生更改时，项目时间线都会更新；不会发生计划的更新。\
  如果担心系统性能并且项目或时间线所依赖的其他项目中很少发生更改，您可能需要选择此选项。

* **仅限自动：**&#x200B;项目时间线每晚都更新；更改后不会立即更新。\
  如果担心系统性能以及项目或时间线所依赖的其他项目中每天发生许多更改，您可能需要选择此选项。

  >[!NOTE]
  >
  >如果项目处于Planning状态，则不会每晚自动重新计算。 它只会在更改时重新计算。

* **仅手动：**&#x200B;仅当您选择&#x200B;**重新计算时间表**&#x200B;的选项时，项目时间表才会更新，如[重新计算项目时间表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)一节中的“手动重新计算”一节所述。\
  如果要一次对项目进行多项更改，并且希望在所有更改完成后（而不是在每次更改后）重新计算时间线，则可能需要选择此选项。
