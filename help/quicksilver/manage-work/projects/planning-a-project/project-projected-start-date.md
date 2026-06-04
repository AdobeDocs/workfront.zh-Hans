---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 项目预计开始日期概览
description: 预计开始日期是基于项目上第一个任务的预计开始日期的项目将要开始的实时日期。
author: Alina
feature: Work Management
exl-id: 6277e6cf-0a73-4ba8-a3fd-c0da473dc5d4
TQID: https://experienceleague.adobe.com/2rcx201EGt4cqRpqfXws6P-NbRnXyVlFoTbJrQJBipg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 430
ht-degree: 0%

---

# 项目预计开始日期概览

## 项目和任务的预计开始日期概览

预计开始日期是基于项目上第一个任务的预计开始日期的项目将要开始的实时日期。

当您首次计划项目时，任务和项目的计划开始日期和计划开始日期相同。 由于可能会出现延迟或任务可能提前完成，因此预计开始日期可能与计划开始日期不同。

项目触发程序上第一个任务的预计开始日期更改项目预计开始日期更改。

## 修改任务的预计开始日期

项目或任务的预计开始日期由Adobe Workfront进行计算，无法手动修改。

以下事件可以触发在任务的预计开始日期进行修改：

* 当您开始处理任务时，任务的“实际开始日期”将成为其“预计开始日期”。
* 如果任务的计划开始日期过去，则预计开始日期将移至未来，指示任务可以开始的最早日期。\
  在计算任务的最早可用开始日期时，Workfront会考虑任务的已计划小时数以及项目或分配给任务的用户的计划。
* 前置任务如果落后运行，则对其依赖任务的预计开始日期产生影响。 依赖任务的预计开始日期根据前置任务的依赖关系类型以及前置任务的预计日期移动。

如果这些任务中的任何一个是项目中的第一个任务，则项目的预计起始日期将更改为匹配此任务的预计起始日期。

## 查找项目或任务的预计开始日期

您可以在Workfront的以下区域中找到项目或任务的预计开始日期：

* 您可以将其添加到项目、任务报告或视图。

  有关创建报告的详细信息，请参阅文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

* 在项目的项目详细信息部分或任务的任务详细信息部分中。
