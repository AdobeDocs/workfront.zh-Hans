---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: “Workfront Fusion版本活动：2021年1月11日一周”
description: 本页介绍2021年1月11日这一周Adobe Workfront Fusion中所做的所有增强功能。
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 2439e2a7-9404-433a-bd71-a7776042d8a0
hidefromtoc: true
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 0%

---

# Workfront Fusion版本活动： 2021年1月11日开始的一周

本页介绍2021年1月11日这一周Adobe Workfront Fusion中所做的所有增强功能。

有关所有最近更改的列表，请参阅 [Adobe Workfront Fusion版本活动](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

有关Workfront Fusion中最近的错误修复列表，请参阅 [Workfront维护更新](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) 页面，并检查标记为Workfront Fusion维护更新的任何更新。

## 扩展连接器和模块现已可用

您现在可以使用Workfront Fusion连接到Widen帐户。 通过“扩展”模块，您可以：

* 向收藏集添加资产或从收藏集中删除资产
* 下载或上传文件
* 读取或更新资产元数据
* 根据您指定的条件搜索资产
* 检索收藏集中的资产列表
* 执行自定义API调用。

有关详细信息，请参阅 [扩展模块](../../../workfront-fusion/apps-and-their-modules/widen-modules.md).

## Datadog连接器和模块现已可用

您现在可以使用Workfront Fusion连接到Data Cloud帐户。

通过使用Data Cloud模块，您可以：

* 帖子时间点
* 执行自定义API调用

有关Data Cloud模块的信息，请参阅 [数据模块](../../../workfront-fusion/apps-and-their-modules/datadog-modules.md).

## Cvent连接器和模块现已可用

您现在可以使用Workfront Fusion 2.0连接到Cevent帐户。

通过Cevent模块，您可以：

* 创建会议请求
* 读取联系人、事件或被邀请者等记录
* 根据您指定的条件列出记录
* 注册或向特定事件添加被邀请者
* 更新或删除联系人
* 进行自定义API调用

有关可用Cvent模块的信息，请参阅 [事件模块](../../../workfront-fusion/apps-and-their-modules/cvent-modules.md).

## Microsoft Dynamics 365连接器和模块现已可用

您现在可以使用Workfront Fusion 2.0连接到Microsoft Dynamics 365帐户。 通过Microsoft Dynamics 365模块，您可以：

* 在Microsoft Dynamics 365中添加或更新记录时会触发方案
* 创建、读取、更新或删除Microsoft Dynamics 365记录
* 执行自定义API调用

有关可用的Microsoft Dynamics 365模块的信息，请参阅 [Microsoft Dynamics 365模块](../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

## DocuSign连接器和模块现已可用

您现在可以使用Workfront Fusion 2.0连接到您的Document帐户。 使用文档模块，您可以：

* 当信封更改其状态时会触发情景
* 创建信封
* 读取、发送或添加收件人到现有信封
* 在文档中添加或修改自定义字段
* 将文档下载为文档
* 将文件上传到信封
* 执行自定义API调用

有关更多信息，请参阅 [DocuSign模块](../../../workfront-fusion/apps-and-their-modules/docusign-modules.md).

## 搜索方案执行历史记录

我们为您提供了更方便的方法，让您能够更轻松地从以前的方案执行中查找特定信息。 Fusion新的全文搜索功能使得可以搜索包中包含的任何数据的执行历史记录。 例如，要确定是哪个执行创建了特定任务，您可以使用全文搜索来搜索该任务ID。

以前，需要单独查看每个执行，才能找到特定的执行信息。

有关更多信息，请参阅 [在Adobe Workfront Fusion中查看方案的执行历史记录](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## Fusion 2.0数据存储的更新

为了更便于您自定义数据存储，我们添加了一些新功能。 现在，当您查看数据存储时，可以：

* 拖放以重新排序列
* 编辑单个单元格
* 添加多行

有关数据存储的更多信息，请参阅 [数据存储模块](../../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

## 通过HTTP连接器发出API密钥授权请求

为了增加访问API的方式的灵活性，我们向HTTP连接器中添加了新模块。 现在，当您访问的Web服务需要使用API密钥时，您可以使用HTTP连接器发出请求。

有关更多信息，请参阅 [HTTP模块](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

## 映射面板中提供的新函数

为了帮助您自定义和简化模块中的公式，我们添加了一些新函数。

* 此

   ```
   omit
   ```

   函数是一个常规函数，它忽略对象的给定键并返回其余键。
* 此

   ```
   pick
   ```

   函数是一个常规函数，仅从对象中选取给定的键。
* 此

   ```
   escapeMarkdown
   ```

   函数是一个字符串函数，可对文本中的所有Markdown标记进行转义。

有关省略和选取函数的详细信息，请参阅 [Adobe Workfront Fusion中的一般函数](../../../workfront-fusion/functions/general-functions.md).

有关escapeMarkdown函数的更多信息，请参阅 [Adobe Workfront Fusion中的字符串函数](../../../workfront-fusion/functions/string-functions.md).
