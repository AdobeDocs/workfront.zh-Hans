---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 文档Webhooks错误处理
description: 文档Webhooks错误处理
author: John
feature: Workfront API
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
source-git-commit: 338cc745a7660ffed8e4d44e19dcadfdc13bc345
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%

---

# 文档Webhooks错误处理

在处理API请求时可能会出现问题。 这应当在所有API端点中以一致的方式进行处理。 发生错误时，Webhook提供程序应在响应标头中包含错误代码。 错误代码包括：

* 403 — 禁止。 表示请求令牌缺失或无效，或者与令牌关联的凭据无权访问指定的资源。 对于基于OAuth的Webhook提供程序，Adobe Workfront将尝试检索新的访问令牌。

* 404 — 未找到。 指示指定的文件或文件夹不存在。

* 500 — 内部服务器错误。 任何其他类型的错误。

* 使用以下格式描述响应正文中的错误：

   ```
   {status: “error”
    error: “Sample error message”}
   ```
