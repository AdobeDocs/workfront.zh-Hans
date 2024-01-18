---
title: 22.3版本发布时间范围内的其他更新
description: 22.3版本发布时间范围内的其他更新
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 22.3其他增强功能

本页介绍了在22.3版本中对“预览”环境进行的所有其他增强。 这些增强功能已在2022年7月11日这一周的生产环境中提供。 有关22.3版本可用的所有更改列表，请参阅 [22.3发行版概述](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## 已更新工时表

我们将继续改进并更新您在使用时间表时的体验。 以下是此更新包含的一些功能：

* 采用新的外观，以便与新的Workfront体验相匹配。

* 自动保存功能可在您添加所记录的小时和小时评论时自动保存它们。

* 更加直观的页面布局以匹配其他对象页面。 例如，我们在时间表中添加了一个左侧面板。 时间表更新现在显示在左侧面板的更新部分中。 您还可以从时间表页面中删除时间表，并将时间表添加到收藏夹列表。

* 在搜索项目、任务或问题并将其添加到时间表时获得更好的体验。 这与Workfront所有其他列表中的体验相匹配。

* “摘要”面板适用于直接从时间表添加注释或更新信息的任务和问题。


通过当前更新，我们还弃用了以下功能：

* 删除了通过更新创建任务。 自2018.2版本发布以来，此功能已从所有其他对象的更新区域移除，但在时间表更新流中仍然可用。

* “从时间表添加费用。 “偏好设置已从‘设置’的‘时间表和小时偏好设置’区域删除，您无法再从‘时间表’记录费用。 您仍然可以从任务和项目页面记录费用。


有关更多信息，请参阅以下文章：

* [了解时间表布局](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [配置时间表和小时首选项](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## 左侧导航面板的增强功能

我们对Adobe Workfront中的左侧导航面板进行了几项增强。

* 左侧导航面板的外观和感觉已更新为Adobe设计标准，包括颜色和字体。

* 面板底部的“添加自定义部分”链接已重命名为“添加仪表板”，以更好地说明其功能。

## 在自定义OAuth2应用程序中启用自动刷新令牌轮换

为了让您更好地控制自定义OAuth2应用程序的安全性，我们添加了启用刷新令牌轮换的选项。 启用此选项后，每次使用刷新令牌时，您的应用程序都会自动创建和发送新的刷新令牌，并禁用旧的刷新令牌。

您的应用程序必须在每次刷新后存储新的刷新令牌。 Workfront未存储此刷新令牌。

以前，刷新令牌会在自定义OAuth2应用程序设置中配置的一段时间后过期。

有关更多信息，请参阅 [为Workfront集成创建OAuth2应用程序](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## 在单页Web应用程序的自定义OAuth2集成中使用PKCE

您现在可以使用PKCE在自定义集成中创建单页Web应用程序。 PKCE是一种安全授权流，可与动态刷新应用程序（如移动应用程序）配合使用，但在所有OAuth2客户端中都具有很高的价值。 PKCE使用动态生成的字符串，而不是静态客户端密钥，从而消除了泄露客户端密钥的风险。

以前，自定义OAuth2应用程序的可用选项使用用户名和密码或客户端密钥。

有关更多信息，请参阅 [为Workfront集成创建OAuth2应用程序](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
