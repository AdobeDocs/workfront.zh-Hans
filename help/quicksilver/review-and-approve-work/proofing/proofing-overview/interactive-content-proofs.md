---
product-area: documents
navigation-topic: proofing-overview
title: 交互式内容校对概述
description: 交互式内容提供了多种吸引观众的方法。 广告公司可以使用从对此内容的响应中收集的分析来衡量其促销活动成功与否。
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: 45dac4c5e8ff584546783d561c04d137697a03a4
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# 交互式内容校对概述

<!-- Audited: 01/2024 -->

交互式内容提供了多种吸引观众的方法。 广告公司可以使用从对此内容的响应中收集的分析来衡量其促销活动成功与否。

交互式内容的示例包括：

* 网站
* 嵌入式或流式视频
* 交互式横幅
* HTML5动画
* 微型网站
* 交互式电子邮件

## 关于为交互式内容创建校样

您可以通过以下方式之一为交互式内容创建验证：

* 从包含交互式内容的ZIP文件创建验证。

  Adobe Workfront会解压缩ZIP文件中的内容，并将其存储在Workfront服务器上。 由于是以这种方式存储的，因此在整个校对审核周期中，内容会保持不变。

* 指定内容的URL。

  这是为交互式内容创建验证的最简单方法。 这也是以交互方式查看内容的唯一方法，因为用户在Internet上体验到内容。

  通过这种方法，Workfront未知的外部服务器可以存储和托管内容。

  我们建议对大型网站使用此方法，因为很难收集构成大型网站的所有文件。 但是，由于验证内容存储在外部，因此Workfront无法保护它免受开发人员的更改影响，因此您可能无法在整个验证审核周期中依赖保持相同的内容。

## 关于在ZIP文件中准备交互式内容以进行校样

在ZIP文件中捆绑交互式内容以进行校对时，请确保它包括以下规范：

* 捆绑包文件中应包含所有资产，如CSS、JavaScript、视频、声音和图像。
* 交互式内容应包含主文件(index.html、index.htm)。 如果未将此文件放在根位置，则工具会自动搜索该文件夹以查找它。 主文件不需要命名为index.html/index.htm ，但是，主位置只能放置一个.html/.htm文件。
* 文件必须至少包含一个静态文件网页。
* 最大包大小为500 MB。
* 对于在iOS中创建的.zip文件，此工具会自动标识内容所在的文件夹。
* 仅支持将交互式项目作为.zip存档。 标准.zip文件提交将失败。
* 网站必须是安全的(HTTPS)。

  使用“桌面校对查看器”时，这不是必需的。

  有关更多信息，请参阅 [了解桌面校对查看器](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* 必须允许在iframe中查看网站。

  使用“桌面校对查看器”时，这不是必需的。

  有关更多信息，请参阅 [了解桌面校对查看器](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## 关于创建交互式验证

准备ZIP压缩包文件后，创建交互式验证。

有关更多信息，请参阅 [在ZIP文件中为交互式内容创建验证](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).

或者，如果您使用的是Workfront Proof，请参阅部分 [为交互式内容生成验证](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generate-a-proof-for-interactive-content) 在文章中 [在Workfront Proof中生成验证](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## 关于审阅交互式校样

我们建议您使用独立的桌面校对查看器作为交互式校对的默认查看器。 但是，如果贵组织的策略不允许使用桌面验证查看器应用程序，则Workfront管理员可以配置您的系统，以便您可以在Web验证查看器中查看捆绑在ZIP存档文件中的交互式内容。 有关桌面校对查看器和Web校对查看器的比较信息，请参阅 [Web验证查看器和桌面验证查看器的区别概述](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
