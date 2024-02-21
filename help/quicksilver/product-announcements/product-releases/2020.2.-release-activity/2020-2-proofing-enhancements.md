---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2校对增强功能
description: 本页介绍了2020.2版本中对生产环境所做的所有“验证”增强。 这些增强功能在2020年5月11日这一周的生产环境中提供。
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 021c6e0c-3593-40f7-8eeb-7e016001893e
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---

# 2020.2校对增强功能

本页介绍了2020.2版本中对生产环境所做的所有“验证”增强。 这些增强功能在2020年5月11日这一周的生产环境中提供。

有关2020.2版本可用的所有更改列表，请参阅 [2020.2版概述](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## 校对域正在从proofhq.com更改为workfront.com。

>[!NOTE]
>
>此功能最初作为2020.1版的一部分进行介绍，但在发布到生产环境之前已从版本中删除。

如果您的防火墙或邮件服务器配置为仅允许特定供应商访问，则必须将以下附加URL添加到您的Workfront，以确保贵组织中的用户可以在列入允许列表中的浏览器验证查看器和桌面验证查看器中查看验证：

&#42;.workfront.com

此 &#42;proofhq.com URL仍然是必需的。

有关更新允许列表的详细信息，请参阅 [配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

此更新仅适用于Workfront中的验证；在使用Workfront Proof独立应用程序时，此更新不适用。

## 来宾所做的校对注释会出现在“更新”区域中

为了简化校对协作，访客注释会显示在更新区域中。

以前，来宾所做的验证评论仅在验证中可用。
