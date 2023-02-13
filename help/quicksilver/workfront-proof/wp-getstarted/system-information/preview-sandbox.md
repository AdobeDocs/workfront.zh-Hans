---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: 预览沙盒测试环境 —  [!DNL Workfront Proof]
description: “预览沙盒”是一个测试环境，用作实时环境的副本，每周末由 [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# 预览沙盒测试环境 —  [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

“预览沙盒”是一个测试环境，用作实时环境的副本，每周末由 [!DNL Workfront Proof].

## 了解预览沙盒

“预览”沙盒用作一个环境，在该环境中，组织中的用户可以安全地测试和处理生产环境中的数据，而不会影响生产环境。 它非常适合运行培训课程、测试新功能以及确定设置功能。

此外，新产品功能在交付到生产环境之前会先上传到预览沙盒环境。 您的用户可以在此尝试新功能，而不会影响他们在生产环境中的常规工作流。

预览沙盒包含您的实际生产数据。 数据会从“生产”流向“预览”，而不是相反。 它会每个周末刷新一次，以便数据最多可能比生产环境滞后一周。 自上次刷新后创建的项目将在“预览沙盒”环境中，直到进行以下刷新。

## 访问预览沙盒

默认情况下，作为系统管理员，您有权访问预览沙盒环境。 如果您无法访问本节所述的“预览沙盒”环境，请与 [!DNL Workfront] 管理员或我们的支持团队。

* [独立访问预览沙盒 [!DNL Workfront Proof] 客户](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [访问预览沙盒作为 [!DNL Workfront]+[!DNL Workfront Proof] 客户](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### 独立访问预览沙盒 [!DNL Workfront Proof] 客户

1. 导航到以下URL:  `https://preview.proofhq.com`.
1. 使用预览凭据登录。\
   除非在发生预览刷新后在生产中更改了这些凭据，否则您的预览凭据应该与生产凭据相同。 仅当每周末都发生刷新时，才会同步登录。 它们不会自动同步。

### 访问预览沙盒作为 [!DNL Workfront+Workfront] 验证客户

作为系统管理员，您可以 [!DNL Workfront Proof] 通过预览沙盒 [!DNL Workfront] 界面。

访问 [!DNL Workfront Proof] 预览沙盒：

1. 登录到 [!DNL Workfront] 环境。
1. 单击 **[!UICONTROL 设置]** 中。
1. 单击 **[!UICONTROL 系统]** >**[!UICONTROL 首选项]**.

1. 在 **[!UICONTROL 测试环境]** ，单击 **[!UICONTROL 沙盒预览]**.

1. 使用预览凭据登录。\
   除非在发生预览刷新后在生产中更改了这些凭据，否则您的预览凭据应与生产凭据相同。 仅当发生刷新时才会同步登录。 它们不会自动同步。
1. 单击 [!DNL Workfront Proof] 图标。\
   ![proof_access_proofhq.png](assets/proof-access-proofhq-350x39.png)\
   的 [!DNL Workfront Proof] 此时会显示预览环境。

## 从预览沙盒接收电子邮件

电子邮件通知从未从 [!DNL Workfront Proof] 预览环境。
