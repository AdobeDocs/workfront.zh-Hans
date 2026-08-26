---
product-area: documents
navigation-topic: documents-navigation-topic
title: Adobe Workfront中的C2PA元数据
description: 了解什么是C2PA元数据以及Adobe Workfront如何将其保留在您上传、存储和下载的文档中。
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 3510218fb179a0852ad22abe2a753ccdb261205a
workflow-type: tm+mt
source-wordcount: 215
ht-degree: 0%

---

# Adobe Workfront中的C2PA元数据

C2PA元数据是安全且易于篡改的信息，随内容一起传输。 当创作AI (GenAI)用于创建或更改图像、视频或音频文件时，C2PA元数据会记录该事实，以便收到文件的任何人都可以查看文件的生成方式。

C2PA元数据基于打开的[C2PA](https://c2pa.org/)标准。

## C2PA元数据包含的内容

C2PA元数据包括：

* 提供GenAI工具的提供商的名称。
* 用于创建或更改内容的GenAI系统的名称和版本号。
* 创建或更改内容的日期和时间。
* 唯一标识符。

C2PA元数据不包括任何个人身份信息(PII)。

## Workfront如何处理C2PA元数据

Adobe Workfront不会修改您所用文件的元数据。 上传已包含C2PA元数据的文件时，Workfront会保留该信息，因为该文件存储在Workfront中并从下载。

由于元数据嵌入在文件本身中，因此通过Workfront工作流保持其完整性，因此，当元数据离开Workfront时，其来源信息将随内容保留。
