---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 故障排除 —  [!DNL Workfront Proof] 校对查看器
description: 如果未加载校对内容，并且您只能看到空的校对查看器，很可能是因为某些内容在本地阻止了此操作。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 39fdf5c2c2114a82c48f515c4a9f088596394045
workflow-type: tm+mt
source-wordcount: '955'
ht-degree: 0%

---

# 故障排除 —  [!DNL Workfront Proof] 校对查看器

<!-- Audited: 01/2024 -->

>[!IMPORTANT]
>
>本文介绍了独立版产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参见 [校对](../../../review-and-approve-work/proofing/proofing.md).

如果未加载校对内容，并且您只能看到空的校对查看器，很可能是因为某些内容在本地阻止了此操作。 尝试以下可能的解决方案。

## 确保您的浏览器 <!--and [!DNL Flash Player]--> 版本为最新

所有开发人员都在不断开发应用程序，并且会定期发布产品的新增功能和修复。 这是为了改进用户体验并保持安全级别，因此最佳实践是仅使用最新版本。 这还有助于避免应用程序之间的冲突。

<!--
### [!DNL Flash Player] Plugin Version

To check your current [!DNL Flash Player] version visit the [[!DNL Adobe] website](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

If your version number differs from the one listed for your platform go to the [[!DNL Flash Player] download page](http://get.adobe.com/flashplayer/otherversions/) and get the latest version.

Please note: we do recommend using the original [!DNL Adobe] plugin, so if your browser uses a built-in solution deactivate it and install the [!DNL Adobe] solution.
-->

### 浏览器版本

通常，大多数浏览器会自动更新，但是如果您遇到任何问题，则值得检查您使用的版本并在需要时执行更新。

在浏览器中，转到 [!UICONTROL 菜单] 并找到 [!UICONTROL 关于] 选项(在某些情况下，这可能在 [!UICONTROL 帮助] 菜单)。 在 [!UICONTROL 关于] 弹出窗口中，您可以找到有关当前浏览器版本的信息以及更新/检查更新的选项。

例如，在Chrome中：

![Chrome浏览器版本](assets/proofview-3.png)

安装最新浏览器版本后，尝试重新打开您的校样并查看问题是否已解决。

<!--

## Ensure Your Local [!DNL Flash] Storage is Available

Our [!DNL Workfront Proof] Viewer is based on Flash, and we store some data about the proofs (i.e., comments, proof tiles, [!DNL Workfront Proof] Viewer settings) on your computer using [!DNL Flash Player]. If the [!DNL Workfront Proof] Viewer opens, but there is no content inside you will want to make sure that the Flash Storage is available on your machine and that [!DNL Workfront Proof] is allowed to use it.

If there is some storage allocated, but you're working with the bigger proofs with multiple pages and comments try to increase the [!DNL Flash] Storage and re-load your proof.

-->

## 确定问题所在

* 验证是否在其他浏览器中打开？
* 如果您每天使用一个浏览器，并且无法在其中查看验证，请尝试在计算机上的其他浏览器中打开相同的验证。 要实现此目的，只需复制主浏览器URL栏中的验证链接，并将其粘贴到其他浏览器中即可。 如果验证在此处打开，请检查您的主浏览器配置、插件和扩展，因为这些可能会干扰。
* 我们没有任何首选浏览器，但如果您当前浏览器出现任何性能问题，我们建议您切换到其他浏览器。
* 验证是否会在您所在位置的其他计算机上打开？
如果您的校对未在计算机上的任何浏览器中打开，请尝试在您所在位置和/或您所在位置之外的其他计算机上打开它。 这将允许您确定特定计算机上是否有问题，或者问题是否位于本地网络中。
如果您的安全级别更高，则您与 [!DNL Workfront Proof] 可能被以下内容阻止：

   * 您的本地AV软件
   * 您的网络安全解决方案
   * DNS、防火墙或代理配置
   * 这些设置超出了我们的控制范围。 有多种安全解决方案可供使用，我们无法分辨哪些解决方案在您的网络中实施，哪些解决方案可能会阻止到您的连接 [!DNL Workfront Proof]. 也不能 [!DNL Workfront Proof] 以决定您的内部安全配置。 如果在您所在位置/网络中的多台计算机上打开验证时遇到问题，我们建议您联系IT团队，以便他们检查网络设置并授权或添加 [!DNL Workfront Proof] 到允许列表（如果需要）。

* 是否与以下对象连接 [!DNL Workfront Proof] 是否允许进入您的网络？
在验证查看器中，我们加载拼贴 — 页面的片段。 如果此内容在您的终端未正确加载，则可能是由于某些连接 [!DNL Workfront Proof] 在您的网络中被阻止。 您需要确保将所有连接和来自*.proofhq.com的所有内容添加到允许列表中。 您的IT团队应该能够帮助验证这一点。

## 查看插件

如果您的浏览器是最新的，并且网络未阻止与的连接 [!DNL Workfront Proof]，您的浏览器中可能会存在一些影响查看校样的问题。 您的浏览器中通常有多个可用的插件和扩展，其中一些插件和扩展可能会干扰其他插件和扩展，或者与其他插件和扩展发生冲突。

最佳实践是删除所有未知加载项，仅保留您使用且您信任的加载项。 每个浏览器都应为您提供用于检查/修改/删除插件和扩展的选项。 我们使用JavaScript加载 [!DNL Workfront Proof] 查看器，以便您特别查看可能会影响该查看器的插件。

如果加载验证时存在任何特定的加载项干扰，您可以尝试在浏览器的控制台中查看详细信息。

![浏览器控制台](assets/proofview-4.png)

在大多数较新的浏览器中，提供了一些其他开发人员工具，可用于进行更高级的故障排除。

如果您在查看验证时遇到问题：

* 打开浏览器的控制台，然后重新加载验证。
* 检查控制台中是否有任何警报或消息。 这些详细信息有助于确定问题的根本原因。
* 让您的IT团队分析结果。 他们应该能够提出建议并帮助解决本地问题。
* 将结果分享给我们的支持团队。 我们很乐意帮忙。

## 检查混合内容设置

与的所有连接 [!DNL Workfront Proof] 通过HTTPS。 但是，在 [!DNL Workfront Proof] 查看器我们通过HTTP加载图块，并使用令牌保护数据。 这会创建一些浏览器或安全解决方案可能阻止的混合内容（默认情况下或通过手动配置）。

如果这是校样未在计算机上打开的原因（您应该能够在浏览器的控制台中看到相关警报），请授权此类连接 [!DNL Workfront Proof] 或者修改您的设置以允许计算机上的被动混合内容。 您的浏览器、AV软件或网络配置可能会阻止混合内容，以确定确切原因。 您应该与IT团队/网络管理员取得联系。 他们还应该能够帮助在您的计算机上启用混合内容。


