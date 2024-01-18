---
title: 20.4其他增强功能
description: 20.4其他增强功能
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# 20.4其他增强功能

本页介绍了20.4版本对“预览”环境所做的所有其他增强。 这些增强功能将在2020年11月9日这一周的“生产”环境中提供。

有关20.4版本可用的所有更改列表，请参阅 [20.4版本概述](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## 管理员的新增功能：切换Workfront环境选项可用

为了获得更高效且更便捷的体验，组管理员和Workfront管理员现在可以从Workfront中的任何页面快速在不同的Workfront环境之间切换，而无需注销。

在新的Workfront Experience中，主菜单中会显示切换到经典选项。

在Workfront Classic中，切换到新体验选项显示在单击全局导航栏右上角的配置文件图片时显示的菜单中。

此功能现已包含在 [管理员基础知识，第1部分学习路径](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) 在Workfront一号。

## 改进了Workfront Proof的加密

我们正在进行一些更改，以提高Workfront校对应用程序的数据移动加密强度。 弱的TLS密码将于2020年11月11日弃用。

访问Workfront时，请确保您使用支持的浏览器。 有关支持的浏览器的更多信息，请参阅 [Adobe Workfront浏览器要求](../../../workfront-basics/workfront-browser-requirements.md).

## 3个电子邮件模板的新外观

为了提高可读性和整体体验，以下电子邮件模板具有新外观：

* 新工作请求
* 您分配到的一个依赖任务现已准备开始
* 具有前置任务完成的团队电子邮件通知

要在预览环境中启用电子邮件进行测试，请参阅中的在预览中管理电子邮件部分 [修改您自己的电子邮件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## 团队的新电子邮件通知

我们为团队添加了以下电子邮件通知：

* 分配给我团队的某个任务的前置任务已完成：当其某个任务的前置任务被标记为完成时，被分配的团队会收到电子邮件通知。
* 已完成分配到我团队中任务的所有前置任务：被分配的团队会收到每个标记为完成前置任务的电子邮件通知。

有关更多信息，请参阅 [通知：有关分配给我的工作的信息](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## 管理员的新增功能：电子邮件通知增强功能

现在，只需单击一下，即可在“设置”中启用或禁用事件电子邮件通知。 只需单击通知名称旁边的打开/关闭开关。

此外，请注意我们的现代样式现在改进了电子邮件通知区域中配置事件通知的体验。

有关配置电子邮件通知的信息，请参阅 [为系统中的每个人配置事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

此功能现已包含在 [电子邮件和应用内通知学习路径](https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-20Y4X000000CaZGUA0) 在Workfront一号。

## 触发事件订阅更新的新API对象

创建了两个新的API对象documentVersion和proofApproval，并将其配置为在文档进行版本控制或审批时触发事件订阅更新。

有关与每个对象关联的字段的完整列表，请参阅 [事件订阅资源字段](../../../wf-api/api/event-sub-resource-fields.md).
