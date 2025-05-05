---
content-type: reference
navigation-topic: announcements
title: 电子邮件欺骗和POP回复删除
description: 我们对Adobe Workfront 20.3版（计划于2020年8月发布）中发送和接收电子邮件的方式做出了两项更改。
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# 电子邮件欺骗和POP回复

我们对Adobe Workfront 20.3版（计划于2020年8月发布）中发送和接收电子邮件的方式做出了两项更改。

## 来自Workfront的出站电子邮件

为了提高电子邮件的成功投放，我们将消除通常标记为垃圾邮件的电子邮件欺骗（请参阅电子邮件欺骗）。 来自Workfront的所有电子邮件都将从`notifications@my.workfront.com`发送，包括自动警报和用户到用户的通信。 Joan Harris的示例电子邮件在电子邮件的“发件人”区域中如下所示：

![示例电子邮件](assets/noreply.png)

*我们强烈建议您联系您的IT团队*，以确保不会阻止来自`notifications@my.workfront.com`的电子邮件，从而接收系统发送的电子邮件。 您还可以参考[配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)，了解有关流量和电子邮件来自哪些IP地址的详细信息。

## 通知的入站电子邮件回复（POP回复）

某些电子邮件通知允许用户通过电子邮件回复，并将回复作为评论回复复制到Workfront的Workfront系统中。 传统上，Workfront中的系统管理员既可以选择提供自己的POP电子邮件服务器来接收这些回复，也可以使用内置的Workfront回复系统。 自定义POP电子邮件服务器选择将在20.3版本中删除。 配置为使用自定义服务器的所有帐户将自动转换为使用本机Workfront电子邮件回复系统。 系统管理员或其他Workfront用户无需执行任何操作。

直接来自Workfront Proof系统的电子邮件不会发生变化。 您将继续像过去一样接收这些电子邮件。

如果您有任何其他问题或顾虑，请联系[Workfront支持团队](https://experienceleague.adobe.com/zh-hans?support-tab=home#support)。
