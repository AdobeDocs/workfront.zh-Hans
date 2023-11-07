---
content-type: api
navigation-topic: api-navigation-topic
title: 结束对JSONP的支持
description: 结束对JSONP的支持
author: Becky
feature: Workfront API
role: Developer
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# 结束对JSONP的支持

由于JSONP（带有Padding的Javascript）是一个存在已知安全漏洞的旧标准，因此，从2018年11月起，Adobe Workfront将不再支持JSONP。 这一决定支持我们实现Workfront平台现代化的更宏大计划。

JSONP是一种可用于执行跨域或跨站点请求的标准。 作为集成的一部分，许多Workfront客户和合作伙伴使用JSONP从其域上的系统访问Workfront。 JSONP允许Workfront应用程序处理来自非Workfront域的请求。

如果您将JSONP用作任何Workfront集成的一部分，则必须更新集成以使用CORS（跨源资源共享）标准。 此更新要求您执行以下操作：

1. 向Workfront支持团队提交请求，以便拥有用于向我们允许列表发出跨域请求的任何域。

   要将您的域添加到CORS允许列表中，请通过844-306-HELP(4357)或在线提交支持票证来联系Workfront客户支持。

   >[!NOTE]
   >
   >只有在2018年8月1日之前使用JSONP的客户才支持将域添加到CORS允许列表。


1. 更改集成代码以使用CORS。
