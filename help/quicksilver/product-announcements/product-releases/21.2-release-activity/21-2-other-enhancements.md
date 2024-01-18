---
content-type: release-notes
keywords: 注释，季度，更新，版本
navigation-topic: 2021-2-release-activity
title: 21.2其他增强功能
description: 本页介绍了在21.2版本中对“预览”环境进行的所有其他增强功能。 这些增强功能将在2021年5月10日这一周的“生产”环境中提供。 有关21.2版本中可用的所有更改列表，请参阅21.2版本概述。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f136c08b-63c0-4e1e-a048-09eb84a0ed54
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# 21.2其他增强功能

本页介绍了在21.2版本中对“预览”环境进行的所有其他增强功能。 这些增强功能将在2021年5月10日这一周的“生产”环境中提供。 有关21.2版本可用的所有更改列表，请参阅 [21.2发行版概述](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## 我们现在正式命名为Adobe Workfront

Workfront已更名为Adobe Workfront。

Adobe Workfront应用程序和面向客户的网站中最突出的领域现已更新。 其他区域将很快更新。

**更新的区域**

* 登录屏幕、顶部导航、校对
* 布局模板UI、主菜单、自定义Forms导出(仅在新的Adobe Workfront Experience中可用)
* Workfront移动设备应用程序(iOS和Android)

区域即将更新

* 适用于桌面和移动设备的校对应用程序
* 列表和报告的PDF导出
* 浏览器选项卡中的Favicon图标

**区域稍后更新**

* 电子邮件通知

## 电子邮件允许列表验证

>[!NOTE]
>
>仅在新的Adobe Workfront Experience中可用。

如果您使用电子邮件允许列表，则新用户和更新后的用户电子邮件地址现在将根据允许列表进行验证。 当添加新用户或编辑现有用户并输入不在允许列表上的电子邮件域时，将会出现一条消息，通知您该用户不会收到电子邮件。 您仍然可以保存用户配置文件，但您应该将域添加到允许列表，以便用户接收电子邮件。

有关更多信息，请参阅 [编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 对象标题的新外观

>[!NOTE]
>
>此功能已于2020年3月10日发布到生产环境。
>
>此功能仅在新的Adobe Workfront Experience中可用。

为了进一步加强信息的层次结构并帮助用户更清楚地了解他们所在的页面，每个对象标题现在具有：

* 每种对象类型都有色彩鲜艳的现代图标
* 对象名称上方列出的对象类型
* 更新的字体样式和文本大小
* 其他次要样式更改

以前，没有图标，并且对象标题右侧会显示带有对象名称的徽章。

新Workfront体验中各个区域（例如增强型分析、资源管理等）的页面标题也具有这种更新的外观。

要详细了解新Workfront Experience中的新对象标头，请参阅 [新建对象标题](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

![](assets/product-announcement-object-header-350x179.png)

## 对象状态搜索响应的更新

Workfront现在以新的方式存储对象状态。

这些更改不会影响发出状态搜索请求的方式。 但是，包含对象状态搜索的API请求将返回不完整的组状态列表。

有关更多信息，请参阅 [核心API更改：状态搜索响应](../../../wf-api/api/api-changes-search.md) .

## 更新了事件订阅有效负荷，以包含所有以ID结尾的字段

现在，所有事件订阅负载都包含以“ID”结尾的每个字段。

请务必注意，每个对象都有其自己唯一的关联字段集，其中包括以ID结尾的唯一关联字段集。 这意味着，虽然每个有效负载都包含该对象的所有以ID结尾的关联字段，但每个对象都有一组以ID结尾的不同字段。

## Blueprint测试版现在可在预览版中使用

>[!NOTE]
>
>在21.3版本（今年晚些时候）发布之前，此功能将不在“生产”环境中正式可用。 仅在新的Adobe Workfront Experience中可用。

Blueprint提供了基本构建块，帮助您创建随增长而增长的工作管理系统。 系统管理员可以浏览Blueprint目录并安装现成的项目模板。

有关更多信息，请参阅 [Blueprint](../../../administration-and-setup/blueprints/blueprints.md).
