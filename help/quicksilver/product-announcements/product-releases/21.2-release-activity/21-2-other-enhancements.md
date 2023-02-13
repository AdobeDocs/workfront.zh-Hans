---
content-type: release-notes
keywords: 注释，季度，更新，发行
navigation-topic: 2021-2-release-activity
title: 21.2其他增强功能
description: 本页介绍了在“预览”环境的21.2版本中所做的所有其他增强。 这些增强功能将于2021年5月10日这一周的生产环境中提供。 有关21.2版本中可用的所有更改的列表，请参阅21.2版本概述。
author: Luke
feature: Product Announcements
exl-id: f136c08b-63c0-4e1e-a048-09eb84a0ed54
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 21.2其他增强功能

本页介绍了在“预览”环境的21.2版本中所做的所有其他增强。 这些增强功能将于2021年5月10日这一周的生产环境中提供。 有关21.2版本中可用的所有更改的列表，请参阅 [21.2版本概述](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## 我们现在是正式的Adobe Workfront

Workfront已更名为Adobe Workfront。

Adobe Workfront应用程序和面向客户的网站中最突出的部分现已更新。 其他方面将很快更新。

**更新的区域**

* 登录屏幕、顶部导航、校样
* 布局模板UI、主菜单、自定义Forms导出(仅在新的Adobe Workfront体验中可用)
* Workfront移动设备应用程序(iOS和Android)

区域即将更新

* 为桌面和移动设备的应用程序校样
* PDF导出列表和报表
* 浏览器选项卡中的收藏夹图标

**区域稍后更新**

* 电子邮件通知

## 电子邮件允许列表验证

>[!NOTE]
>
>仅在新的Adobe Workfront体验中可用。

如果您使用电子邮件允许列表，则系统现在会根据该验证新用户和更新用户电子邮件地址允许列表。 当您添加新用户或编辑现有用户，并输入未在中的电子邮件域允许列表时，系统会显示一条消息，通知您用户将不会收到电子邮件。 您仍可以保存用户配置文件，但应将域添加到允许列表中，以便用户收到电子邮件。

有关更多信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 对象标头的新外观

>[!NOTE]
>
>此功能于2020年3月10日发布到生产环境。
>
>此功能仅在新的Adobe Workfront体验中可用。

为了进一步强化信息的层次结构并帮助用户更清楚地了解他们所在的页面，每个对象标头现在都具有：

* 每种对象类型的彩色、更现代的图标
* 对象名称上方列出的对象类型
* 更新的字体样式和文本大小
* 其他次要样式更改

以前，对象标题的右侧没有显示任何图标和具有对象名称的徽章。

新Workfront体验（如增强的分析、资源管理和其他体验）中区域的页眉也具有这种更新的外观。

要了解有关新Workfront体验中新对象标头的更多信息，请参阅 [新对象标头](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

![](assets/product-announcement-object-header-350x179.png)

## 对象状态搜索响应的更新

Workfront现在以新方式存储对象状态。

这些更改不会影响发出状态搜索请求的方式。 但是，包含对象状态搜索的API请求将返回组状态列表不完整。

有关更多信息，请参阅 [核心API更改：状态搜索响应](../../../wf-api/api/api-changes-search.md) .

## 更新了事件订阅负载，以包含以ID结尾的所有字段

现在，所有事件订阅负载都包含以“ID”结尾的每个字段。

请务必注意，每个对象都有其自己唯一的关联字段集，其中包含以ID结尾的一组唯一的关联字段。 这意味着，尽管每个有效负载包含该对象以ID结尾的所有关联字段，但每个对象具有以ID结尾的不同字段集。

## Blueprint测试版现已在“预览”中提供

>[!NOTE]
>
>在今年晚些时候发布的21.3版本之前，此功能通常不会在生产环境中提供。 仅在新的Adobe Workfront体验中可用。

Blueprint提供基本的构建基块，帮助您创建一个随您一起扩展的工作管理系统。 系统管理员可以浏览Blueprint目录并安装现成的项目模板。

有关更多信息，请参阅 [蓝图](../../../administration-and-setup/blueprints/blueprints.md).
