---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 速度问题 [!DNL Workfront Proof]
description: 此帮助页面可帮助您确定在使用 [!DNL Workfront Proof] 与您的ISP或 [!DNL Workfront Proof]的内容交付网络。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 0%

---

# 速度问题 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

此帮助页面可帮助您确定在使用 [!DNL Workfront Proof] 与您的ISP或 [!DNL Workfront Proof]的内容交付网络。

速度问题通常是由本地ISP连接或本地Internet接入设置（例如，使用代理服务器的情况）引起的，因此很遗憾，速度问题不在控制之下 [!DNL Workfront Proof].

尽管如此，您可以采取一些步骤来检查连接速度，以确定您遇到的问题的根本原因。 所有这些步骤对于故障排除过程同样重要，我们建议您花时间收集所有所列步骤的信息，以确保对问题进行最准确的诊断。

收集所有详细信息后，我们建议您咨询当地IT部门，以确定任何本地问题。 如果您在此事上需要进一步帮助，请联系我们 [支持团队](https://support.workfront.com/hc/en-us/requests/new).

## 确定系统的哪个部分速度较慢

使用 [!DNL Workfront Proof]，则您可能正在使用功能板，例如管理文件夹内容和用户，或者使用 [!DNL Workfront Proof] 查看者：进行验证审阅、检查已发表的评论等。

确定系统的哪个确切部分速度慢是排除速度问题的第一步。 报告时 [!DNL Workfront Proof] 速度慢，请确保描述以下内容：

* 您在其他网页上是否遇到速度慢？
* 是否在功能板中出现问题或 [!DNL Workfront Proof] 查看者？
* 系统的哪个部分速度很慢？ (例如，处理新校样或在 [!DNL Workfront Proof] 查看器)

## 运行traceroute和ping测试

遇到性能问题时，务必运行traceroute命令来验证连接。 要执行此操作，请在系统中打开命令提示符(Mac/Linux中的终端)并执行以下步骤：

1. 键入以下任一内容，然后等待跟踪器完成：

   * Windows: **tracert app.proofhq.com**
   * Mac/Linux: **traceroute app.proofhq.com**

1. （仅限Windows）类型 **ping app.proofhq.com**.
1. Ping完成后，在命令提示符中右键单击并选择“全选”。
1. 将结果复制并粘贴到电子邮件的回复中。
在将结果发送给支持团队之前，请确保允许traceroute和ping完成。

## 使用Speedtest.net测试连接速度

1. 单击 [此处](http://www.speedtest.net/) 访问Speedtest.net。
1. 按照Speedtest知识库中的说明来测试Internet连接的速度。
1. 将结果复制并粘贴到我们的支持团队的电子邮件中。

## 在浏览器控制台中检查网络选项卡

现代浏览器中提供的Web控制台可收集有关任何网络延迟的有用信息，事实证明，这些信息将有助于我们确定您遇到的速度问题的根本原因。

要检查网页的加载时间，请执行以下操作：

1. 打开浏览器的控制台和“网络”选项卡。
1. 重新加载页面。
1. 拍摄屏幕截图或记录结果的屏幕截图。
1. 与支持团队共享结果。

请确保屏幕截图显示所有数据 — 您可以在拍摄屏幕截图时展开控制台窗口，或在屏幕截图中向下滚动。

如果您不知道如何在浏览器中打开控制台，请参阅以下记录的步骤：

* [铬黄](http://screencast.com/t/AgQU6JQQ)
* [Safari](http://screencast.com/t/f31GqQYm0w)
* [Firefox](http://screencast.com/t/Xg7SscmAi)
* [Edge](http://www.screencast.com/t/epSwBiaD)
* [Internet Explorer](http://screencast.com/t/x5Q3eHczbc)

您还可以查看浏览器的文档以了解更多详细信息。

## 在其他网络和计算机上检查您的连接

检查您是否在使用不同设备或网络时遇到相同的连接速度问题，是故障排除过程中的关键步骤。 请尝试切换到其他计算机或移动设备，并尝试使用替代网络（如移动数据）。

比较不同组合中的连接：在同一网络上使用不同的计算机，在不同网络上使用同一台计算机，同时使用备用计算机和网络，然后与支持团队共享结果。
