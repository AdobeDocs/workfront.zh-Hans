---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 疑难解答 — Mac上校对查看器中的界面字体损坏
description: 如果您发现校对查看器未正确显示界面字体，这可能是由于Mac计算机上的字体存在某些问题所致。 要解决此问题，请尝试以下解决方案 — 编辑我。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# 疑难解答 — Mac上校对查看器中的界面字体损坏

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

如果您发现校对查看器未正确显示界面字体，这可能是由于Mac计算机上的字体存在某些问题所致。 要解决此问题，请尝试以下解决方案：

## 删除字体重复项

检查系统中是否存在任何重复的字体。

1. 关闭您正在使用的浏览器。
1. 在“应用程序”文件夹中打开字体帐簿应用程序。
1. 单击 **[!UICONTROL 所有字体]** (1)。
1. 单击 **[!UICONTROL 编辑]** > **[!UICONTROL 查找已启用的重复项]**.

1. 单击 **[!UICONTROL 是]** 来解析重复项。
1. 如果看到有关损坏字体的警告，请单击 **[!UICONTROL 是]**.
1. 重新启动计算机。
1. 重试校样。

## 清除字体缓存

有时，Mac OS X中的字体缓存会损坏。 例如，当字体或一系列字体重新安装多次，或者应用程序已更新或重新安装时。 除操作系统的字体缓存文件外，某些应用程序可能有自己的字体缓存。 删除这些字体缓存文件可以解决出现乱码文本的问题。

首先，您需要启动字体手册，选择您遇到问题的字体或系列，然后按键盘上的“删除”按钮。 您还可以右键单击并选择 [!UICONTROL 移除系列]. 如果不确定导致问题的字体或系列，您可能需要尝试按如上所述先删除重复项。

第二步是清除字体缓存，有多种方法可实现此目的。

第一种方法是，在启动时听到启动提示声后，立即按住Shift键，直接重新启动到安全模式。 加载此模式时，应显示一个进度条，在该进度条中，系统将运行各种检查和维护例程，其中一个例程是清除字体缓存。

第二种方法是使用终端，该终端可通过在管理帐户中运行以下命令来完成： *sudo atsutil数据库 — remove*

>[!NOTE]
>
>此命令将要求您输入密码，键入时不会显示该密码。 我们建议咨询您的IT部门，因为这可能需要您计算机上的管理员权限。

另一种方法是使用字体缓存实用程序（如FontNuke），并通过其帮助清除缓存。

许多印前和画布/设计工作室还使用通用型服务器软件来管理字体的许可和分发。 有时，通用类型服务器字体缓存可能会出现问题，这可能导致 [!DNL Workfront Proof] 注释会消失。

要进行修复，请清除通用类型服务器字体缓存并重新启动通用类型服务器。

## 修复 [!DNL Flash] 字体冲突

您可能无权访问此功能，因为它受 [!DNL Flash]，在大多数环境中已弃用。

旧版校对查看器基于 [!DNL Flash Player] 有时，当校样查看器中缺少文本时，OS X与之之间可能存在字体冲突 [!DNL Flash Player]. 尝试以下操作：

1. 打开“查找器”并打开 **[!UICONTROL 开始]** 选项卡。
1. 按Option键(Alt⌥)打开 [!UICONTROL 库] 文件夹。
1. 在按住Option键的同时，单击 [!UICONTROL 库] 文件夹。
1. 在 [!UICONTROL 库] 文件夹打开，转到 [!UICONTROL 字体] 文件夹。
1. 移动位于 [!UICONTROL 字体] 文件夹移入其他文件夹中，可能是在您的桌面上（请不要在Fonts文件夹内创建其他文件夹）。
1. 此操作将隐藏您的所有自定义字体；您仍应将标准系统字体保存在其单独位置。
1. 退出并重新启动 [!DNL Safari].
1. 重新打开校样。

您现在应该看到您的字体。 如果您不需要从主目录中删除的任何字体，则可以安全地删除这些字体。 否则，请分批完成这些操作，将它们复制回Library/Fonts文件夹，然后查看是哪个操作导致了问题。
