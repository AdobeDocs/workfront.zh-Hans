---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 自动提醒与提醒通知
description: 本文介绍了自动提醒与提醒通知之间的区别，并提供了每种的情景。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 26c6fa2c-5c3a-4f53-bd7e-e49a623ff60d
TQID: https://experienceleague.adobe.com/hSVm-rgiBcbHaCwO1veCLEo-q6U5SWzt58qO6KqC84M
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 249
ht-degree: 0%

---

# 自动提醒与提醒通知

本文介绍了自动提醒与提醒通知之间的区别，并提供了每种的情景。 有关所有[!DNL Adobe Workfront]通知的更多信息，请参阅[[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md)。

## 自动提醒

以下特性专用于自动提醒：

* 只能由[!DNL Workfront]管理员打开和编辑
* 在到期时、延迟或接近计划完成日期时，在所有任务和问题中触发
* 只能发送给被分派人、被分派人的经理或直接经理的经理。
* 无法向其附加电子邮件模板。

方案：如果您希望提醒在整个系统中的所有任务和问题中触发，则配置自动提醒设置。 有关详细信息，请参阅[设置自动提醒](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md)。

## 提醒通知

以下特征特定于提醒通知：

* 可以由管理员创建，也可以由任何具有“计划标准”许可证和管理权限的用户创建“提醒通知”
* 只能手动关联到对象
* 只能通知有关附加对象的信息
* 可以发送给各种对象利益相关者，如所有者、创建者、批准者或任务接受者
* 可以使用默认电子邮件或使用附加的自定义电子邮件模板

情景：如果您要为项目、时间表构建提醒，或者想要自定义任务和问题的提醒，则配置提醒通知。 有关详细信息，请参阅[设置提醒通知](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md)。
