---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: 批量编辑用户的其他组
description: 在批量编辑时，我尝试将单个其他组添加到大量用户。 保存更改后，将删除所有现有的其他组，仅保留新的其他组。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
TQID: 'https://experienceleague.adobe.com/oH--gAyZgNsSf-HBHUs7TSZxW3jAktySyvZx-wNlpG0'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
    internal-label: Workfront Proof
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%
---
# 批量编辑用户的其他组

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

## 问题：

在批量编辑时，我尝试将单个其他组添加到大量用户。
保存更改后，将删除所有现有的其他组，仅保留新的其他组。

## 回答：

产生的行为取决于所选用户的当前组成员资格：

* 如果所有选定用户“其他组”成员资格完全匹配……
选择用户并选择[!UICONTROL 编辑]后，[!UICONTROL 其他组]字段将显示完整列表
这些用户所属的所有组的成员。

* 如果所选用户具有不同的其他组成员资格……
选择用户并单击[!UICONTROL 编辑]后，[!UICONTROL 其他组]字段将为空白。

单击&#x200B;**[!UICONTROL 保存更改]**&#x200B;后，将保存“其他组”字段中显示的任何内容。

字段的上一个内容将被覆盖。
