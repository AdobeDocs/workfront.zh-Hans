---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 防止在费率发生更改时重新计算财务费用操作影响历史小时数
description: 您需要更新用户或职务角色的每小时成本（由于加薪或其他情况），但您不希望此更改影响以前已登录项目的小时数，或希望它仅影响部分历史小时数。
author: Alina
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# 防止在费率发生更改时重新计算财务费用操作影响历史小时数

## 问题

您需要更新用户或职务角色的每小时成本（由于加薪或其他情况），但您不希望此更改影响以前已登录项目的小时数，或希望它仅影响部分历史小时数。

## 解决方案

将您不希望更改的小时数添加到项目上的账单记录，并将账单记录的状态设置为“已开单”。  这将锁定旧汇率，并且Recalculate Finecs操作将忽略此锁定。  任何不属于已计费账单记录的小时数均按新费率计算。 有关更多信息，请参阅 [重新计算项目财务](../../manage-work/projects/project-finances/recalculate-project-finances.md).
