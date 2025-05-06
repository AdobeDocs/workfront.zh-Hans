---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 更正工时表的工作周开始日期
description: 时间表上每周的开始日期与我预期的每周开始日期不匹配。
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: ae3fc73e93474c75fd03144b66af23f7142867c0
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# 更正工时表的工作周开始日期

<!--Audited: 5/2025-->

## 问题

时间表上每周的开始日期与我预期的每周开始日期不匹配。

这通常发生在您未分配到时间表配置文件并且您的时间表是手动创建的。


## 解决方案

您的Workfront管理员应该创建时间表配置文件并将每个人分配给配置文件，如[创建、编辑和分配时间表配置文件](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)中所述。 您的Workfront管理员可以定义工时表的开始日期不是预期的每周开始日期。 与他们核实，了解您的时间表的时间表配置文件的开始日期。

如果您的时间表是手动创建的，则时间表中的一周的开始日期会使用用户配置文件中的电子邮件区域设置，如[配置我的设置](/help/quicksilver/workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)一文中所述。

例如，如果“电子邮件区域设置”设置为“英语（美国）”，则时间表中的周从星期日开始。 或者，在“电子邮件区域设置”设置为“英语（英国）”的情况下，时间表中的一周从星期一开始。


<!--This is the old content for this article but I found this was not working this way at all, so I changed it to what it is today: 

## Problem

The start day of the week on my timesheet does not match the start day of the week that is configured on my timesheet profile (as described in [Create, edit, and assign timesheet profiles](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).).

## Solution

The start day of the week of a timesheet in Adobe Workfront uses the language and locale settings in your browser to determine the day of the week. Because of this, you need to update the language and locale settings for your browser. 

For example, with the browser language set to English and the locale set to United States, the week starts on Sunday. Alternatively, the browser language set to English and the locale set to United Kingdom, the start day is Monday.

This setting also affects the start day of the week in the pop-up calendars across the system.

The locale change does not affect the start day of the week on the Resource Grid (or resource grid view). The week always starts on Sunday.

Following are the directions for changing language and locale settings for various browsers that are supported with Workfront.

* **Chrome:** Copy and paste the following link into your Chrome browser: `chrome://settings/languages` then go to Languages.
* **Firefox:**Copy and paste the following link into your Firefox browser: `about:preferences#content` then go to Languages.
* **IE 11:** Tools -> Internet Options -> General -> Languages
* **Safari:** Unfortunately, Safari does not allow changing web browsing languages without also changing your entire operating system language. It is probably easier to simply install another browser like Chrome or Firefox.

-->


