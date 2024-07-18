---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: 任务相关性类型概览
description: 依赖关系类型是指任务之间的前置任务关系。 它们根据前置任务的开始或结束来定义相关任务可以开始或结束的时间。
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# 任务相关性类型概览

<!-- Audited: 12/2023 -->

依赖关系类型是指任务之间的前置任务关系。 它们根据前置任务的开始或结束来定义相关任务可以开始或结束的时间。

>[!IMPORTANT]
>
>Adobe Workfront不会根据依赖关系类型限制依赖任务的开始或完成，除非强制实施前置任务关系。 有关强制前置任务的信息，请参阅[强制前置任务](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md)。

在任务之间建立此关系时，必须指定前置任务关系的依赖关系类型。

有关前置任务的详细信息，请参阅[前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

以下是Workfront依赖关系类型：

* **完成 — 开始(fs)**：前置任务必须先完成，相关任务才能开始。 这是默认的依赖关系类型，在未指定其他依赖关系类型时使用。
* **完成 — 完成(ff)**：前置任务必须先完成，相关任务才能完成。
* **开始 — 开始(ss)**：前置任务必须先开始，相关任务才能开始。 除非前置任务至少已启动，否则无法启动相关任务。
* **开始 — 完成(sf)**：前置任务必须先开始，相关任务才能完成。 您可以在前置任务开始之前开始相关任务，但除非前置任务已开始，否则无法完成该任务。
* **Scheduled-Start (sd)**：这会将任务计划为“完成 — 开始”，但实际强制类型是“完成 — 完成”。 使用此项时，相关任务计划在前置任务完成后开始。 然而，执行使得相关任务可以随时开始，但在前置任务完成之前无法完成。

>[!NOTE]
>
>依赖关系类型的缩写在任务列表中用于定义前置任务关系。 有关详细信息，请参阅[任务前置任务概述](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md)中的[任务列表中的前置任务值示例](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md#examples-of-predecessor-values-in-a-task-list)。

