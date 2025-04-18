---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Webhooks概述
description: Webhooks概述
author: Becky
feature: Workfront API
role: Developer
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 0%

---


# Webhooks概述

Adobe Workfront Document Webhooks定义了一组API端点，Workfront通过这些API端点向外部文档提供商发出授权的API调用。 这允许任何人为任何文档存储提供商创建中间件插件。

![Webhooks](assets/mceclip0-350x262.png)

基于webhook的集成的用户体验将与现有文档集成的用户体验类似，例如Google Drive、Box和Dropbox。 例如，Workfront用户将能够执行以下操作：

* 导航外部文档提供程序的文件夹结构
* 搜索文件
* 将文件链接到Workfront
* 将文件上载到外部文档提供商
* 查看文档的缩略图

**参考实现**

为了帮助快速启动新的Webhooks实施的开发，Workfront提供了参考实施的示例。 这些示例可在[https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app)中找到。 这些示例基于Java，并允许Workfront在网络文件系统上连接文档。 

>[!NOTE]
>
>GitHub上的资源仅用作示例，无法执行实施。

## 版本

* 版本1.0（发行日期 — 2015年5月）：初始规范

* 版本1.1（发行日期：2015年6月）。 更新了/uploadInit — 添加了documentId和documentVersionId

* 版本1.2（发行日期 — 2015年10月）：已添加/createFolder

* 即将发布的版本（发行日期 — 待定）：

   * 添加了/delete
   * 添加了/rename
   * 添加了/serviceInfo
   * 添加了/customAction
   * 将分页和parentId添加到/search
