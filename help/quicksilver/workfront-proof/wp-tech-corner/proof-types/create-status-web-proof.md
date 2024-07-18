---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: 使用 [!DNL Workfront Proof]创建静态网站校对
description: 您可以从网页创建静态校样。 此外，您还可以通过定义捕获的屏幕分辨率来模拟各种设备。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# 使用[!DNL Workfront Proof]创建静态网站校对

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

您可以从网页创建静态校样。 此外，您还可以通过定义捕获的屏幕分辨率来模拟各种设备。

## 创建静态网站验证

1. 打开[!UICONTROL 新校对]页面，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中生成校对中所述。
1. 在&#x200B;**www.shareyourlink.com**&#x200B;框中粘贴或键入您的URL。
1. 您可以重复此步骤以添加多个URL。
1. 在此框的正下方，单击分辨率（默认值为1366x768），然后在&#x200B;**[!UICONTROL 屏幕分辨率]**框中选择所需的任何分辨率。
如果要验证移动设备的设计，请选择较小的分辨率。 通常，会根据屏幕/浏览器窗口分辨率来设计加载。

1. 如果要包含与输入的URL位于同一域/子域的已连接页面，请单击&#x200B;**[!UICONTROL 查找子页面]**。
   [!DNL Workfront Proof]扫描连接的页面，并在&#x200B;**[!UICONTROL 查找子页面]**&#x200B;选项下方列出这些页面。 您可以选择要包含的页面。

1. 通过[!UICONTROL 合并校样]功能，您可以将所有网页作为单个多页校样提交。
1. 单击&#x200B;**[!UICONTROL 完成]**，然后按照[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中生成校对中的说明完成配置校对。

## 关于受密码保护的页面和需要授权的页面

[!DNL Workfront Proof]无法捕获受密码保护的网站作为静态校对。

列入允许列表为了从需要授权的页面创建验证，您的IT团队必须将以下URL之一添加到贵公司的URL中，我们的Web捕获工具可通过该URL进行连接：

美国&#x200B;**AWS群集**： webcapture.proofhq.com

美国&#x200B;**GCP群集**： webcapture.gcp.proofhq.com

**EMEA集群**： webcapture.proofhq.eu

>[!NOTE]
>
>对于需要授权且受密码保护的网站的内部页面，我们建议使用交互式校对，而不是静态校对。 有关详细信息，请参阅[交互式内容校对概述](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md)。

## 关于处理静态网站验证

* 动画、嵌入视频、脚本和交互不能包含在静态网站验证中。 如果要验证交互式内容，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中生成验证中的[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中生成验证。

* 验证页面通常以每页约20秒的速率捕获并准备。 但是，总体准备时间还取决于托管页面的服务器。 该工具会等待60秒才加载每个提交的URL。 如果超过此等待时间，验证将失败。
* 对于组合验证，如果任何URL未响应捕获工具，则验证失败。
* 在栅格化之后，[!DNL Workfront Proof]捕获长达195英寸的网页。 如果网页长度超过此长度，则验证失败。
* 文本提取适用于所有文本元素，但置为图像的文本不会提取。
* 可以在验证上单击文本超链接，链接的页面将在新的浏览器选项卡中打开。
* 如果在`<a>`标记内使用了style=&quot;display：block&quot;元素，则图像上的超链接不可点击。 我们建议调整页面设计的这些部分。
* 为获得最佳结果，我们建议使用最佳编码实践和公认的标准来创建页面。
