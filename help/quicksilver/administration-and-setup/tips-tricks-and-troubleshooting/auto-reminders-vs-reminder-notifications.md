---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 自动提醒与提醒通知
description: 本文介绍了自动提醒和提醒通知之间的差异，并提供了每种情况的情景。 有关所有 [!DNL Adobe Workfront] 通知，请参阅Adobe [!DNL Workfront] 通知。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 26c6fa2c-5c3a-4f53-bd7e-e49a623ff60d
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# 自动提醒与提醒通知

本文介绍了自动提醒和提醒通知之间的差异，并提供了每种情况的情景。 有关所有 [!DNL Adobe Workfront] 通知，请参阅 [[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md).

## 自动提醒

以下特征专门用于自动提醒：

* 只能由 [!DNL Workfront] 管理员
* 在所有任务和问题到期、延迟或接近计划完成日期时触发
* 只能发送给被分派人、被分派人的经理或直接经理的经理。
* 不能为其附加电子邮件模板。

方案：如果您希望在整个系统的所有任务和问题上触发提醒，请配置自动提醒设置。 有关更多信息，请参阅 [设置自动提醒](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

## 提醒通知

以下特征专门用于提醒通知：

* 可由管理员或具有计划许可证和对提醒通知拥有管理访问权限的任何用户创建
* 只能手动与对象关联
* 只能通知附加的对象
* 可以发送给各种对象利益相关方，如所有者、创建者、审批者或代理人
* 可以使用默认电子邮件，也可以使用附加的自定义电子邮件模板

方案：如果要为项目、时间表生成提醒，或要自定义任务和问题的提醒，请配置提醒通知。 有关更多信息，请参阅 [设置提醒通知](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
