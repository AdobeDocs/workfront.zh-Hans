---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: 配置 [!DNL Workfront Proof] 电子邮件以避免垃圾邮件过滤器
description: “您的电子邮件客户端的垃圾邮件过滤器有一个重要用途：保护您免受恼人的和可能的恶意垃圾邮件电子邮件的侵扰。 但是，如果垃圾邮件过滤器中的设置不正确，则可能会阻止您看到以下重要的 [!DNL Workfront Proof] 电子邮件：验证电子邮件通知、新闻通讯和特殊通信。”
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 配置[!DNL Workfront Proof]电子邮件以避免垃圾邮件过滤器

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

您的电子邮件客户端的垃圾邮件过滤器有一个重要用途：保护您免受恼人的和可能的恶意垃圾邮件电子邮件的侵扰。 但是，如果垃圾邮件过滤器中的设置不正确，则可能会阻止您看到以下重要的[!DNL Workfront Proof]电子邮件：验证电子邮件通知、新闻通讯和特殊通信。

列入允许列表为了确保您的[!DNL Workfront Proof]电子邮件始终被发送到您的收件箱而不是垃圾邮件文件夹，您应该将以下内容添加到中：

* [!DNL Workfront Proof]邮件服务器： **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot;电子邮件地址(例如，notification@proofhq.com)

有关要添加到允许列表的URL的详细信息，请参阅[配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)一文中的[配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

## [!DNL Workfront Proof] &quot;[!UICONTROL 来自]&quot;电子邮件地址

根据您的电子邮件客户端类型，您可能需要将[!DNL Workfront Proof]“[!UICONTROL from]”电子邮件地址添加到以下项之一，以防止垃圾邮件过滤器将来将您的电子邮件路由到您的垃圾邮件文件夹：

* 您的联系人列表
* 您的[!UICONTROL 安全发件人]列表
* 您创建的用于将这些地址的电子邮件传送到收件箱的过滤器

您可能还需要从垃圾邮件文件夹中删除任何现有的[!DNL Workfront Proof]电子邮件，并检查任何“[!UICONTROL 来自]”地址是否位于阻止的地址列表中。 此帮助页列出了[!DNL Workfront Proof] [!UICONTROL 来自]的地址，并显示了如何在以下电子邮件客户端中将它们添加到垃圾邮件过滤器：

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>如果您对此处描述的过程有任何疑问，请查看电子邮件客户端的帮助。

有关详细信息，请参阅[为常用电子邮件客户端配置垃圾邮件设置](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md)。

## 要复制的[!DNL Workfront Proof] &quot;[!UICONTROL from]&quot;电子邮件地址

为确保您的[!DNL Workfront Proof]电子邮件送达收件箱，您需要将两个[!DNL Workfront Proof]电子邮件地址分别添加到电子邮件客户端的垃圾邮件过滤器中：

* 一般支持地址[!DNL support@proofhq.com]，[!DNL Workfront Proof]从中发送许多电子邮件通信
* [!DNL Workfront Proof]发送校样通知电子邮件给校样创建者和审阅者的通知地址，其中包含校样链接。 这可能是常规地址、notification@support.proofhq.com，或者如果您具有自定义子域或白标签域，则可能是特定地址。

要将[!DNL Workfront Proof]个[!UICONTROL 来自]的地址添加到电子邮件客户端的过滤器，请执行以下操作：

1. 复制常规的[!DNL Workfront Proof]支持“[!UICONTROL 来自]”电子邮件地址(support@proofhq.com)，并将其粘贴到为电子邮件客户端指定的字段中。
1. 复制以下[!DNL Workfront Proof]个“[!UICONTROL 来自]”电子邮件地址中的相应一个，并将其单独粘贴到为电子邮件客户端指定的字段中：

   * notification@support.proofhq.com（如果您没有自定义子域或白标签域）
   * notification@yoursubdomain.proofhq.com（如果您有自定义的子域）；请在此地址中替换您的子域名
   * notification@yoursubdomain.yourdomain.com（如果您拥有白标签域）；请在此地址中替换您的子域名和域名

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
