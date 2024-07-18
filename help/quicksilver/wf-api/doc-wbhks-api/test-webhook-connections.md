---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 测试Webhook连接
description: 测试Webhook连接
author: Becky
feature: Workfront API
role: Developer
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---


# 测试Webhook连接

要验证文档webhook实施是否正常工作，请运行本节中的手动测试。 这些步骤通过Adobe Workfront Web界面间接点击webhook实施的端点。

## 先决条件

运行测试需要以下先决条件：

* 启用了高级文档管理(ADM)的Workfront帐户

* 此帐户中拥有系统管理员权限的Workfront用户

* 带有Workfront可访问的HTTP端点的文档Webhook实例

这些测试还假定您的Document Webhook实例已注册。 (您可以在设置>文档>自定义集成下在Workfront中注册实例。)

**测试1：为用户预配Document Webhook服务**

测试基于OAuth的Webhook提供程序的身份验证URL和令牌端点URL。

1. 在Workfront中，单击顶部导航栏中的“文档”链接，转到“文档”主页面。
1. 单击添加文档下拉列表，然后在添加服务下选择文档Webhook服务。
1. （仅限OAuth服务）完成上一步后，您将在弹出窗口中看到服务的OAuth2身份验证页面加载。 （注意：系统可能会提示您先登录服务。） 在身份验证页面中，通过单击信任或允许按钮授予Workfront对用户帐户访问权限。
1. 验证您的服务是否已添加到添加文档下拉列表中。 如果您最初没有看到该页面，请尝试刷新浏览器。

**测试2：将文档链接到Workfront测试以下端点： /files、/metadata**

1. 在Workfront中，单击顶部导航栏中的“文档”链接，转到“文档”主页面。
1. 在“添加文档”下选择文档Webhook服务。
1. 在该模式中，导航浏览文件夹结构。
1. 验证您是否能够导航文件夹结构。
1. 选择文档并将其链接到Workfront

**测试3：导航到内容管理系统中的文档**

测试以下端点： /metadata （尤其是viewLink）

1. 将文档链接到Workfront
1. 选择文档并单击“打开”链接。
1. 验证文档是否在新选项卡中打开。

**测试4：导航到内容管理系统（登录时）中的文档**

测试以下端点： /metadata （尤其是viewLink）

1. 确保您已从内容管理系统注销。
1. 将文档链接到Workfront。
1. 选择文档并单击“打开”链接。
1. 验证内容管理系统的登录屏幕是否在新选项卡中加载。
1. 登录并验证您是否已转到文档

**测试5：从内容管理系统下载文档**

测试以下端点（特别是下载链接）： /metadata 

1. 将文档链接到Workfront。
1. 选择文档并单击“下载”链接。
1. 验证下载是否开始。

**测试6：搜索内容**

测试以下端点： /search

1. 在Workfront中，单击顶部导航栏中的“文档”链接，转到“文档”主页面。
1. 在“添加文档”下选择文档Webhook服务。
1. 在该模式窗口中，执行搜索。
1. 验证搜索结果是否正确。

**测试7：将文档从Workfront发送到内容管理系统**

测试以下端点： /files、/uploadInit、/upload

1. 在Workfront中，单击顶部导航栏中的“文档”链接，转到“文档”主页面。
1. 将文档从计算机上传到Workfront
1. 转到文档详情页面
1. 从“文档操作”下拉列表中，选择“发送到……”下的Document Webhook服务
1. 转到所需的目标文件夹，然后单击保存按钮。
1. 验证文档是否已上传到内容管理系统中的正确位置。

**测试8：在Workfront中查看缩略图**

测试以下端点： /thumbnail

1. 将文档链接到Workfront。
1. 选择列表中的文档。
1. 验证缩略图是否显示在右侧面板中。

**测试9：获取内容字节**

测试以下端点： /download

1. 将文档链接到Workfront。
1. 转到文档详情页面。
1. 通过选择“文档操作”>“发送到……”>“Workfront”，将文档发送到Workfront。 这将在Workfront中创建一个新文档版本。
1. 通过单击下载链接，从Workfront下载文档。

**测试10：刷新访问令牌（仅限OAuth2 Webhook提供程序）**

测试以下端点：令牌端点URL

1. 为用户预配Document Webhook服务
1. 通过1 )等待用户访问令牌超时或2)在外部系统中手动使其失效，来使其失效。
1. 在Workfront中刷新访问令牌。 例如，您可以将文档链接到Workfront中来执行此操作。 如果您能够导航到文档并进行链接，则您将知道访问令牌已成功刷新。

>[!NOTE]
>
>目前，发送至……不可用于链接的文档。 Workfront将添加此参数。 您可以通过使用REST客户端(例如Postman)手动点击端点来测试/download端点。 或者，可以通过生成数字验证来测试/download端点。 要启用数字校对，请联系Workfront。
