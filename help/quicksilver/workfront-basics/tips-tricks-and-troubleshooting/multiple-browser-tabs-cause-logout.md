---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 多个浏览器选项卡会导致Workfront注销
description: 当用户打开多个浏览器标签时，Workfront 可能会自动注销。
feature: Get Started with Workfront
author: Becky
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
TQID: https://experienceleague.adobe.com/Zof7zbTOm-w1vyBTchiXJv2QrNYbOxw9O4DYIjYQ6Ss
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 165
ht-degree: 32%

---

# 多个浏览器选项卡会导致Workfront注销

## 问题

当用户打开了多个浏览器选项卡，并单击进入已处于不活动状态一段时间的选项卡时，选项卡会话已过期。 用户看不到他们打开的页面，而是看到以下消息：

```
Tab session expired
This tab session has been halted due to inactivity. Refresh the tab to continue where you left off.
```

## 原因

此行为是由基于策略的身份验证(PBA)导致的，PBA是您的组织配置的一种安全措施。 当选项卡处于非活动状态的时间超过在组织的PBA配置中设置的时间限制时，选项卡会话将过期。

## 解决方案

解决方案取决于您是否在登录到Workfront的其他选项卡中处于活动状态。

* 如果您打开了活动的 Workfront 选项卡，请重新加载已过期的选项卡。 它将会返回到您在过期之前打开的页面。

* 如果您没有打开活动的 Workfront 选项卡，请再次登录 Workfront。
