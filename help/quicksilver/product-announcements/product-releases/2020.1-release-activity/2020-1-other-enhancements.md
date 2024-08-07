---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1其他增强功能
description: 本页介绍了2020.1版本对Workfront常规区域所做的所有增强。 这些增强功能目前在“预览”环境中提供，并将于2020年3月底或4月初在“生产”环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a716590c-c833-458a-a138-9bc0723e5896
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# 2020.1其他增强功能

本页介绍了2020.1版本对Workfront常规区域所做的所有增强。 这些增强功能目前在“预览”环境中提供，并将于2020年3月底或4月初在“生产”环境中提供。

有关2020.1版本可用的所有更改列表，请参阅[2020.1版本概述](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md)。

## 列入允许列表向添加验证所需的更改

>[!NOTE]
>
>此功能已从2020.1版本中删除。 稍后将提供。

校对域正在从proofhq.com更改为workfront.com。

如果您的防火墙或邮件服务器配置为仅允许特定供应商访问，则必须将以下附加URL添加到您的Workfront，以确保贵组织中的用户可以在列入允许列表中的浏览器验证查看器和桌面验证查看器中查看验证：

&#42;.workfront.com

&#42;proofhq.com URL仍然是必需的。

有关更新允许列表的详细信息，请参阅[配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

>[!NOTE]
>
>此更新仅适用于Workfront中的校对；在使用Workfront Proof独立应用程序时，此更新不适用。

## 更新了Workfront Cookie行为以保持与Chrome的兼容性

为了与即将发布的Google Chrome更新(Chrome v80)保持兼容性，我们已更新Workfront平台以确保随请求正确发送Cookie。

此Chrome更新将更改SameSite Cookie属性的默认值。 如果要测试Google Chrome更新后Workfront实例的行为方式，请调整Chrome中的标志，并启用以下选项：

* &quot;默认为Cookie设置SameSite&quot;
* “不具有SameSite的Cookie必须是安全的”

## Workfront注释同步到Jira

适用于Jira集成的Workfront现在将您的Workfront评论同步到Jira的原生评论流。

以前，您可以将评论从Jira同步到Workfront，但不能将评论从Workfront同步到Jira。

有关详细信息，请参阅[配置Adobe Workfront for Jira](../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)。

## 删除了FlashPortfolio优化器

我们删除了适用于所有客户的Workfront ClassicPortfolio中的新旧版(基于Flash)Optimizer之间的切换功能。 旧版Portfolio优化器是一个已弃用的功能，现在新的工具可提供相同的功能。

有关项目组合优化器的信息，请参阅https://experience.workfront.com/s/article/Understanding-the-Portfolio-Optimizer-356650079

有关在Workfront中弃用基于Flash的工具的信息，请参阅[在Adobe Workfront中替换基于Flash的工具](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md)。
