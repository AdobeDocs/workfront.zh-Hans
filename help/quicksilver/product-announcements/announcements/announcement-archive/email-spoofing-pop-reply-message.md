---
content-type: reference
navigation-topic: announcements
title: 删除电子邮件欺骗和POP回复
description: 在20.3版本（定于2020年8月）中，我们将对Adobe Workfront发送和接收电子邮件的方式进行两项更改。
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# 电子邮件欺骗和POP回复

在20.3版本（定于2020年8月）中，我们将对Adobe Workfront发送和接收电子邮件的方式进行两项更改。

## 来自Workfront的出站电子邮件

为了增加电子邮件的成功发送，我们将消除电子邮件欺骗，该电子邮件通常标记为垃圾邮件（请参阅电子邮件欺骗）。 所有来自Workfront的电子邮件都将从notifications@my.workfront.com发送，其中包括自动警报和用户与用户的通信。 Joan Harris发送的示例电子邮件在电子邮件的发件人区域中如下所示：

![](assets/noreply.png)

*我们强烈建议您联系您的IT团队* 以确保系统中传入电子邮件不会阻止来自notifications@my.workfront.com的电子邮件。 您还可以引用 [配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) 有关流量和电子邮件来源的IP地址的详细信息。

## 对通知的入站电子邮件回复（POP回复）

某些电子邮件通知允许用户通过电子邮件回复，并让回复作为评论回复复制到Workfront中的Workfront系统。 Workfront的系统管理员传统上能够选择提供自己的POP电子邮件服务器以接收这些回复，还是使用内置的Workfront回复系统。 在20.3版本中，将删除自定义POP电子邮件服务器选项。 配置为使用自定义服务器的所有帐户将自动转换为使用本机Workfront电子邮件回复系统。 系统管理员或其他Workfront用户无需执行任何操作。

对于直接从Workfront校样系统发送的电子邮件，不会发生任何更改。 您将继续像过去一样收到这些电子邮件。

如果您有其他问题或疑问，请联系 [Workfront支持团队](https://one.workfront.com/s/support?language=en_US).
