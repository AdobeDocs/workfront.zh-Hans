---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 移动或复制的任务或问题的自定义状态
description: 将任务或问题移动或复制到其他项目时，任务或问题上的某些状态可能会更新以匹配目标项目组使用的状态。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4bd9b89d-9c66-4af7-97bf-f9518ad55d7c
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
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
