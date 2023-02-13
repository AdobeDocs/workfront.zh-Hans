---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: 批量编辑用户的其他组
description: 在批量编辑时，我尝试向大量用户添加单个其他组。 保存更改后，所有现有的其他组都被删除，并且只保留新的其他组。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# 批量编辑用户的其他组

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

## 问题：

在批量编辑时，我尝试向大量用户添加单个其他组。
保存更改后，所有现有的其他组都被删除，并且只保留新的其他组。

## 答案：

结果行为取决于所选用户的当前组成员资格：

* 如果所有选定用户的其他组成员关系完全匹配……在您选择用户并选择 [!UICONTROL 编辑], [!UICONTROL 其他组] 字段将显示这些用户所属的所有组的完整列表。

* 如果所选用户具有不同的其他组成员关系……选择用户并单击 [!UICONTROL 编辑], [!UICONTROL 其他组] 字段将为空。

单击 **[!UICONTROL 保存更改]**，则保存“其他群组”字段中显示的任何内容。

字段的先前内容会被覆盖。
