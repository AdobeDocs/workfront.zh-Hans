---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 组锁定状态和已解锁状态
description: 锁定群组的自定义状态是一种方法，可确保群组及其子组中的人员在其工作流程中使用相同的流程。 组状态锁定后，该组和较低组中的所有用户都可以使用该状态。 尽管您(或Workfront管理员)可以编辑或删除您锁定的状态，但下面子组的管理员无法为这些组编辑或删除状态。 相反，解锁群组的自定义状态，使较低子组的管理员能够更灵活地管理其工作流。 他们可以更改已解锁状态的属性，或删除其组的属性。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3463e4cb-7336-49b7-b81a-c2acef72f61d
source-git-commit: d67de32fcbe4706cf8a1fc6f5bb8ec9d08b07119
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# 组锁定状态和已解锁状态

锁定群组的自定义状态是一种方法，可确保群组及其子组中的人员在其工作流程中使用相同的流程。 组状态锁定后，该组和较低组中的所有用户都可以使用该状态。 虽然您(或Workfront管理员)可以编辑或删除您锁定的状态，但以下子组的管理员不能为这些组编辑或删除状态；他们只能更改其在“状态”列表中的显示顺序。

相反，解锁群组的自定义状态后，较低子组的管理员可以更灵活地管理其群组中使用的唯一工作流。 解锁组状态后，下级子组的管理员可以更改其属性或删除这些子组的属性。

>[!IMPORTANT]
>
>如果在解锁自定义状态一段时间后锁定该状态，则状态设置将替换下方子组中的组管理员所做的设置。 状态处于锁定状态时，这些管理员无法修改或删除其组的状态。

有关锁定或解锁组状态的说明，请参阅 [创建或编辑群组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

您可以在组批准流程中同时使用锁定状态和已解锁状态。 如果创建具有已解锁组状态的组批准流程，则用户可以将批准流程附加到与该组关联的任何项目、任务或问题。

