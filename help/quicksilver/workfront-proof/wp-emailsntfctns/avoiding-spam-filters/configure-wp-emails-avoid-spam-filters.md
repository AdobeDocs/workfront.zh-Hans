---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: 配置 [!DNL Workfront Proof] 电子邮件以避免垃圾邮件过滤器
description: “电子邮件客户端的垃圾邮件过滤器具有重要用途：保护您免受烦人且可能有恶意的垃圾邮件的侵害。 但是，如果您在垃圾邮件过滤器中没有正确的设置，则可能会阻止您看到以下重要信息 [!DNL Workfront Proof] 电子邮件：校样电子邮件通知、新闻稿和特殊通信。”
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 配置 [!DNL Workfront Proof] 电子邮件以避免垃圾邮件过滤器

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

电子邮件客户端的垃圾邮件过滤器具有重要用途：保护您免受烦人且可能有恶意的垃圾邮件的侵害。 但是，如果您在垃圾邮件过滤器中没有正确的设置，则可能会阻止您看到以下重要信息 [!DNL Workfront Proof] 电子邮件：校样电子邮件通知、新闻稿和特殊通信。

确保您的 [!DNL Workfront Proof] 电子邮件始终会发送到您的收件箱而不是垃圾邮件文件夹，您应将以下内容添加到允许列表:

* [!DNL Workfront Proof] 邮件服务器： **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL 从]“电子邮件地址(例如notification@proofhq.com)

有关要添加到的URL的更多信允许列表息，请参阅 [配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) 在文章中 [配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] &quot;[!UICONTROL 从]“电子邮件地址”

根据您的电子邮件客户端类型，您可能需要添加 [!DNL Workfront Proof] &quot;[!UICONTROL 从]“电子邮件地址”，用于阻止垃圾邮件过滤器将来将电子邮件路由到您的垃圾邮件文件夹：

* 您的联系人列表
* 您的 [!UICONTROL 安全发件人] 列表
* 您创建的过滤器，用于将电子邮件从这些地址发送到您的收件箱

您可能还需要删除任何现有的 [!DNL Workfront Proof] 从垃圾邮件文件夹发送电子邮件，并检查是否有“[!UICONTROL 从]“地址位于阻止的地址列表上。 此帮助页面列出了 [!DNL Workfront Proof] &quot;[!UICONTROL 从]“地址并显示如何将这些地址添加到以下电子邮件客户端中的垃圾邮件过滤器：

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>如果您对此处介绍的过程有任何疑问，请查看电子邮件客户的帮助。

有关更多信息，请参阅 [为常用电子邮件客户端配置垃圾邮件设置](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## 的 [!DNL Workfront Proof] &quot;[!UICONTROL 从]“复制电子邮件地址”

确保您的 [!DNL Workfront Proof] 电子邮件到达您的收件箱，您需要添加两个 [!DNL Workfront Proof] 电子邮件地址会单独添加到电子邮件客户端的垃圾邮件过滤器：

* 一般支持地址， [!DNL support@proofhq.com]，从中 [!DNL Workfront Proof] 发送许多电子邮件通信
* 通知地址，其中 [!DNL Workfront Proof] 向校样创建者和具有校样链接的审阅者发送校样通知电子邮件。 如果您拥有自定义的子域或白标签域，则这可以是常规地址、notification@support.proofhq.com或特定地址。

添加 [!DNL Workfront Proof] &quot;[!UICONTROL 从]“电子邮件客户端过滤器的地址：

1. 复制常规 [!DNL Workfront Proof] 支持&quot;[!UICONTROL 从]“电子邮件地址(support@proofhq.com)，并将其粘贴到为电子邮件客户端指示的字段中。
1. 复制以下任一项 [!DNL Workfront Proof] &quot;[!UICONTROL 从]“电子邮件地址并单独将其粘贴到为您的电子邮件客户端指定的字段中：

   * notification@support.proofhq.com如果您没有自定义的子域或白标签域
   * notification@yoursubdomain.proofhq.com（如果您有自定义的子域）；用此地址替换子域名
   * notification@yoursubdomain.yourdomain.com（如果您有白色标签域）；将您的子域名替换为此地址中的域名

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
