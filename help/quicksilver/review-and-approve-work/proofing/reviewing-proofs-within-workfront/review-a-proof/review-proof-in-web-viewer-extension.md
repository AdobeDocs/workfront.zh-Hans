---
product-area: documents
navigation-topic: proofing-overview
title: 在Web验证查看器扩展中查看交互式内容
description: Adobe Workfront审阅工具是一种浏览器扩展，它允许您校对ZIP文件或URL中的交互式内容。
author: Courtney
feature: Digital Content and Documents
exl-id: 4fea13cc-2d56-466e-8851-6134782e7e80
source-git-commit: 78d9e8e47f8f6777f9211d8f85a3dfbc9405d798
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 1%

---

# 使用Adobe Workfront审阅工具审阅交互式内容


>[!IMPORTANT]
>
> 对于托管在需要SSO身份验证或阻止在iFrame中打开其网站的网站（例如Figma）上的交互式内容，我们建议使用桌面验证查看器。

Adobe Workfront审阅工具是一个基于Web的浏览器扩展，它允许您在ZIP文件中或使用URL标记交互式内容。 Adobe Workfront审核工具在以下浏览器中提供：

* Firefox
* Chrome
* Edge
* Safari

## 安装扩展

### 先决条件

* 必须删除旧版Web Viewer扩展才能使用Adobe Workfront审阅工具。

### 安装扩展

审阅人和批准者必须安装Adobe Workfront审阅工具。 在下列浏览器中：

* [Firefox扩展](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Chrome扩展](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)

* [Safari扩展](https://apps.apple.com/us/app/adobe-workfront-review-tool/id6741517062?mt=12)



要使交互式校样在Adobe Workfront审核工具中自动打开，Workfront管理员必须更新workfront中的校样设置，如下节所述。

## 使用GenStudio for Performance Marketing和Creative Cloud Express中的Adobe Workfront审核工具

查看GenStudio for Performance Marketing和Creative Cloud Express中的内容需要此扩展。 Assets将自动在Web查看器中打开。 您无需更新任何帐户设置。


## 更新Workfront校对默认值

要使用Workfront审核工具作为交互式内容的默认查看器，您必须更新Workfront中的验证默认值。

>[!IMPORTANT]
>
>如果您需要查看的内容位于某个网站上，我们建议您使用桌面验证查看器
>
>* 需要SSO身份验证
>* 阻止在iFrame中打开其网站，例如Figma

### 将Adobe Workfront审阅工具设为URL和ZIP校样的默认查看器

要将Web审阅工具用于URL和ZIP验证，Workfront管理员必须调整交互式验证的默认设置。

1. 在Workfront的主菜单中，单击&#x200B;**校对**。
1. 单击&#x200B;**帐户设置**，然后单击&#x200B;**设置**&#x200B;选项卡。
1. 在&#x200B;**验证默认值**&#x200B;部分中，找到&#x200B;**交互式验证的桌面验证查看器**，然后单击&#x200B;**设置**。
1. 在下拉菜单中，选择&#x200B;**已禁用**。 通过URL或ZIP文件创建的交互式验证现在会自动在Adobe Workfront审阅工具（基于Web的浏览器）中打开。
1. 单击&#x200B;**保存**。

>[!NOTE]
>
>此更改适用于Workfront实例中的所有交互式验证。 我们建议先在预览环境中测试新体验，然后再在生产环境中启用它。 通过将&#x200B;**交互式校对的桌面校对查看器**&#x200B;帐户设置更改回&#x200B;**启用所有交互式校对**，可以轻松切换回桌面查看器。

### 将Adobe Workfront审阅工具设为仅用于ZIP校样的默认查看器

要仅将Web审阅工具用于ZIP验证，Workfront管理员必须调整交互式验证的默认设置。

1. 在Workfront的主菜单中，单击&#x200B;**校对**。
1. 单击&#x200B;**帐户设置**，然后单击&#x200B;**设置**&#x200B;选项卡。
1. 在&#x200B;**验证默认值**&#x200B;部分中，找到&#x200B;**交互式验证的桌面验证查看器**，然后单击&#x200B;**设置**。
1. 在下拉菜单中，选择&#x200B;**仅对从URL**&#x200B;创建的交互式验证启用。 从ZIP文件创建的交互式验证现在会自动在Adobe Workfront审阅工具（基于Web的浏览器）中打开。 从URL创建的交互式验证仍然会在桌面验证查看器中打开。
1. 单击&#x200B;**保存**。

>[!NOTE]
>
>此更改适用于您的Workfront实例中的所有ZIP校样。 我们建议先在预览环境中测试新体验，然后再在生产环境中启用它。 通过将&#x200B;**交互式校对的桌面校对查看器**&#x200B;帐户设置更改回&#x200B;**启用所有交互式校对**，可以轻松切换回桌面查看器。

