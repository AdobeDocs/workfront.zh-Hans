---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 使用人工智能生成模块
description: 您可以输入文本提示来创建针对该提示配置的HTTP模块。
author: Becky
feature: Workfront Fusion
source-git-commit: c80f9ab6d10aa9067b995c99107f98301fa17872
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 1%

---

# 使用人工智能生成模块

<!--DO NOT DELETE - linked through CSH-->

您可以使用AI输入文本提示，描述您需要模块执行的操作。 然后，Fusion将生成一个HTTP模块，该模块将连接到所需API的正确端点。

与从AI生成的任何内容一样，我们建议您仔细检查并测试生成的模块，以确保其按预期执行。

## 当前支持的AI模块应用程序

Fusion AI当前可以生成连接到以下应用程序的模块：

* Adobe经理
* Adobe Analytics
* Adobe PDF服务
* AdobeMarketo
* AdobeFrame.io
* Dropbox
* NetSuite
* Google 日历
* 阿特拉西安·吉拉
* GitLab
* Spotify
* 比特桶
* OpenAI
* Slack

## 生成模块

1. 添加模块并选择 **使用AI生成** 从应用程序列表中。

   或

   右键单击方案编辑器的空白区域，然后选择 **使用AI生成**.
1. 在框中输入文本提示。

   有关提示的信息，请参阅 [创建文本提示的提示](#tips-for-creating-text-prompts) 本文章中。
1. 将应用程序的API令牌添加到模块中。
1. 检查模块，确保看起来已针对相应的应用程序和操作对该模块进行了配置。
1. （视情况而定）如果模块未附加到场景，请将其拖动到适当位置。

我们建议测试模块，以确保生成的模块按预期执行。

## 创建文本提示的提示

文本提示应至少包括以下信息：

* 要连接的应用程序
* 要执行的操作

>[!INFO]
>
>**示例**：
>
>* `Retrieve a list of my calendars from Google Calendar`
>
>   这包括应用程序 `Google Calendar` 和操作 `Retrieve a list of my calendars`.
>
>* `Retrieve popular songs from Spotify`
>
>   这包括应用程序 `Spotify` 和操作 `Retrieve popular songs`.

创建文本提示时，请考虑以下事项：

* 由于每个Fusion模块只执行一项操作，因此您的文本提示应描述一项特定操作。
* 使用直接、简单的语言。
* 检查并测试您的模块。 如果它未按预期执行，请优化您的提示并重试。



