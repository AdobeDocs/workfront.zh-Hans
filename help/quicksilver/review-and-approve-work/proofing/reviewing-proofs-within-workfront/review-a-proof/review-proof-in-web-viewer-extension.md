---
product-area: documents
navigation-topic: proofing-overview
title: 在Web验证查看器扩展中查看交互式内容
description: Adobe Workfront审阅工具是一种浏览器扩展，它允许您校对ZIP文件或URL中的交互式内容。
author: Courtney
feature: Digital Content and Documents
source-git-commit: def2526e2e1bb83998f0adc221b3011c471f72f8
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 1%

---


# 使用Adobe Workfront审阅工具审阅交互式内容

<span class="preview">Adobe Workfront审核工具将于2024年11月1日提供。</span>

Adobe Workfront审阅工具是一种浏览器扩展，它允许您校对ZIP文件或URL中的交互式内容。 Adobe Workfront审核工具在以下浏览器中提供：

* Firefox
* Chrome
* Edge

对于阻止在iFrame中打开其网站的网站（例如Figma），我们建议使用桌面校对查看器。

## 先决条件

要使用Web审阅工具，Workfront管理员必须禁用自动为交互式内容打开桌面验证查看器的设置：

1. 在Workfront的主菜单中，单击&#x200B;**校对**。
1. 单击&#x200B;**帐户设置**，然后单击&#x200B;**设置**&#x200B;选项卡。
1. 在&#x200B;**验证默认值**&#x200B;部分中，找到&#x200B;**交互式验证的桌面验证查看器**，然后单击&#x200B;**设置**。
1. 在下拉菜单中，选择&#x200B;**已禁用**。
1. 单击&#x200B;**保存**。

>[!IMPORTANT]
>
>此更改适用于预览和生产环境中的所有交互式验证。 我们建议先在预览环境中测试新体验，然后再在生产环境中启用它。 通过将帐户设置更改回&#x200B;**Enabled （对于所有交互验证）**&#x200B;或&#x200B;**Enabled （仅对于从URL创建的交互验证）**，可以轻松切换回Desktop Viewer。


## 安装扩展

审阅人和批准者必须在以下浏览器之一中安装Adobe Workfront审阅：

* [Firefox扩展](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Chrome扩展](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)

安装该扩展后，将在Adobe Workfront审核工具中自动打开交互式验证。


必须禁用用于打开交互式校对的桌面校对查看器的设置，才能使用Workfront审阅工具。 有关禁用此设置的信息，请参阅上面的[先决条件](#prerequisites)部分。



