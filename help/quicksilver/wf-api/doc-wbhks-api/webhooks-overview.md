---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Webhooks概述
description: Webhooks概述
author: Becky
feature: Workfront API
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Webhooks概述

Adobe Workfront Document Webhooks定义了一组API端点，Workfront通过这些端点对外部文档提供程序进行授权API调用。 这允许任何人为任何文档存储提供程序创建中间件插件。

![](assets/mceclip0-350x262.png)

基于Webhook的集成的用户体验将与现有文档集成的用户体验相似，例如Google Drive、Box和Dropbox。 例如，Workfront用户将能够执行以下操作：

* 导航外部文档提供程序的文件夹结构
* 搜索文件
* 将文件链接到Workfront
* 将文件上传到外部文档提供程序
* 查看文档的缩略图

**参考实施**

为帮助快速开始开发新的Webhook实施，Workfront提供了一个参考实施。 此代码可在 [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app) . 此实施基于Java，允许Workfront在网络文件系统上连接文档。 

## 版本

* 1.0版（发行日期 — 2015年5月）：初始规范

* 1.1版（发行日期 — 2015年6月）。 更新了/uploadInit — 添加了documentId和documentVersionId

* 1.2版（发行日期 — 2015年10月）：添加了/createFolder

* 即将推出的版本（发行日期 — 待定）：

   * 添加了/delete
   * 添加了/重命名
   * 添加了/serviceInfo
   * 添加了/customAction
   * 将分页和parentId添加到/search
