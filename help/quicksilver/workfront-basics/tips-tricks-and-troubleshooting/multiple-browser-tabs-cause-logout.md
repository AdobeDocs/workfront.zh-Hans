---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 多个浏览器选项卡会导致Workfront注销
description: 当用户打开多个浏览器标签时，Workfront 可能会自动注销。
feature: Get Started with Workfront
source-git-commit: ef85b267b3417dddd0c9cc4a2b916b83dc416e14
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 7%

---

# 多个浏览器选项卡会导致Workfront注销

>[!IMPORTANT]
>
>此问题仅出现在已载入Adobe IMS的组织中。

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

* 如果您打开了活动的Workfront选项卡，请重新加载已过期的选项卡。 它会返回到在过期之前打开的页面。

* 如果尚未打开活动的Workfront选项卡，请重新登录Workfront。