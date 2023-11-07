---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: DOCU对象不支持链接文件夹
description: DOCU对象不支持链接文件夹
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# 不支持使用API添加链接的文件夹

不支持使用API将链接文件夹添加到文档(DOCU)对象的文件夹数组。 请求将成功，但某些外部提供商可能会从系统中移除文档。 这是因为，外部体系将被用作最终真相来源。 因此，如果文档从外部提供程序中删除，则该文档被视为不再存在。 在链接的（外部）文件夹中未找到任何文档均可以自动从中删除 [!DNL Workfront] 却无法取回它们。
