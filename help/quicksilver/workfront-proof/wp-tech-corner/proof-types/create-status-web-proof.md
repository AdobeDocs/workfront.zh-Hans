---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: 使用创建静态网站校样 [!DNL Workfront Proof]
description: 您可以从网页创建静态校样。 此外，您还可以通过定义捕获的屏幕分辨率来模拟各种设备。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# 使用创建静态网站校样 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

您可以从网页创建静态校样。 此外，您还可以通过定义捕获的屏幕分辨率来模拟各种设备。

## 创建静态网站校样

1. 打开 [!UICONTROL 新校样] 页面，如 [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).
1. 在 **www.shareyourlink.com** 框中。
1. 您可以重复此步骤以添加多个URL。
1. 在此框的正下方，单击分辨率（默认为1366x768），然后选择您希望在 **[!UICONTROL 屏幕分辨率]** 框中。
如果要校样移动设备的设计，请选择较小的分辨率。 通常，设计会根据屏幕/浏览器窗口分辨率加载。

1. 单击 **[!UICONTROL 查找子页面]** 如果要包含与输入的URL位于同一域/子域的已连接页面，请执行以下操作：
   [!DNL Workfront Proof] 扫描连接的页面，并在 **[!UICONTROL 查找子页面]** 选项。 您可以选择要包含的页面。

1. 使用 [!UICONTROL 合并校样] 功能，您可以将所有网页作为单页多页校样提交。
1. 单击 **[!UICONTROL 完成]**，然后按照 [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## 关于受密码保护的页面和需要授权的页面

[!DNL Workfront Proof] 无法捕获受密码保护的网站作为静态校样。

为了从需要授权的页面创建校样，您的IT团队必须将以下URL之一添加到您公司的中，我们的Web捕允许列表获工具可通过该URL进行连接：

**AWS聚集在美国**:webcapture.proofhq.com

**美国GCP集群**:webcapture.gcp.proofhq.com

**EMEA群集**:webcapture.proofhq.eu

>[!NOTE]
>
>对于需要授权和受密码保护的网站的内部页面，我们建议使用交互式校样，而不是静态校样。 有关更多信息，请参阅 [交互式内容校样概述](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## 关于处理静态网站校样

* 静态网站校样中不能包含动画、嵌入式视频、脚本和交互。 如果要校样交互式内容，请参阅 [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) in [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* 通常以每页约20秒的速率捕获校样页面。 但是，整体准备时间也取决于托管页面的服务器。 工具会等待60秒，才能加载每个提交的URL。 如果超过此等待时间，校样将失败。
* 对于组合校样，如果任何URL没有响应捕获工具，校样将失败。
* [!DNL Workfront Proof] 会在光栅化后捕获长达195英寸的网页。 如果网页的时长超过此时长，校样将失败。
* 对于所有文本元素，都提供了文本提取功能，但放置为图像的文本却无法提取。
* 文本超链接在校样中是可单击的，并且链接的页面会在新的浏览器选项卡中打开。
* 如果在 `<a>` 标记。 我们建议调整页面设计的这些部分。
* 为获得最佳结果，我们建议使用最佳编码实践和公认的标准创建页面。
