---
filename: api-changes-search
content-type: api
keywords: 对象，状态，搜索，最佳，实践，响应
navigation-topic: api-navigation-topic
title: “核心API更改：状态搜索响应
description: 更改了Workfront存储状态对象的方式。
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 1%

---

# 核心API更改：状态搜索响应

已更改Workfront存储状态对象的方式。 这些更改不会影响状态搜索请求的发出方式，但会影响API请求返回的响应，这些API请求包括通过返回组状态的不完整列表来搜索状态对象。

## 最佳实践

为了可靠地获取群组可用状态的完整列表，以下请求被视为最佳实践。

>[!NOTE]
>
>无论是否对您的群集进行了状态搜索更改，都建议所有用户使用这些请求结构。

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

所有这三个端点都接受 **includeHidden=true** 参数来获取给定组的隐藏项目/任务/问题状态。 根据这些最佳实践示例对状态搜索查询进行建模，可确保每个响应都包含所有组状态信息。

以下是对包含系统级别锁定状态的任务组进行状态搜索查询的示例 **Custom_1** 和未锁定状态 **Custom_2**:

>**示例:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

使用此格式可确保您的响应将包含以下所有内容：

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

在旧版系统下，状态搜索查询将复制查询中包含的所有组可用的所有系统状态。 然后，旧版响应将包含查询中每个群组可用的所有系统状态和群组级别状态。

例如，此查询（不遵循当前推荐的最佳实践）：

>**示例:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

在旧版系统下将具有以下响应，其中包括所有对象状态：

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

但是，在对状态的存储和使用方式进行了更新后，状态不会复制组，而是由系统级别的每个组继承。 因此，搜索API查询只会读取与特定组直接关联的状态，因此响应包含系统锁定状态和未锁定状态，但仅适用于在添加相关状态后创建的组。

更新旧版系统后，如果未能使用更新的最佳实践方法进行状态搜索查询，则响应中将返回组状态列表不完整。

以下是旧版系统更新后，此过时的请求结构返回的结果示例：

>**示例:**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

请注意，此响应仅包含特定于组的状态，并且不包含在系统级别声明的状态：

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
