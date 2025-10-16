---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 在利率变化时，防止“重新计算财务”操作影响历史小时数
description: 您需要更新用户或工作角色的小时成本（由于加薪或其他情况），但您不希望此更改影响之前已登录项目的小时数，或者希望它仅影响部分历史小时数。
author: Lisa
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# 在利率变化时，防止“重新计算财务”操作影响历史小时数

## 问题

您需要更新用户或工作角色的小时成本（由于加薪或其他情况），但您不希望此更改影响之前已登录项目的小时数，或者希望它仅影响部分历史小时数。

## 解决方案

添加您不希望更改为项目记帐记录的小时数，并将记帐记录的状态设置为“已记帐”。  该比率将锁定旧比率，并且将被重新计算财务操作忽略。  任何不属于已记帐记帐记录的小时数均按新费率计算。 有关详细信息，请参阅[重新计算项目财务](../../manage-work/projects/project-finances/recalculate-project-finances.md)。
