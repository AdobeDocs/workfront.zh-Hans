---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 'Workfront Fusion发布活动：2021年1月11日当周'
description: 本页介绍了2021年1月11日这一周在Adobe Workfront Fusion中所做的所有增强。
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 2439e2a7-9404-433a-bd71-a7776042d8a0
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Workfront Fusion发行活动： 2021年1月11日起的一周

本页介绍了2021年1月11日这一周在Adobe Workfront Fusion中所做的所有增强。

有关所有最近更改的列表，请参阅[Adobe Workfront Fusion发行活动](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)。

有关Workfront Fusion中最近的错误修复列表，请参阅[Workfront维护更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html)页面，并检查任何标记为Workfront Fusion维护更新的更新。

## 现在提供加宽连接器和模块

您现在可以使用Workfront Fusion连接到Widen帐户。 使用Widen模块，您可以：

* 在收藏集中添加或删除资源
* 下载或上传文件
* 读取或更新资源元数据
* 根据您指定的条件搜索资源
* 检索收藏集中的资产列表
* 执行自定义API调用。

有关详细信息，请参阅[加宽模块](../../../workfront-fusion/apps-and-their-modules/widen-modules.md)。

## Datadog连接器和模块现已可用

您现在可以使用Workfront Fusion连接到Datadog帐户。

使用Datadog模块，您可以：

* Post时间系列点
* 执行自定义API调用

有关Datadog模块的信息，请参阅[Datadog模块](../../../workfront-fusion/apps-and-their-modules/datadog-modules.md)。

## Cvent连接器和模块现已可用

您现在可以使用Workfront Fusion 2.0连接到Cvent帐户。

使用Cvent模块，您可以：

* 创建会议请求
* 读取记录，如联系人、活动或受邀者
* 根据您指定的条件列出记录
* 在特定活动中注册或添加被邀请者
* 更新或删除联系人
* 进行自定义API调用

有关可用Cvent模块的信息，请参阅[Cvent模块](../../../workfront-fusion/apps-and-their-modules/cvent-modules.md)。

## Microsoft Dynamics 365连接器和模块现已推出

您现在可以使用Workfront Fusion 2.0连接到Microsoft Dynamics 365帐户。 使用Microsoft Dynamics 365模块，您可以：

* 在Microsoft Dynamics 365中添加或更新记录时触发方案
* 创建、读取、更新或删除Microsoft Dynamics 365记录
* 执行自定义API调用

有关可用的Microsoft Dynamics 365模块的信息，请参阅[Microsoft Dynamics 365模块](../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md)。

## DocuSign连接器和模块现已可用

您现在可以使用Workfront Fusion 2.0连接到Docusign帐户。 通过Docusign模块，您可以：

* 在信封更改其状态时触发方案
* 创建信封
* 在现有信封中读取、发送或添加收件人
* 添加或修改文档中的自定义字段
* 将文档下载为已存档
* 将文件上载到信封
* 执行自定义API调用

有关详细信息，请参阅[DocuSign模块](../../../workfront-fusion/apps-and-their-modules/docusign-modules.md)。

## 搜索场景执行历史记录

我们使您更容易地从以前的场景执行中查找特定信息。 Fusion的新全文搜索功能可用于搜索捆绑包中包含的任何数据的执行历史记录。 例如，要确定哪个执行创建了特定任务，您可以使用全文搜索来搜索该任务ID。

以前，查找特定的执行信息需要分别查看每个执行。

有关详细信息，请参阅[在Adobe Workfront Fusion中查看方案的执行历史记录](../../../workfront-fusion/scenarios/view-scenario-execution-history.md)。

## Fusion 2.0数据存储的更新

为了让您更轻松地自定义数据存储，我们添加了一些新功能。 现在，当您查看数据存储时，您可以：

* 拖放以重新排序列
* 编辑单个单元格
* 添加多行

有关数据存储区的详细信息，请参阅[数据存储模块](../../../workfront-fusion/apps-and-their-modules/data-store-modules.md)。

## 通过HTTP连接器发出API密钥授权请求

为了提高访问API方式的灵活性，我们在HTTP连接器中添加了一个新模块。 现在，当您要访问的Web服务需要使用API密钥时，可以使用HTTP连接器发出请求。

有关详细信息，请参阅[HTTP模块](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)。

## 映射面板中可用的新函数

为了帮助您自定义和简化模块中的公式，我们添加了一些新函数。

* 此

  ```
  omit
  ```

  函数是一个常规函数，它省略了对象的给定键并返回其余键。
* 此

  ```
  pick
  ```

  function是一个常规函数，只从对象中选取给定的键。
* 此

  ```
  escapeMarkdown
  ```

  函数是一个字符串函数，可转义文本中的所有Markdown标记。

有关omit和pick函数的更多信息，请参阅[Adobe Workfront Fusion中的常规函数](../../../workfront-fusion/functions/general-functions.md)。

有关escapeMarkdown函数的详细信息，请参阅Adobe Workfront Fusion中的[字符串函数](../../../workfront-fusion/functions/string-functions.md)。
