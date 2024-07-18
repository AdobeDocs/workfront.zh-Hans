---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 锁定和未锁定的组状态
description: 锁定组的自定义状态是一种方法，可确保组及其子组中的人员在其工作流程中使用相同的流程。 当组状态被锁定时，该组和较低组中的所有用户都可以使用该状态。 虽然您(或Workfront管理员)可以编辑或删除您锁定的状态，但以下子组的管理员无法对这些组执行此操作。 相反，解锁组的自定义状态使较低子组的管理员可以更灵活地管理其工作流。 他们可以更改已解锁状态的属性或为其组删除它。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3463e4cb-7336-49b7-b81a-c2acef72f61d
source-git-commit: d67de32fcbe4706cf8a1fc6f5bb8ec9d08b07119
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# 锁定和未锁定的组状态

锁定组的自定义状态是一种方法，可确保组及其子组中的人员在其工作流程中使用相同的流程。 当组状态被锁定时，该组和较低组中的所有用户都可以使用该状态。 虽然您(或Workfront管理员)可以编辑或删除您锁定的状态，但以下子组的管理员无法对这些组执行此操作；他们只能更改其在状态列表中的显示顺序。

相反，解锁组的自定义状态使较低子组的管理员可以更灵活地管理其组中使用的独特工作流。 解锁组状态时，较低子组的管理员可以更改其属性，或删除这些子组的属性。

>[!IMPORTANT]
>
>如果在自定义状态解锁任意时间段后将其锁定，则您对状态的设置将替换较低子组中组管理员所做的设置。 当状态被锁定时，这些管理员无法修改或删除其组的状态。

有关锁定或解锁组状态的说明，请参阅[创建或编辑组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)。

您可以在组审批流程中使用锁定和未锁定状态。 如果您创建的组审批流程具有未锁定的组状态，则用户可以将审批流程附加到与组关联的任何项目、任务或问题。

