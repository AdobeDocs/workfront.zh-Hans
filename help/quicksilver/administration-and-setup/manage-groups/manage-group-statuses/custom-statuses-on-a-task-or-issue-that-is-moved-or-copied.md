---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 移动或复制的任务或问题的自定义状态
description: 将任务或问题移动或复制到其他项目时，任务或问题上的某些状态可能会更新以匹配目标项目组使用的状态。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4bd9b89d-9c66-4af7-97bf-f9518ad55d7c
TQID: 'https://experienceleague.adobe.com/GzG3KBfUw05edjA0DVRtODyGprG2mKVjOuUV2L5eWto'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: 254442ca-6997-5cfa-963e-f420870aea53
    internal-label: People Teams and Groups
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%
---
# 移动或复制的任务或问题的自定义状态

将任务或问题移动或复制到其他项目时，任务或问题上的某些状态可能会更新以匹配目标项目组使用的状态。 这取决于该组中是否存在具有相同键的状态：

* 如果任务或问题上的状态与目标项目的组使用的状态具有相同的键，则任务或问题上的状态将保持不变。

  如果这两种状态的标签不匹配，任务或问题上的状态会继承目标项目组使用的状态标签。

* 如果任务或问题中的状态与目标项目组中的对等状态具有不同的键，则任务或问题中的状态将更改为目标项目组中的对等默认状态。

有关状态键的信息，请参阅[创建或编辑组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)。
