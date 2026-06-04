---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 在利率变化时，防止“重新计算财务”操作影响历史小时数
description: 您需要更新用户或工作角色的小时成本（由于加薪或其他情况），但您不希望此更改影响之前已登录项目的小时数，或者希望它仅影响部分历史小时数。
author: Lisa
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
TQID: https://experienceleague.adobe.com/TBeLp0FaUmlRk2uk5SdCqntrUWeAAVucox6Dyx5M0Uw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 188
ht-degree: 0%

---

# 在利率变化时，防止“重新计算财务”操作影响历史小时数

## 问题

您需要更新用户或工作角色的小时成本（由于加薪或其他情况），但您不希望此更改影响之前已登录项目的小时数，或者希望它仅影响部分历史小时数。

## 解决方案

添加您不希望更改为项目记帐记录的小时数，并将记帐记录的状态设置为“已记帐”。  该比率将锁定旧比率，并且将被重新计算财务操作忽略。  任何不属于已记帐记帐记录的小时数均按新费率计算。 有关详细信息，请参阅[重新计算项目财务](../../manage-work/projects/project-finances/recalculate-project-finances.md)。
