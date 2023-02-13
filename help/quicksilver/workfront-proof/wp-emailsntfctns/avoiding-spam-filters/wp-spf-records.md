---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront校样SPF记录
description: Workfront Proof从Workfront Proof电子邮件地址(如notification@proofing.yourdomain.com)向审阅人发送电子邮件通知。 为确保收件人的邮件服务器信任所有Workfront Proof电子邮件通知，您需要设置 [!DNL Sender Policy] Framework(SPF)记录，用于连接到 [!DNL Workfront Proof] 帐户（例如poofing.yourdomain.com）。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Workfront校样SPF记录

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] 通过向审阅人发送电子邮件通知 [!DNL Workfront Proof] 电子邮件地址，如notification@proofing.yourdomain.com。 为了确保收件人的邮件服务器信任所有 [!DNL Workfront Proof] 电子邮件通知，您需要设置 [!UICONTROL 发件人策略框架] (SPF)记录，用于连接到 [!DNL Workfront Proof] 帐户(例如， **poofing.yourdomain.com**)。

要设置SPF记录，您需要包含用于主域的SPF记录。

1. 添加 **[!UICONTROL DNS TXT]** 的条目，其中包含以下值：

   `v=spf1 a:mx.proofhq.com -all`

   您的电子邮件管理员或IT人员可以帮助您进行设置。

   >[!TIP]
   >
   >您可以在 [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) 查看 [!DNL Workfront] SPF记录。
