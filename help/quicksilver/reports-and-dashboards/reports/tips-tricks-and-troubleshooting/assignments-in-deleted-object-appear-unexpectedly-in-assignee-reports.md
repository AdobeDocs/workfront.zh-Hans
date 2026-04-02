---
title: 被删除对象中的工作分配在被分配人报告中意外出现
description: 被删除对象中的工作分配在被分配人报告中意外出现
author: Courtney
draft: Probably
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# 被删除对象中的工作分配在被分配人报告中意外出现

## 问题

删除具有指定任务的对象后，该对象和指定任务都会被删除。 但是，该任务可能仍会出现在某些报表中。

例如，如果删除分配给用户的任务，则也会删除分配给用户的任务。 但是，如果您稍后运行按任务接受者筛选的任务报告，并且指定了该用户，则该报告仍会列出已删除的任务（如果该任务仍在回收站中）。

## 原因

这是由于回收站的体系结构限制所致。 由于需要重新设计建筑的规模，目前没有解决这个问题的计划。
