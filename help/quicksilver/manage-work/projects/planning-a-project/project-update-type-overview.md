---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 项目更新类型概述
description: 项目的更新类型指示Adobe Workfront如何计算项目的时间轴。 项目计划中的更改可能会触发项目时间轴中的更改。 必须自动或手动重新计算项目的时间轴，以确保项目的时间轴随这些更改而保持最新。
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# 项目更新类型概述

项目的更新类型指示Adobe Workfront如何计算项目的时间轴。 项目计划中的更改可能会触发项目时间轴中的更改。 必须自动或手动重新计算项目的时间轴，以确保项目的时间轴随这些更改而保持最新。

有关重新计算项目时间轴的信息，请参阅 [重新计算项目时间表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

## 项目更新类型

项目有四种更新类型，具体取决于您希望Workfront何时重新计算项目时间轴。 从下面的列表中选择更新类型。

有关如何更新项目更新类型的信息，请参阅 [选择项目更新类型](../../../manage-work/projects/manage-projects/select-project-update-type.md).

>[!IMPORTANT]
>
>如果项目的时间轴超过15年，Workfront不会自动计算时间轴或在发生更改时计算时间轴。 超过15年的项目更新类型始终为手动。

* **自动和更改：** 这是默认设置。 每当项目或时间轴所依赖的其他项目中发生更改时，项目时间轴都会更新。 项目时间轴也会在每晚更新。 \
   这是推荐的设置，因为它可确保项目时间轴始终为最新。

   当您更新任务或项目并触发时间轴重新计算时，所有可用日期都会立即显示，从而允许您继续工作。 对于任务超过100个的项目，需要较长计算的日期将变暗。

   ![](assets/dates-dimmed-when-insline-editing-350x146.png)

   这表示重新计算尚未完成，并且日期可能会发生更改。

* **仅更改：** 每当项目或时间轴所依赖的其他项目中发生更改时，项目时间轴都会更新；不会进行计划更新。\
   如果您担心系统性能，并且在项目或时间轴所依赖的其他项目中很少发生更改，则可能需要选择此选项。

* **仅自动：** 项目时间表每天晚上都会更新；所做的更改不会立即更新。\
   如果您担心系统性能，并且在项目或时间轴所依赖的其他项目中每天发生许多更改，则可能需要选择此选项。

   >[!NOTE]
   >
   >如果项目处于“计划”状态，则它不会每天晚上自动重新计算。 它只会在更改时重新计算。

* **仅手动：** 仅当您选择 **重新计算时间轴**，如文章“手动重新计算”一节中所述 [重新计算项目时间表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
   如果您同时对项目进行多次更改，并且希望在所有更改（而不是在每次更改后）之后重新计算时间轴，则可能需要选择此选项。
