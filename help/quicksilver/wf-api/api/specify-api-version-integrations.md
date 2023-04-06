---
content-type: api
navigation-topic: api-navigation-topic
title: 在集成中指定API版本
description: 在集成中指定API版本
author: Becky
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 2b9eacc9b2c8f499cdd1794a55879a56224051c8
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# 在集成中指定API版本

所有Adobe Workfront URI应在URI的“attask/api”部分之后引用API的特定版本。 以下示例调用版本15.0:

`attask/api/v15.0/<objectName>/<objectId>`

请确保您的所有集成都调用了当前支持的Workfront API。

## Workfront API的发布和弃用计划

新版API会定期发布，通常每年发布两次。 每个版本在其发行日期后三年内受支持，在已弃用状态下再受一年支持，即版本可用但不受支持。

有关Workfront API的发行频率和弃用计划的更多信息，请参阅 [API版本控制和支持计划](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* API的默认版本设置为最新版本。 任何未指定版本的API调用都将使用默认版本。 每次Workfront发布新版API时，默认版本都将更新至最新版本。 **因此，在发布新版本的Workfront API后，应检查使用默认版本的任何API调用，以确保仍支持该功能。**
>
>* 如果贵组织当前使用默认API，则Workfront管理员已收到公告中心消息，其中包含有关默认API的进一步说明。
>
>要查看API的最新版本，请参阅 [API版本控制和支持计划](../../wf-api/api/api-version-support-schedule.md).


## 确定您使用的API版本

您可以通过检查发送到Workfront API的HTTP请求的URI来确定您所使用的API的版本。 以下示例显示了一个Workfront请求URI，该URI指定了API的版本15:

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

如果URI未指定版本，则它使用API的默认版本，如以下示例所示：

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> 在URI中未指定API版本的集成会自动路由到API的默认版本。

## 更新集成以使用支持的API版本

构建或维护Workfront集成时，您应该包含一种方法，用于动态更新API版本和其他可能发生更改的属性（例如您的API密钥）。

要提高集成更新的效率，您应考虑以下有关记录集成值的建议：

* 在您保持更新的属性文件中存储值，但以未来更改为条件
* 创建Web服务以实时管理资产
* 将属性值存储到应用程序可读取的数据存储中

在设计Workfront集成时考虑到这一点，可在这些值不可避免地发生更改时，轻松地需要大量开发工作。
