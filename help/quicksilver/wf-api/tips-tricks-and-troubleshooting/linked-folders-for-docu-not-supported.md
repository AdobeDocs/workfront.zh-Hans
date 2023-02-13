---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: DOCU对象不支持链接的文件夹
description: DOCU对象不支持链接的文件夹
author: Becky
feature: Workfront API
source-git-commit: 9bdc433158e471729bd27d701947d6ae41aa06e7
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---


# 不支持使用API添加链接的文件夹

不支持使用API将链接的文件夹添加到文档(DOCUM)对象的文件夹数组。 请求将成功，但某些外部提供程序可能会从系统中删除该文档。 这是因为外部系统将被用作真相的最终来源。 因此，如果从外部提供商中删除文档，则文档将被视为不再存在。 在链接的（外部）文件夹中未找到的任何文档都可以自动从 [!DNL Workfront] 却无法挽回。
