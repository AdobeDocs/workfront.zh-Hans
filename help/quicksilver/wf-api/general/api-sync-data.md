---
content-type: api
keywords: API，数据，同步，日志，条目，对象
navigation-topic: general-api
title: 使用API同步程序和服务的数据
description: 使用API同步程序和服务的数据
author: Becky
feature: Workfront API
role: Developer
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# 使用API同步程序和服务的数据

以下是您利用API同步程序和服务的数据的几种常用方法。

## 近乎实时的更新

Adobe Workfront使用“事件订阅”（通常称为Webhook）通过API将有关受支持对象和操作的近乎实时更新发送到所需的端点。 您可以预期在5秒内收到有关新对象和操作的更新，但平均更新大约会在1秒后到达。 有关支持的对象类型、支持的操作类型、技术细节以及如何设置事件订阅的示例的其他信息，请参阅[事件订阅API](../../wf-api/general/event-subs-api.md)和[事件订阅交付要求](../../wf-api/general/setup-event-sub-endpoint.md)。

## 批量更新

批量更新是一种通过定期向Workfront服务器发出请求来配置系统以进行更新的方法。 有很多方法可以做到这一点，但通常流程包括让您的服务向Workfront API服务器发出请求，并搜索自上次请求调用以来创建或修改的对象。 有关可能的请求调用和有用参数的信息，请参阅[API基础知识](../../wf-api/general/api-basics.md)文章中的[GET行为](../../wf-api/general/api-basics.md#get-behavior)部分。

在为批量更新设置服务时，请谨记以下一些重要事项：

### 输入日期

输入日期是使用ISO 8601格式存储的。 该标准包括日期、时间和时区信息。

**示例：** ISO 8601日期格式

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

创建对象的日期和上次修改对象的日期分别存储为“entryDate”和“lastUpdateDate”。 有关Workfront对象、其关联字段和字段名称的深入信息，请参阅[API资源管理器](../../wf-api/general/api-explorer.md)。 请注意，任何给定的Workfront对象的entryDate都不会更改，其中lastUpdatedDate在每次修改对象时都会更改。

**示例：**&#x200B;利用&#x200B;**lastUpdateDate**&#x200B;字段请求问题对象的GET。 此请求将返回自指定日期以来更新的所有问题。

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v15.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### 日志条目对象

如果您希望获取有关对象上特定字段的更改，则可以查询“Journal Entry”对象。 可以将Workfront日志条目对象设置为在修改特定对象字段时记录有关这些字段的信息，请参阅[配置系统更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md)以获取更多详细信息。

将某个字段设置为记录为日志条目对象的一部分时，每次修改该字段时将创建相应的日志条目。 然后，您可以使用类似于以下内容的API调用查询Journal Entry对象：

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v15.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>“entryDate”用于查看更改的日志条目，而不是查看已更改的对象本身。
