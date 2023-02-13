---
content-type: reference
navigation-topic: announcements
title: 新的Adobe Workfront托管系统将请求队列的POP电子邮件替换为21.1
description: 我们正在将请求队列的POP电子邮件选项替换为新的Adobe Workfront管理系统。 您仍可以通过电子邮件提交请求，但是您需要在“请求队列”区域设置一个新的Workfront托管电子邮件地址。
author: Luke
feature: Product Announcements
exl-id: d7147641-ba36-422b-a9b2-3c2f4ab609d8
source-git-commit: f05b462ff596ccc19215ca684802a9820a98211a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# 新的Adobe Workfront托管系统将请求队列的POP电子邮件替换为21.1

我们正在将请求队列的POP电子邮件选项替换为新的Adobe Workfront管理系统。 您仍可以通过电子邮件提交请求，但是您需要在“请求队列”区域设置一个新的Workfront托管电子邮件地址。

## 为什么删除POP电子邮件选项？

POP技术是一种不可靠、不太安全的电子邮件选项。 此外，我们还看到许多与POP电子邮件有关的客户问题。 更改Workfront托管系统将获得更可靠的体验。

## 我需要采取什么操作？

您需要为您在生产环境中使用POP电子邮件设置的每个请求队列设置一个新电子邮件地址，并根据需要分发新的电子邮件地址。 有关更多信息，请参阅 [允许用户将问题通过电子邮件发送到请求队列项目](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## 什么是过渡计划？

从2月初的21.1版本开始，您将有60天时间将用户转换到新的 *@intake.workfront.com* 您创建的电子邮件地址。 在60天内，以前使用的POP电子邮件将继续有效。

## 如何在“预览”中测试此代码？

要在预览中测试此更改，您需要在预览环境中启用电子邮件。 为此，请按照 [允许从预览沙盒环境发送电子邮件](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!IMPORTANT]
>
>您在此处设置的内容将不会传递到生产环境。 在将功能发布到生产环境后，您需要再次完成此过程。
