---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: 预览沙盒测试环境 —  [!DNL Workfront Proof]
description: 预览沙盒是一个测试环境，用作实时环境的副本，每个周末由 [!DNL Workfront Proof]刷新。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# 预览沙盒测试环境 — [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

预览沙盒是一个测试环境，用作实时环境的副本，每个周末由[!DNL Workfront Proof]刷新。

## 了解“预览Sandbox”

预览Sandbox用作一种环境，贵组织中的用户可以在其中安全地测试和处理生产环境中的数据，而不会影响生产环境。 它非常适合于运行培训课程、测试新功能和确定设置功能。

此外，新产品功能在交付到生产环境之前，会先上传到预览沙盒环境。 您的用户可以在那里试用新功能，而不会影响他们在生产环境中的正常工作流程。

预览沙盒包含您的实际生产数据。 数据会从生产环境流向预览环境，而不是反向流动。 它每周末都会刷新，因此数据最多可以为生产环境滞后一周。 在上次刷新后创建的项目会一直位于预览沙盒环境中，直到下次刷新为止。

## 访问预览沙盒

默认情况下，作为系统管理员，您有权访问预览沙盒环境。 如果您无法按本节所述访问“预览沙盒”环境，请联系您的[!DNL Workfront]管理员或我们的支持团队。

* [以独立 [!DNL Workfront Proof] 客户身份访问预览沙盒](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [以 [!DNL Workfront]+[!DNL Workfront Proof] 客户身份访问预览沙盒](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### 以独立[!DNL Workfront Proof]客户身份访问预览沙盒

1. 导航到此URL： `https://preview.proofhq.com`。
1. 使用预览凭据登录。\
   您的预览凭据应与生产凭据相同，除非您在发生预览刷新后在生产环境中更改了这些凭据。 只有在每周末进行刷新时，才会同步登录。 它们不会自动同步。

### 以[!DNL Workfront+Workfront]验证客户身份访问预览沙盒

作为系统管理员，您可以通过[!DNL Workfront]界面访问[!DNL Workfront Proof]预览沙盒。

要访问[!DNL Workfront Proof]预览沙盒，请执行以下操作：

1. 登录到您的[!DNL Workfront]环境。
1. 单击全局导航栏中的&#x200B;**[!UICONTROL 设置]**。
1. 单击&#x200B;**[!UICONTROL 系统]** >**[!UICONTROL 首选项]**。

1. 在&#x200B;**[!UICONTROL 测试环境]**&#x200B;分区中，单击&#x200B;**[!UICONTROL 沙盒预览]**。

1. 使用预览凭据登录。\
   您的预览凭据应与生产凭据相同，除非您在预览刷新后在生产环境中更改了这些凭据。 只有在刷新时才会同步登录。 它们不会自动同步。
1. 单击全局导航栏中的[!DNL Workfront Proof]图标。\
   ![proof_access_proofhq.png](assets/proof-access-proofhq-350x39.png)\
   显示[!DNL Workfront Proof]预览环境。

## 从预览Sandbox接收电子邮件

绝不会从[!DNL Workfront Proof]预览环境中触发电子邮件通知。
