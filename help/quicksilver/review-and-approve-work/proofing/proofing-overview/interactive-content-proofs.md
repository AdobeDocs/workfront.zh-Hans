---
product-area: documents
navigation-topic: proofing-overview
title: 交互式内容校样概述
description: 交互式内容提供了多种吸引观看者的方法。 代理机构可以使用从对此内容的响应中收集的分析来衡量其促销活动是否成功。
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# 交互式内容校样概述

交互式内容提供了多种吸引观看者的方法。 代理机构可以使用从对此内容的响应中收集的分析来衡量其促销活动是否成功。

交互式内容的示例包括：

* 网站
* 嵌入式或流式视频
* 交互式横幅
* HTML5动画
* 微型站点
* 交互式电子邮件

本文提供了以下关于校对交互式内容的信息：

## 关于为交互式内容创建校样

您可以通过以下方式之一为交互式内容创建校样：

* 从包含交互内容的ZIP文件创建校样。

   Adobe Workfront会从ZIP文件中解压缩内容，并将其存储在Workfront服务器上。 由于它是以这种方式存储的，因此您可以在整个校样审阅周期中依赖保持相同的内容。

* 指定内容的URL。

   这是为交互式内容创建校样的最简单方法。 这也是当用户在Internet上体验内容时，您可以以交互方式查看内容的唯一方法。

   使用这种方法，Workfront未知的外部服务器将存储并托管该内容。

   我们建议对大型网站使用此方法，因为很难收集构成大型网站的所有文件。 但是，由于校样的内容是在外部存储的，因此Workfront无法保护其免受开发人员对其进行的更改的影响，因此您可能无法在整个校样审阅周期中始终使用相同的内容。

## 关于在ZIP文件中准备交互式内容以进行校对

在ZIP文件中捆绑交互式内容进行校对时，请确保包含以下规范：

* 包文件中应包含所有资产，如CSS、JavaScript、视频、声音和图像。
* 交互式内容应包含主文件(index.html、index.htm)。 如果此文件未放在根位置，则工具会自动搜索文件夹以查找它。 主文件不需要命名为index.html/index.htm ，但主位置只能放置一个.html/.htm文件。
* 文件必须至少包含一个静态文件网页。
* 最大包大小为500 MB。
* 对于在iOS中创建的.zip文件，该工具会自动标识内容所在的文件夹
* 交互式项目仅作为.zip存档受支持。 标准.zip文件提交将失败。
* 网站必须是安全的(HTTPS)。

   使用桌面校对查看器时不需要这样做。

   有关更多信息，请参阅 [了解桌面校对查看器](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* 必须允许在iFrame中查看网站。

   使用桌面校对查看器时不需要这样做。

   有关更多信息，请参阅 [了解桌面校对查看器](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## 关于创建交互式校样

在准备ZIP包文件后，创建一个交互式校样。

有关更多信息，请参阅 [在ZIP文件中为交互式内容创建校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).

或者，如果您使用的是Workfront校样，请参阅 [为交互式内容生成校样](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generati) 在文章中 [在Workfront校样中生成校样](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## 关于审阅交互式校样

我们建议您使用独立的桌面校对查看器作为交互式校样的默认查看器。 但是，如果贵组织的策略不允许使用桌面校对查看器应用程序，则Workfront管理员可以配置您的系统，以便您能够在Web校对查看器中查看捆绑在ZIP存档文件中的交互式内容。 有关桌面校对查看器和Web校对查看器的比较信息，请参阅 [Web校对查看器与桌面校对查看器概述之间的差异](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
