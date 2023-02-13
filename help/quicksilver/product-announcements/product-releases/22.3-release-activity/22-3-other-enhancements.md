---
title: 22.3版本时间段内的其他更新
description: 22.3版本时间段内的其他更新
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# 22.3其他增强功能

本页介绍2.3版本到“预览”环境的所有其他增强功能。 这些增强功能在2022年7月11日这一周的生产环境中提供。 有关22.3版本中可用的所有更改的列表，请参阅 [22.3版本概述](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## 更新的工时单

在使用工时单时，我们将继续改进和更新您的体验。 以下是此更新中包含的一些功能：

* 与新Workfront体验相匹配的新外观。

* 自动保存功能，可在添加时自动保存记录的小时和小时注释。

* 更直观的页面布局，以匹配其他对象页面。 例如，我们在时间表中添加了一个左面板。 时间表更新现在显示在左侧面板的“更新”部分中。 您还可以从时间表页中删除时间表，并将时间表添加到收藏夹列表。

* 在搜索项目、任务或问题并将其添加到时间表时获得更好的体验。 这与Workfront中所有其他列表中的体验相匹配。

* “摘要”面板可用于任务和问题，以便直接从时间表添加注释或更新信息。


在当前更新中，我们还弃用了以下功能：

* 已删除从更新创建任务。 自2018.2版本以来，已从所有其他对象的“更新”区域中删除了此功能，但该功能仍在时间表更新流中可用。

* “添加工时单的费用”。 “首选项已从“设置”的“时间表和小时数首选项”区域中删除，您无法再从时间表记录费用。 您仍可以记录任务和项目页面中的费用。


有关更多信息，请参阅以下文章：

* [了解时间表布局](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [配置工时单和工时首选项](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## 增强了左侧导航面板

我们对Adobe Workfront的左侧导航面板进行了多项增强。

* 左侧导航面板的外观已更新为Adobe设计标准，包括颜色和字体。

* 面板底部的“添加自定义部分”链接已更名为“添加功能板”，以更好地说明其功能。

## 在自定义OAuth2应用程序中启用自动刷新令牌旋转

为了让您能够更好地控制自定义OAuth2应用程序的安全性，我们已添加到选项以启用刷新令牌轮换。 启用此选项后，每次使用刷新令牌时，您的应用程序都会自动创建并发送新的刷新令牌，并禁用旧令牌。

您的应用程序必须在每次刷新后存储新的刷新令牌。 Workfront不存储此刷新令牌。

以前，在自定义OAuth2应用程序设置中配置的设置时间段后，刷新令牌会过期。

有关更多信息，请参阅 [为Workfront集成创建OAuth2应用程序](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## 在您的自定义OAuth2集成中为单页Web应用程序使用PKCE

您现在可以使用PKCE在自定义集成中创建单页Web应用程序。 PKCE是一种安全的授权流程，可与动态刷新应用程序（如移动设备应用程序）的应用程序配合使用，但在所有OAuth2客户端中都很有价值。 PKCE使用动态生成的字符串而不是静态客户端密钥，从而消除了泄露的客户端密钥的风险。

以前，自定义OAuth2应用程序的可用选项使用的是用户名和密码，或客户端密钥。

有关更多信息，请参阅 [为Workfront集成创建OAuth2应用程序](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
