---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 疑难解答 — Mac上的验证查看器中的界面字体损坏
description: Mac上的验证查看器中错误编号拍摄损坏的界面字体
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# 疑难解答 — Mac上的验证查看器中的界面字体损坏

>[!IMPORTANT]
>
>本文介绍了独立版产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参见 [校对](../../../review-and-approve-work/proofing/proofing.md).

如果您注意到验证查看器未正确显示界面字体，则可能是由于您的Mac计算机上的字体存在一些问题。 要解决此问题，请尝试以下解决方案：

## 删除字体重复项

检查系统中是否存在任何重复的字体。

1. 关闭您正在使用的浏览器。
1. 在“应用程序”文件夹中打开“字体簿”应用程序。
1. 单击 **[!UICONTROL 所有字体]** (1)。
1. 单击 **[!UICONTROL 编辑]** > **[!UICONTROL 查找启用的重复项]**.

1. 单击 **[!UICONTROL 是]** 以解决重复项。
1. 如果看到有关损坏字体的警告，请单击 **[!UICONTROL 是]**.
1. 重新启动计算机。
1. 重试校对。

## 清除字体缓存

有时，Mac OS X中的字体缓存会损坏。 例如，当某个字体或字体系列被重新安装多次时，或者应用程序被更新或重新安装时。 除了操作系统的字体缓存文件之外，某些应用程序可能还有自己的字体缓存。 删除这些字体缓存文件可以解决乱码文本的问题。

首先，您需要启动“Font Book（字体簿）”，选择您遇到的字体或系列，然后按键盘上的“Delete（删除）”按钮。 您还可以右键单击并选择 [!UICONTROL 删除家庭]. 如果您不确定导致问题的字体或系列，可能需要先按照上述说明删除重复项。

第二步是清除字体缓存，有几种方法可以做到这一点。

第一种，只要在启动时听到启动铃声时按住Shift键，就可以重新引导至安全模式。 加载此模式时，应出现一个进度条，在此期间系统将运行各种检查和维护例程，其中一个是清除字体缓存。

第二种方法是使用“终端”，可以通过从管理帐户中运行以下命令来完成： *sudo atsutil数据库 — remove*

>[!NOTE]
>
>此命令将要求您输入密码，键入密码时不会显示密码。 我们建议您咨询您的IT部门，因为这样可能需要您计算机的管理员权限。

另一种方法是使用字体缓存实用程序（例如FontNuke）并在其帮助下清除缓存。

许多印前和图稿/设计工作室也使用Universal Type Server软件来管理字体的许可和分发。 有时，Universal Type Server Font Cache可能会出现问题，这可能导致 [!DNL Workfront Proof] 注释消失。

要进行修复，请清除通用类型服务器字体缓存并重新启动通用类型服务器。

## 修复 [!DNL Flash] 字体冲突

您可能无法访问此功能，因为它受支持 [!DNL Flash]，该功能已在大多数环境中弃用。

旧版验证查看器的基础是 [!DNL Flash Player] 有时，当验证查看器中缺少文本时，OS X与之间存在字体冲突 [!DNL Flash Player]. 尝试以下操作：

1. 打开Finder并打开 **[!UICONTROL 开始]** 选项卡。
1. 按Option键(⌥Alt)打开 [!UICONTROL 库] 文件夹来创建。
1. 按住Option键，单击 [!UICONTROL 库] 文件夹。
1. 在 [!UICONTROL 库] 文件夹打开，转到 [!UICONTROL 字体] 文件夹的位置。
1. 移动所有位于 [!UICONTROL 字体] 文件夹移入其他文件夹，可能在您的桌面上（请不要在Fonts文件夹内创建其他文件夹）。
1. 此操作会隐藏所有自定义字体；您仍应将标准系统字体保存在其单独位置。
1. 退出并重新启动 [!DNL Safari].
1. 重新打开验证。

您现在应该可以看到您的字体。 如果您不需要从主目录中删除的任何字体，则可以安全地删除它们。 否则，请分批查看，将它们复制回Library/Fonts文件夹，然后查看导致问题的文件。
