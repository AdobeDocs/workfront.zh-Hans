---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: 任务依赖关系类型概述
description: 依赖关系类型是指任务之间的前置关系。 它们根据从属任务的上一任务的开始或结束来定义从属任务的开始或结束时间。
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# 任务依赖关系类型概述

依赖关系类型是指任务之间的前置关系。 它们根据从属任务的上一任务的开始或结束来定义从属任务的开始或结束时间。

>[!IMPORTANT]
>
>Adobe Workfront不会根据依赖关系类型限制从属任务的开始或结束，除非强制实施前置关系。 有关强制前置任务的信息，请参阅 [强制前置任务](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

在任务之间建立此关系时，必须指定前置关系的“依赖类型”。

有关前置任务的详细信息，请参阅 [任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

以下是Workfront依赖关系类型：

* **完成开始(fs)**:前置任务必须在从属任务开始之前完成。 这是默认的依赖关系类型，在未指定其他依赖关系类型时使用。
* **完成(ff)**:前置任务必须在从属任务完成之前完成。
* **开始(ss)**:前置任务必须在从属任务开始之前启动。 除非前任至少已启动，否则无法启动从属任务。
* **开始完成(sf)**:前置任务必须在从属任务完成之前启动。 您可以在前置任务开始之前启动从属任务，但除非前置任务开始，否则无法完成该任务。
* **计划开始(sd)**:这会将任务计划为“完成开始”，但实际执行类型是“完成完成”。 使用此方法时，将安排从属任务在前置任务完成后启动。 但是，强制执行使从属任务可以随时启动，但只有在上一任务完成之后才能完成。
