---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 测试Webhook连接
description: 测试Webhook连接
author: John
feature: Workfront API
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: a62ae524f922326811423cd17d0656920b7cc9d3
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---


# 测试Webhook连接

要验证文档WebHook实施是否正常工作，请在此部分中运行手动测试。 这些步骤将通过Adobe Workfront Web界面并间接点击您Webhook实施的端点。

## 先决条件

运行测试需要满足以下先决条件：

* 启用了高级文档管理(ADM)的Workfront帐户

* 具有系统管理员权限的此帐户的Workfront用户

* 具有可供Workfront访问的HTTP端点的文档Webhook实例

这些测试还假定您的Document Webhook实例已注册。 (您可以在Workfront中的设置>文档>自定义集成下注册您的实例。)

**测试1:为用户配置文档Webhook服务**

测试基于OAuth的Webhook提供程序的身份验证URL和令牌端点URL。

1. 在Workfront中，通过单击顶部导航栏中的“文档”链接，转到主“文档”页面。
1. 单击“添加文档”下拉列表，然后在“添加服务”下选择“文档Webhook服务”。
1. （仅限OAuth服务）完成上一步后，您将在弹出窗口中看到服务的OAuth2身份验证页面加载。 (注：系统可能会提示您先登录您的服务。) 在身份验证页面中，通过单击信任或允许按钮，授予Workfront对用户帐户的访问权限。
1. 验证您的服务是否已添加到添加文档下拉列表中。 如果最初未看到，请尝试刷新浏览器。

**测试2:将文档链接到Workfront测试以下端点：/files， /metadata**

1. 在Workfront中，通过单击顶部导航栏中的“文档”链接，转到主“文档”页面。
1. 在“添加文档”下选择您的文档Webhook服务。
1. 在模式窗口中，导航到文件夹结构。
1. 验证您是否能够导航文件夹结构。
1. 选择文档并将其链接到Workfront

**测试3:导航到内容管理系统中的文档**

测试以下端点：/metadata（特别是viewLink）

1. 将文档链接到Workfront
1. 选择文档并单击“打开”链接。
1. 验证文档是否在新选项卡中打开。

**测试4:导航到内容管理系统中的文档（通过登录）**

测试以下端点：/metadata（特别是viewLink）

1. 确保您已注销内容管理系统。
1. 将文档链接到Workfront。
1. 选择文档并单击“打开”链接。
1. 验证内容管理系统的登录屏幕是否在新选项卡中加载。
1. 登录并验证您是否已转到文档

**测试5:从内容管理系统下载文档**

测试以下端点（特别是下载链接）：/metadata 

1. 将文档链接到Workfront。
1. 选择文档，然后单击Download（下载）链接。
1. 确认开始下载。

**测试6:搜索内容**

测试以下端点：/search

1. 在Workfront中，通过单击顶部导航栏中的“文档”链接，转到主“文档”页面。
1. 在“添加文档”下选择您的文档Webhook服务。
1. 在模式窗口中，执行搜索。
1. 验证搜索结果是否正确。

**测试7:将文档从Workfront发送到内容管理系统**

测试以下端点：/files， /uploadInit， /upload

1. 在Workfront中，通过单击顶部导航栏中的“文档”链接，转到主“文档”页面。
1. 从计算机将文档上传到Workfront
1. 转到文档详细信息页面
1. 从文档操作下拉列表中，在发送到……下选择您的文档Webhook服务
1. 转到所需的目标文件夹，然后单击保存按钮。
1. 确认文档已上传到内容管理系统中的正确位置。

**测试8:在Workfront中查看缩略图**

测试以下端点：/缩略图

1. 将文档链接到Workfront。
1. 在列表中选择文档。
1. 验证缩略图是否显示在右侧面板中。

**测试9:获取内容字节**

测试以下端点：/download

1. 将文档链接到Workfront。
1. 转到文档详细信息页面。
1. 通过选择文档操作>发送到…… > Workfront，将文档发送到Workfront。 这将在Workfront中创建新文档版本。
1. 单击下载链接，从Workfront下载文档。

**测试10:刷新访问令牌（仅OAuth2 Webhook提供程序）**

测试以下端点：令牌端点URL

1. 为用户配置文档Webhook服务
1. 通过1)等待用户的访问令牌超时或2)在外部系统中手动使其失效，来使用户的访问令牌失效。
1. 在Workfront中刷新访问令牌。 例如，您可以通过将文档链接到Workfront来执行此操作。 如果您能够导航到并链接文档，则会知道访问令牌已成功刷新。

>[!NOTE]
>
>目前，“发送到……”不适用于链接的文档。 这将由Workfront添加。 您可以使用REST客户端(如Postman)手动点击端点来测试/download端点。 或者，可以通过生成数字校样来测试/download端点。 要启用数字校样，请联系Workfront。
