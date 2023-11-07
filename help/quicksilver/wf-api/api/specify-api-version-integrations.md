---
content-type: api
navigation-topic: api-navigation-topic
title: 在您的集成中指定API版本
description: 在您的集成中指定API版本
author: Becky
feature: Workfront API
role: Developer
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# 在您的集成中指定API版本

所有Adobe Workfront URI都应在URI的“attask/api”部分后面引用API的特定版本。 以下示例调用版本15.0：

`attask/api/v15.0/<objectName>/<objectId>`

请确保您的所有集成都调用当前支持的Workfront API。

## Workfront API的发布和弃用计划

API的新版本会定期发布，通常每年发布两次。 每个版本在发布日期后支持三年，并且还有一个年处于已弃用状态，该状态表示版本可用但不受支持。

有关Workfront API发行节奏和弃用计划的更多信息，请参阅 [API版本控制和支持计划](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* API的默认版本设置为最新版本。 任何未指定版本的API调用都将使用默认版本。 每当Workfront发布API的新版本时，默认版本都将更新为最新版本。 **因此，在发布Workfront API的新版本后，应该检查任何使用默认版本的API调用，以确保仍然支持该功能。**
>
>* 如果您的组织当前正在使用默认API，则Workfront管理员已收到Announcement Center消息，该消息包含有关默认API的更多说明。
>
>要查看API的最新版本，请参阅 [API版本控制和支持计划](../../wf-api/api/api-version-support-schedule.md).


## 确定您使用的API版本

您可以通过检查发送到Workfront API的HTTP请求的URI来确定正在使用的API版本。 以下示例显示了一个指定API版本15的Workfront请求URI：

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

如果URI未指定版本，则它使用的是API的默认版本，如以下示例所示：

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> 未在URI中指定API版本的集成会自动路由到API的默认版本。

## 更新集成以使用支持的API版本

在构建或维护Workfront集成时，您应该包括用于动态更新API版本和其他可能发生更改的属性（例如API密钥）的方法。

为了提高集成更新效率，您应该考虑以下有关记录集成值的建议：

* 根据未来更改将值存储在您保持更新的属性文件中
* 创建Web服务以实时管理资产
* 将属性值存储在应用程序可读取的数据存储中

在设计Workfront集成时，如果上述值不可避免地发生变化，那么通过考虑上述因素，您便无需进行大量开发工作。
