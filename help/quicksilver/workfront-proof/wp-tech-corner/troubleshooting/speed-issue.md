---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: ' [!DNL Workfront Proof]中的速度问题'
description: 此帮助页可帮助您确定在使用 [!DNL Workfront Proof] 时可能遇到的任何速度问题是否与您的ISP或 [!DNL Workfront Proof]的内容交付网络有关。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 20fcf4dd07c1058559533501f7e297d78c43a70b
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# [!DNL Workfront Proof]中的速度问题

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

此帮助页可帮助您确定在使用[!DNL Workfront Proof]时可能遇到的任何速度问题是否与您的ISP或[!DNL Workfront Proof]的内容交付网络有关。

速度问题通常是由于本地ISP连接或本地Internet访问设置（例如，使用了代理服务器）造成的，因此很遗憾，这不在[!DNL Workfront Proof]的控制范围之内。

也就是说，您可以执行一些步骤来检查连接速度，以确定您所遇到的问题的根本原因。 所有这些步骤对于故障排除过程同样重要，我们建议您花一些时间收集有关列出的所有步骤的信息，以确保对问题进行最准确的诊断。

收集所有详细信息后，我们建议您咨询当地IT部门，以确定任何本地问题。

## 确定系统的哪个部分速度较慢

当您使用[!DNL Workfront Proof]时，您可能会使用功能板，例如，管理文件夹内容和用户，或者使用[!DNL Workfront Proof]查看器：进行校样审核，检查已作出的评论等。

确定系统哪个部分速度较慢是解决速度问题的第一步。 当您报告[!DNL Workfront Proof]速度缓慢时，请确保描述以下内容：

* 您是否在其他网页中遇到速度变慢的问题？
* 问题是否在仪表板或[!DNL Workfront Proof]查看器中出现？
* 系统的哪个部分速度较慢？ （例如，处理新验证或在[!DNL Workfront Proof]查看器中打开评论）

## 运行traceroute和ping测试

当您遇到性能问题时，请务必运行traceroute命令来验证连接。 为此，请在系统中打开命令提示符(Mac/Linux中的“Terminal（终端）”)，然后执行以下步骤：

1. 键入以下内容之一，然后等待跟踪程序完成：

   * Windows： **tracert app.proofhq.com**
   * Mac/Linux： **traceroute app.proofhq.com**

1. （仅限Windows）类型&#x200B;**ping app.proofhq.com**。
1. Ping完成后，在命令提示符下右键单击并选择“Select All（全选）”。
1. 将结果复制并粘贴到您电子邮件的回复中。
在将结果发送到支持团队之前，请确保允许traceroute和ping完成。

## 使用Speedtest.net测试连接速度

1. 打开浏览器，然后转到Speedtest.net。
1. 按照Speedtest知识库中的说明测试Internet连接的速度。
1. 将结果复制并粘贴到我们的支持团队的电子邮件中。

## 检查浏览器控制台中的“网络”选项卡

现代浏览器中提供的Web控制台可收集有关任何网络延迟的有用信息，这些信息将帮助我们确定您所遇到的速度问题的根本原因。

要检查网页的加载时间：

1. 打开浏览器的控制台和Network选项卡。
1. 重新加载页面。
1. 拍摄屏幕快照或录制结果的屏幕截图。
1. 将结果分享给支持团队。

请确保屏幕快照显示了所有数据 — 您可以在拍摄屏幕快照时展开控制台窗口，或者在屏幕截图中向下滚动。

您还可以查看浏览器的文档以了解更多详细说明。

## 检查您在其他网络和计算机上的连接

检查使用其他设备或网络的连接速度是否遇到同样的问题是故障排除过程中的关键步骤。 请尝试切换到其他计算机或移动设备，并尝试使用替代网络（例如移动数据）。

比较不同组合的连接：在同一网络上使用不同的计算机，在不同网络上使用相同的计算机，同时使用替代计算机和网络，然后与支持团队共享结果。
