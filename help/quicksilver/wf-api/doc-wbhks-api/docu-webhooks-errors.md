---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 文档Webhooks错误处理
description: 文档Webhooks错误处理
author: Becky
feature: Workfront API
role: Developer
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# 文档Webhooks错误处理

处理API请求时可能会出现问题。 应当在所有API端点中以一致的方式处理此问题。 发生错误时，webhook提供程序应在响应标头中包含错误代码。 错误代码包括：

* 403 — 禁止访问。 指示请求令牌缺失或无效，或者与令牌关联的凭据无权访问指定的资源。 对于基于OAuth的webhook提供程序，Adobe Workfront将尝试检索新的访问令牌。

* 404 — 未找到。 指示指定的文件或文件夹不存在。

* 500 — 内部服务器错误。 任何其他类型的错误。

* 使用以下格式对响应正文中的错误的描述：

  ```
  {status: "error"
   error: "Sample error message"}
  ```
