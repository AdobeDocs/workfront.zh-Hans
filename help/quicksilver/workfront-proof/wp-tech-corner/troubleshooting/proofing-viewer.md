---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 疑难解答 —  [!DNL Workfront Proof] 校样查看器
description: 如果校样内容未加载，并且您只能看到空校样查看器，则很可能是因为本地有某些内容阻止了此操作。 请在下面尝试可能的解决方案。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 0%

---

# 疑难解答 —  [!DNL Workfront Proof] 校样查看器

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

如果校样内容未加载，并且您只能看到空校样查看器，则很可能是因为本地有某些内容阻止了此操作。 请在下面尝试可能的解决方案。

## 确保您的浏览器和 [!DNL Flash Player] 版本为最新

所有开发人员都会不断处理其应用程序，并且会定期为其产品发布新功能和修复。 这是为了改善用户体验并维护安全级别，因此最好只使用最新版本。 这也有助于避免应用程序之间的冲突。

### [!DNL Flash Player] 插件版本

检查您的当前 [!DNL Flash Player] 版本访问 [[!DNL Adobe] 网站](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

如果版本号与为平台列出的版本号不同，请转到 [[!DNL Flash Player] 下载页面](http://get.adobe.com/flashplayer/otherversions/) 并获取最新版本。

请注意：我们建议使用 [!DNL Adobe] 插件，因此，如果您的浏览器使用内置解决方案来停用它并安装 [!DNL Adobe] 解决方案。

### 浏览器版本

现在，大多数浏览器都会自动更新，但如果您遇到任何问题，则需要检查您使用的版本并在需要时执行更新。

在您的浏览器中，转到 [!UICONTROL 菜单] 并找到 [!UICONTROL 关于] 选项(在某些情况下，这可能显示在 [!UICONTROL 帮助] 菜单)。 在 [!UICONTROL 关于] 弹出窗口，您将找到有关当前浏览器版本的信息以及用于更新/检查更新的选项。

请在Chrome中参阅：

![ProofView_3.png](assets/proofview-3-350x206.png)

在您的 [!DNL Flash Player] 已安装的插件和浏览器版本尝试重新打开校样，并查看问题是否已解决。

## 确保您的本地 [!DNL Flash] 存储可用

我们的 [!DNL Workfront Proof] 查看器基于Flash，我们存储了一些有关校样的数据(例如，注释、校样图块、 [!DNL Workfront Proof] 查看器设置) [!DNL Flash Player]. 如果 [!DNL Workfront Proof] 查看器随即会打开，但您内部没有内容，您需要确保Flash存储在您的计算机上可用，并且 [!DNL Workfront Proof] 允许使用它。

如果分配了一些存储，但您正在使用包含多个页面的较大校样，并且会尝试增加 [!DNL Flash] 存储并重新加载校样。

请看我们的 [查看校样时出现问题 —  [!DNL Flash] 共享对象说明](../../../workfront-proof/wp-tech-corner/troubleshooting/view-proof-flash-shared-object.md) 以了解详细说明。

## 确定问题所在

* 是否在其他浏览器中打开校样？
* 如果您每天使用一个浏览器，并且在查看校样时遇到问题，请尝试在计算机上的其他浏览器中打开相同的校样。 为此，只需从主浏览器的URL栏中复制校样链接，并将其粘贴到其他浏览器中即可。 如果校样在此处打开正常，请查看主浏览器配置、插件和扩展，因为这些组件可能会干扰您的配置、插件和扩展。
* 我们没有任何首选的浏览器，但是如果您当前的浏览器中存在任何性能问题，我们建议您切换到其他浏览器。
* 在您位置的其他计算机上打开的校样是否？
如果校样未在计算机上的任何浏览器中打开，请尝试在您所在位置和/或位置外的其他计算机上将其打开。 这将允许您确定问题是否由特定计算机决定，或问题是否在本地网络中。
如果安全级别较高，则连接到 [!DNL Workfront Proof] 可能会被以下用户阻止：

   * 您的本地AV软件
   * 您的网络安全解决方案
   * DNS、防火墙或代理配置
   * 这些设置超出了我们的控制范围。 有各种可用的安全解决方案，我们无法判断您的网络中实施了哪些解决方案，哪些解决方案可能会阻止与 [!DNL Workfront Proof]. 这也不是 [!DNL Workfront Proof] 来决定您的内部安全配置。 如果您在位置/网络的多台计算机上打开校样时遇到问题，我们建议您与IT团队联系，以便他们检查网络设置并授权或添加 [!DNL Workfront Proof] ，如允许列表果需要。

* 是否与 [!DNL Workfront Proof] 允许在您的网络中吗？
在校样查看器中，我们加载图块 — 页面的片段。 如果此内容在您的末尾未正常加载，则可能是 [!DNL Workfront Proof] 在您的网络中被阻止。 您需要确保将*.proofhq.com中的所有连接和所有内容都添加到允许列表中。 您的IT团队应该能够帮助验证此信息。

## 审核插件

如果您的浏览器和 [!DNL Flash Player] 插件为最新，且您的网络未阻止与 [!DNL Workfront Proof] 浏览器中可能存在一些影响查看校样的内容。 现在，您的浏览器中有多个可用的插件和扩展，其中一些插件和扩展会干扰其他插件或与其他插件冲突。

最佳做法是删除所有未知的附加组件，并仅保留您使用和信任的附加组件。 每个浏览器都应为您提供用于检查/修改/删除插件和扩展的选项。 我们的 [!DNL Workfront Proof] 查看者基于 [!DNL Flash] 我们会使用JavaScript加载查看器，因此您需要特别查看可能影响这些查看器的插件。

请访问下面列出的页面，以了解开发人员有关如何禁用浏览器加载项的更多详细信息：

* 铬黄： [plugins](https://support.google.com/chrome/answer/142064?hl=en-GB) / [扩展](https://support.google.com/chrome/answer/113907?hl=en-GB)
* Firefox: [附加组件](https://support.mozilla.org/en-US/kb/disable-or-remove-add-ons)
* Internet Explorer: [附加组件](http://windows.microsoft.com/en-GB/internet-explorer/manage-add-ons#ie=ie-11)
* Safari: [附加组件](http://support.apple.com/en-gb/HT203353)

如果存在任何干扰校样加载的特定附加组件，您可以尝试在浏览器控制台中检查详细信息。

![ProofView_4.png](assets/proofview-4-350x57.png)

在大多数较新的浏览器中，有一些其他开发人员工具可用，可用于进行更高级的故障诊断。

如果您在查看校样时遇到问题：

* 打开浏览器的控制台并重新加载校样。
* 检查控制台中是否有警报或消息。 这些详细信息有助于确定问题的根本原因。
* 让您的IT团队分析结果。 他们应该能够提供建议并帮助解决当地问题。
* 与我们的 [支持团队](https://support.workfront.com/hc/en-us/requests/new). 我们很乐意协助。

如果您不知道如何在浏览器中打开控制台，请参阅记录的步骤：

* [Firefox](http://screencast.com/t/eP6FRtk4vxWS)
* [Internet Explorer](http://screencast.com/t/bYzq1iQv)
* [Google Chrome](http://screencast.com/t/2anpeAzOOyj)
* [Safari](http://screencast.com/t/rnOvgl3GidjL)

您还可以查看浏览器开发人员的文档以了解更多详细信息。

## 检查混合内容设置

与 [!DNL Workfront Proof] 过HTTPS。 但是，在 [!DNL Workfront Proof] 我们通过HTTP加载图块的查看器，并且使用令牌保护数据。 这会创建一些浏览器或安全解决方案可能会阻止的混合内容（默认情况下或根据手动配置）。

如果这是校样未在计算机上打开的原因（您应该能够在浏览器控制台中看到相关警报），请为 [!DNL Workfront Proof] 或者，修改设置以允许在您的计算机上使用被动混合内容。 您的浏览器、AV软件、网络配置等可能会阻止混合内容，以确定具体原因，请与您的IT团队/网络管理员联系。 他们还应该能够帮助您在计算机上启用混合内容。

联系我们的 [支持团队](https://support.workfront.com/hc/en-us/requests/new) 如果你需要我们的帮助。
