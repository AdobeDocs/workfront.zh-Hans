---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 使用AI生成场景区段
description: 您可以输入文本提示来创建针对该提示配置的HTTP模块。
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: 5de5b96bc74ce9b819acfa7b5f16652509ccade1
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# 使用AI生成场景区段

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>由于此功能位于Beta中，因此仅对某些Workfront用户可用。

您可以使用AI输入文本提示，描述需要场景的一部分执行的操作。 然后，Fusion将生成将执行这些操作的模块，您可以在场景中使用这些模块。

与从AI生成的任何内容一样，我们建议您仔细检查并测试生成的模块，以确保它们按预期执行。

## 当前支持的AI模块应用程序

Fusion AI当前可以生成连接到以下应用程序的模块：

* Adobe Firefly
* Azure OpenAI
* Microsoft Graph
* Adobe Workfront规划
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

1. 开始添加模块，并从应用程序列表中选择&#x200B;**使用AI生成**。

   或

   单击方案编辑器页面底部附近的“使用AI生成”图标![使用AI生成](assets/generate-with-ai-icon-beta.png)。

   将打开AI助手面板。
1. 在框中输入文本提示。

   有关提示的提示，请参阅本文中的[创建文本提示的提示](#tips-for-creating-text-prompts)。

   AI Assistant生成模块或模块集。
1. （视情况而定）如有必要，请将应用程序的API令牌添加到模块中。
1. 检查模块，确保已针对相应的应用程序和操作配置它们。
1. （视情况而定）如果生成的场景部分未附加到场景，请将其拖动到适当位置。

我们建议测试这些模块以确保它们按预期执行。

## 创建文本提示的提示

文本提示应至少包括以下信息：

* 要连接的应用程序
* 要执行的一个或多个操作

>[!IMPORTANT]
>
>您可以一次生成多个模块，但一次只能为一个应用程序生成模块。

>[!INFO]
>
>**示例**：
>
>* `Delete the records 'xyz-123', 'xyz-456', 'xyz-789' from Adobe Workfront Planning`
>这包括应用程序`Workfront Planning`和操作`delete records`。 此提示将创建三个模块，每个要删除的记录各一个。
>* `Change campaign summary of the record 'xyz-123' from Adobe Workfront Planning`
>这包括应用程序`Workfront Planning`和操作`change campaign summary`。
>* `Get all field details in the record type with ID 'test-record' from Adobe Workfront Planning`
>这包括应用程序`Workfront Planning`和操作`get field details`。
>
>以下示例不正确：
>
>* `Generate an image in Adobe Firefly and upload it to Dropbox`
>
>    此示例不正确，因为它包含多个应用程序

创建文本提示时，请考虑以下事项：

* 使用直接、简单的语言。
* 检查并测试您的模块。 如果它未按预期执行，请优化您的提示并重试。
