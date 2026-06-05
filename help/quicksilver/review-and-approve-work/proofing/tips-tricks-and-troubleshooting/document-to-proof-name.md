---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: 上载后文档名称已更改并包含无效字符
description: 某些文档无法转换为验证。
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
TQID: https://experienceleague.adobe.com/bE5iUIG7rFpIIa3zXt-5pO0sgfbEO-3QDVFVLwkayIo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 135
ht-degree: 1%

---

# 上载后文档名称已更改并包含无效字符

## 问题

某些文档无法转换为验证。

## 原因

上载到Workfront的文件不能包含文件名中的某些字符。 如果文件在文件名中包含以下任何字符，则在上载文件时，将从文件名中删除这些字符： `! # % * \ | ' " / ? < > { } [ ]`。

如果在初次上传后，文档名称更新为包含无效字符，则验证生成将失败。

## 解决方案

从文档名称中删除无效字符：

1. 选择文档，然后单击&#x200B;**文档详细信息**。
1. 单击文档名称并删除无效字符，然后按Enter。

   无效的字符： `! # % * \ | ' " / ? < > { } [ ]`

   ![文档名称](assets/doc-name.png)

1. 刷新页面并生成验证。
