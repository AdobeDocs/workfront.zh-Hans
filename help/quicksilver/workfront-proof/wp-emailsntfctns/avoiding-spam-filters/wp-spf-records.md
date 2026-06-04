---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront Proof SPF记录
description: Workfront Proof会通过Workfront Proof电子邮件地址（如notification@proofing.yourdomain.com）向审阅人发送电子邮件通知。 为了确保收件人的邮件服务器信任所有Workfront Proof电子邮件通知，您需要为连接到 [!DNL Workfront Proof] 帐户的自定义域设置 [!DNL Sender Policy] Framework (SPF)记录（例如，proofing.yourdomain.com）。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
TQID: https://experienceleague.adobe.com/LTZzs99Zzsn5dbOlu4wP1coyJAMDnnCZZ1pTTbEjT24
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 181
ht-degree: 0%

---

# Workfront Proof SPF记录

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

[!DNL Workfront Proof]通过[!DNL Workfront Proof]电子邮件地址（如notification@proofing.yourdomain.com）向审阅人发送电子邮件通知。 为了确保收件人的邮件服务器信任所有[!DNL Workfront Proof]电子邮件通知，您需要为连接到[!DNL Workfront Proof]帐户的自定义域设置[!UICONTROL 发件人策略框架] (SPF)记录（例如，**proofing.yourdomain.com**）。

要设置SPF记录，您需要包含用于主域的SPF记录。

1. 使用下列值为您的域添加&#x200B;**[!UICONTROL DNS TXT]**&#x200B;条目：

   `v=spf1 a:mx.proofhq.com -all`

   您的电子邮件管理员或IT人员可以帮助您进行此设置。

   >[!TIP]
   >
   >您可以在[[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx)处使用免费工具查看[!DNL Workfront] SPF记录。
