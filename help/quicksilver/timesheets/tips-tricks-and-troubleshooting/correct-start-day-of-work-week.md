---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 更正工时单的工作周开始日期
description: 我的时间表上一周的开始日期与在时间表配置文件上配置的一周的开始日期不匹配。
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# 更正工时单的工作周开始日期

## 问题

我的时间表上一周的开始日期与在时间表配置文件上配置的一周的开始日期不匹配(如 [创建、编辑和分配工时单配置文件](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).)。

## 解决方案

在Adobe Workfront中，时间表一周的第一天使用浏览器中的语言和区域设置来确定一周中的哪一天。 因此，您需要更新浏览器的语言和区域设置。 

例如，浏览器语言设置为英语，区域设置设置为美国，一周从星期日开始。 或者，浏览器语言设置为英语，区域设置设置为英国，开始日期为星期一。

此设置还会影响整个系统中弹出日历中一周的开始日期。

区域设置更改不会影响资源网格（或资源网格视图）上一周的开始日期。 一周总是在星期日开始。

以下是Workfront支持的各种浏览器的语言和区域设置更改说明。

* **铬黄：** 将以下链接复制并粘贴到您的Chrome浏览器中： `chrome://settings/languages` 然后转到语言。
* **Firefox:**将以下链接复制并粘贴到Firefox浏览器中： `about:preferences#content` 然后转到语言。
* **IE 11:** 工具 — > Internet选项 — >常规 — >语言
* **Safari:** 遗憾的是，Safari不允许在不更改整个操作系统语言的情况下更改Web浏览语言。 只需安装其他浏览器（如Chrome或Firefox），可能会更加容易。

 
