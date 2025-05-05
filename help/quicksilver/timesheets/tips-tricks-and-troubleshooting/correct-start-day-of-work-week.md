---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 更正工时表的工作周开始日期
description: 时间表上每周的开始日期与时间表配置文件上配置的一周中的开始日期不匹配。
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# 更正工时表的工作周开始日期

## 问题

时间表上一周的开始日期与时间表配置文件（如[创建、编辑和分配时间表配置文件](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)中所述）上配置的每周开始日期不匹配。

## 解决方案

Adobe Workfront中时间表一周的开始日期使用浏览器中的语言和区域设置来确定一周的哪一天。 因此，您需要更新浏览器的语言和区域设置。

例如，如果将浏览器语言设置为“英语”，区域设置设置为“美国”，则一周从星期日开始。 此外，浏览器语言设置为英语，区域设置设置为英国，开始日期是星期一。

此设置还会影响系统中弹出日历中一周的开始日期。

区域设置更改不会影响资源网格（或资源网格视图）上星期的开始日期。 一周总是在星期日开始。

以下是Workfront支持的各种浏览器更改语言和区域设置的说明。

* **Chrome：**&#x200B;将以下链接复制并粘贴到Chrome浏览器中： `chrome://settings/languages`，然后转到“语言”。
* **Firefox：**&#x200B;将以下链接复制并粘贴到Firefox浏览器中： `about:preferences#content`，然后转到语言。
* **IE 11：**&#x200B;工具 — > Internet选项 — >常规 — >语言
* **Safari：**&#x200B;很遗憾，Safari不允许在不更改整个操作系统语言的情况下更改Web浏览语言。 直接安装其他浏览器(如Chrome或Firefox)可能更容易。


