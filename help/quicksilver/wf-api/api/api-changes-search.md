---
filename: api-changes-search
content-type: api
keywords: 对象，状态，搜索，最佳，实践，响应
navigation-topic: api-navigation-topic
title: '核心API更改：状态搜索响应'
description: 更改Workfront存储状态对象的方式。
feature: Workfront API
role: Developer
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 1%

---

# 核心API更改：状态搜索响应

Workfront存储状态对象的方式已发生更改。 这些更改不会影响发出状态搜索请求的方式，但将影响API请求返回的响应，API请求通过返回不完整的组状态列表来搜索状态对象。

## 最佳实践

为了可靠地获取组可用的状态完整列表，以下请求被视为最佳实践。

>[!NOTE]
>
>建议所有用户使用这些请求结构，无论集群是否进行了状态搜索更改。

对于项目组状态：

>**示例:**

```
/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

对于任务组状态：

>**示例:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

对于问题组状态：

>**示例:**

```
/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

这三个端点都接受 **includeHidden=true** 以获取给定组的隐藏项目/任务/问题状态的参数。 在这些最佳实践示例之后对状态搜索查询建模将确保每个响应中包含所有组状态信息。

以下是向任务组发出的状态搜索查询示例，该任务组包括系统级别的锁定状态 **Custom_1** 和已解锁状态 **Custom_2**：

>**示例:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

使用此格式可确保您的响应将包括以下所有内容：

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

## 了解对旧版状态搜索查询所做的更改

在旧式系统下，状态搜索查询将复制可用于查询中包含的所有组的所有系统状态。 然后，旧版响应将包括查询中每个组可用的所有系统状态和组级别状态。

例如，此查询（不遵循当前推荐的最佳实践）：

>**示例:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

在旧版系统中将具有以下响应，其中包括所有对象状态：

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

但是，在对存储和使用状态的方式进行更新后，状态不会为组复制，而是由系统级别的每个组继承。 因此，搜索API查询只会读取与特定组直接关联的那些状态，因此响应将包含系统锁定和未锁定状态，但仅适用于添加相关状态后创建的组。

更新旧版系统后，如果未使用更新后的最佳实践方法进行状态搜索查询，将导致响应中返回的组状态列表不完整。

以下是更新旧系统后，此过时的请求结构返回的示例：

>**示例:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

请注意，此响应仅包括组特定的状态，而不包括在系统级别声明的那些状态：

```
{
  "data": [
    {
      "color": "8BC34A",
      "equatesWith": "NEW",
      "groupID": "602d286d000004fc8f53942de697a868",
      "label": "Custom_2",
      "objCode": "CSTEM",
      "value": "MMI"
    }
  ]
}
```
