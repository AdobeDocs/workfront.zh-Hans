---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: DOCU对象不支持链接文件夹
description: DOCU对象不支持链接文件夹
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
TQID: https://experienceleague.adobe.com/iPjiffn9QLDldjWRdxMyf8RTaZaB9X6axc7UVY1B3Bg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 118
ht-degree: 0%

---

# 不支持使用API添加链接的文件夹

不支持使用API将链接文件夹添加到文档(DOCU)对象的文件夹数组。 请求将成功，但某些外部提供商可能会从系统中移除文档。 这是因为，外部体系将被用作最终真相来源。 因此，如果文档从外部提供程序中删除，则该文档被视为不再存在。 在链接的（外部）文件夹中未找到任何文档都可能会自动从[!DNL Workfront]中删除，无法恢复它们。
