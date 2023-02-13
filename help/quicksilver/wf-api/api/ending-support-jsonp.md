---
content-type: api
navigation-topic: api-navigation-topic
title: 停止对JSONP的支持
description: 停止对JSONP的支持
author: John
feature: Workfront API
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: 606d19b8a83b833aba6d6b15231a8683aa2cee40
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# 停止对JSONP的支持

由于JSONP（带内边距的Javascript）是一个具有已知安全漏洞的旧标准，因此自2018年11月起，Adobe Workfront将不再支持JSONP。 这一决定支持我们更大的Workfront平台现代化倡议。

JSONP是执行跨域或跨站点请求的标准。 许多Workfront客户和合作伙伴使用JSONP从其自己域的系统中访问Workfront（作为集成的一部分）。 JSONP允许Workfront应用程序处理来自非Workfront域的请求。

如果您在任何Workfront集成中使用JSONP，则必须更新集成才能使用CORS（跨域资源共享）标准。 此更新要求您执行以下操作：

1. 向Workfront支持团队提交请求，以包含任何用于向我们的提出跨域请求的允许列表域。

   要将您的域添加到CORS允许列表中，请联系Workfront客户支持(844-306-HELP(4357))或通过在线提交支持票证来联系。

   >[!NOTE]
   >
   >仅2018年8允许列表月1日之前使用JSONP的客户支持将域添加到CORS。


1. 更改集成代码以使用CORS。
