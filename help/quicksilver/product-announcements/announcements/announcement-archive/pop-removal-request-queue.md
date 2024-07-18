---
content-type: reference
navigation-topic: announcements
title: 新的Adobe Workfront托管系统使用21.1替换了请求队列的POP电子邮件
description: 我们正在将请求队列的POP电子邮件选项替换为新的Adobe Workfront托管系统。 您仍可以通过电子邮件提交请求，但您需要在“请求队列”区域中设置一个新的Workfront托管电子邮件地址。
author: Luke
feature: Product Announcements
exl-id: d7147641-ba36-422b-a9b2-3c2f4ab609d8
source-git-commit: f05b462ff596ccc19215ca684802a9820a98211a
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# 新的Adobe Workfront托管系统使用21.1替换了请求队列的POP电子邮件

我们正在将请求队列的POP电子邮件选项替换为新的Adobe Workfront托管系统。 您仍可以通过电子邮件提交请求，但您需要在“请求队列”区域中设置一个新的Workfront托管电子邮件地址。

## 为什么要删除POP电子邮件选项？

POP技术是一种不可靠且不太安全的电子邮件选项。 此外，我们看到许多与POP电子邮件相关的客户问题。 更改为Workfront托管系统将提供更可靠的体验。

## 我需要执行什么操作？

您需要为生产环境中使用POP电子邮件设置的每个请求队列设置一个新的电子邮件地址，并根据需要分发新的电子邮件地址。 有关详细信息，请参阅[允许用户通过电子邮件将问题发送到请求队列项目](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md)。

## 过渡计划是什么？

从2月初的21.1版本开始，您有60天的时间将用户转移到您创建的新&#x200B;*@intake.workfront.com*&#x200B;电子邮件地址。 在60天内，以前使用的POP电子邮件将继续工作。

## 如何在“预览”中测试此设置？

要在预览中测试此更改，您需要在预览环境中启用电子邮件。 为此，请按照[从预览Sandbox环境启用电子邮件投放](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)中在预览中管理电子邮件一节中的说明进行操作。

>[!IMPORTANT]
>
>您在此处设置的内容不会转移到您的生产环境中。 将功能发布到生产环境后，您需要再次执行此过程。
