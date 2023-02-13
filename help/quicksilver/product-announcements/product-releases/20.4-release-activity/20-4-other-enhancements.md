---
title: 20.4其他增强功能
description: 20.4其他增强功能
author: Luke
draft: Probably
feature: Product Announcements
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# 20.4其他增强功能

本页介绍20.4版本到“预览”环境的所有其他增强功能。 这些增强功能将于2020年11月9日这一周的生产环境中提供。

有关20.4版本中可用的所有更改的列表，请参阅 [20.4版本概述](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## 管理员的新增功能：切换Workfront环境选项可用

为了获得更高效、更便捷的体验，组管理员和Workfront管理员现在可以在Workfront中任意页面的不同Workfront环境之间快速切换，而无需注销。

在新的Workfront体验中，主菜单中会显示选项“切换到经典”。

在Workfront Classic中，单击全局导航栏右上角的配置文件图片时，显示的菜单中会显示切换到新体验选项。

此功能现在包含在 [管理员基础知识，第1部分学习路径](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) Workfront一号。

## 改进了Workfront校样的加密

我们正在进行一些更改，以提高Workfront校样应用程序的动态数据加密的强度。 弱TLS加密将于2020年11月11日被弃用。

请确保您在访问Workfront时使用受支持的浏览器。 有关支持的浏览器的更多信息，请参阅 [Adobe Workfront浏览器要求](../../../workfront-basics/workfront-browser-requirements.md).

## 3个电子邮件模板的新外观

为了提高可读性和整体体验，以下电子邮件模板具有全新的外观：

* 新工作请求
* 您分配到的从属任务现已准备就绪，可以开始
* 具有上一任结束的团队电子邮件通知

要在预览环境中为测试目的启用电子邮件，请参阅 [激活或停用您自己的事件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## 适用于团队的新电子邮件通知

我们为团队添加了以下电子邮件通知：

* 分配给我团队的任务的前置任务已完成：当其任务的前任标记为完成时，分配的团队会收到电子邮件通知。
* 分配给我团队的任务的所有前任都已完成：所分配的团队会收到每个标记为完成的前任的电子邮件通知。

有关更多信息，请参阅 [通知：关于分配给我的工作的信息](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## 管理员的新增功能：电子邮件通知增强功能

现在，只需单击一次，即可在“设置”中启用或禁用事件电子邮件通知。 只需单击通知名称旁边的开/关开关。

此外，请注意我们的现代样式，现在改进了“电子邮件通知”区域中配置事件通知的体验。

有关配置电子邮件通知的信息，请参阅 [为系统中的每个人配置事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

此功能现在包含在 [电子邮件和应用程序内通知学习路径](https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-20Y4X000000CaZGUA0) Workfront一号。

## 可触发事件订阅更新的新API对象

创建了两个新的API对象（documentVersion和proofApproval），并将其配置为在文档版本控制或批准时触发事件订阅更新。

有关与每个对象关联的字段的完整列表，请参阅 [事件订阅资源字段](../../../wf-api/api/event-sub-resource-fields.md).
