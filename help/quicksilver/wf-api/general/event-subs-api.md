---
content-type: api
navigation-topic: general-api
title: 事件订阅API
description: 事件订阅API
author: Becky
feature: Workfront API
role: Developer
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: 5b984451d19ed0381c75c4fa19f3eba16804fbf5
workflow-type: tm+mt
source-wordcount: '2666'
ht-degree: 3%

---


# 事件订阅API

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

当事件订阅支持的Adobe Workfront对象上发生操作时，您可以将Workfront配置为将响应发送到所需的端点。 这意味着第三方应用程序在更新发生后不久即可通过Workfront API接收来自Workfront交互的更新。 通常，您可以预期在记录数据更改后的5秒内收到webhook通知。 平均而言，客户会在距记录的数据更改不到1秒的时间内收到webhook通知。

由于事件订阅将数据发送到其他服务，因此它们通过命令而不是通过Workfront应用程序进行管理。

列入允许列表要通过防火墙接收事件订阅负载，必须将以下IP地址添加到您的：

对于欧洲的客户：**&#x200B;**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**对于位于欧洲以外地区的客户：**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

以下主题支持事件订阅API：

## 事件订阅支持的对象

事件订阅支持以下Workfront对象。

* 审批
* 审批阶段
* 审批阶段参与者
* 任务分配
* 公司
* 仪表板
* 文档
* 费用
* 字段
* 小时
* 问题
* 注释
* 项目组合
* 项目群
* 项目
* 记录
* 记录类型
* 报告
* 任务
* 模板
* 时间表
* 用户
* Workspace

有关事件订阅对象支持的字段列表，请参阅[事件订阅资源字段](../../wf-api/api/event-sub-resource-fields.md)。

## 事件订阅身份验证

要创建、查询或删除事件订阅，您的Workfront用户需要满足以下条件：

* 要使用事件订阅，需要具有“系统管理员”访问级别。
* 需要`sessionID`标头才能使用事件订阅API

  有关详细信息，请参阅[API基础知识](api-basics.md#authentication)中的[身份验证](api-basics.md)。

## 形成订阅资源

订阅资源包含以下字段。

* objId（可选）

   * **字符串** — 为其触发事件的指定objCode的对象的ID。 如果未指定此字段，则用户会收到指定类型的所有对象的事件。

* 对象代码（必需）

   * **字符串** — 订阅更改的对象的对象代码。 下表中列出了objCode的可能值。

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <thead> 
       <tr> 
        <th><p>对象</p></th> 
        <th><p>对象代码</p></th> 
       </tr> 
      </thead> 
      <tbody> 
       <tr> 
        <td scope="col">审批</td> 
        <td scope="col"><p>审批</p></td> 
       </tr> 
       <tr> 
        <td scope="col">审批阶段</td> 
        <td scope="col"><p>approval_stage</p></td> 
       </tr> 
       <tr> 
        <td scope="col">审批阶段参与者</td> 
        <td scope="col"><p>approval_stage_participant</p></td> 
       </tr> 
       <tr> 
        <td scope="col">任务分配</td> 
        <td scope="col"><p>分配</p></td> 
       </tr> 
       <tr> 
        <td scope="col">公司 </td> 
        <td scope="col"><p>CMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">仪表板</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>文档</p></td> 
        <td scope="col">DOCU </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>费用</p></td> 
        <td scope="col">展开</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>字段</p></td> 
        <td scope="col"><p>字段</p></td> 
       </tr> 
      <tr> 
        <td scope="col"><p>小时</p></td> 
        <td scope="col">HOUR</td> 
       </tr> 
       <tr> 
        <td scope="col">问题</td> 
        <td scope="col"><p>OPTASK</p></td> 
       </tr> 
       <tr> 
        <td scope="col">注释</td> 
        <td scope="col">注释</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>项目组合</p></td> 
        <td scope="col"><p>端口</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>项目群</p></td> 
        <td scope="col"><p>PRGM</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>项目</p></td> 
        <td scope="col"><p>项目</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>记录</p></td> 
        <td scope="col"><p>记录</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>记录类型</p></td> 
        <td scope="col"><p>记录类型</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>报告</p></td> 
        <td scope="col"><p>PTLSEC</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>任务</p></td> 
        <td scope="col"><p>任务</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>模板</p></td> 
        <td scope="col"><p>模板</p></td> 
       </tr> 
       <tr> 
        <td scope="col">时间表</td> 
        <td scope="col">TSHET</td> 
       </tr> 
       <tr> 
        <td scope="col">用户</td> 
        <td scope="col">用户</td> 
       </tr> 
       <tr> 
        <td scope="col">Workspace</td> 
        <td scope="col">Workspace</td> 
       </tr> 
      </tbody> 
     </table>

* eventType（必需）

   * **字符串** — 表示对象订阅的事件类型的值。 可用的事件类型包括：

      * 创建
      * 删除
      * 更新

* url（必需）

   * **字符串** — 通过HTTP向其发送订阅事件负载的终结点的URL。

* authToken（必需）

   * **字符串** — 用于使用“URL”字段中指定的URL进行身份验证的OAuth2持有者令牌。

## 创建事件订阅API请求

在确保用户具有管理员访问权限并形成订阅资源后，便可以创建事件订阅。

使用以下语法构建URL。

**请求URL**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**请求标头**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>标题名称</p> </th> 
   <th> <p>标头值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Content-type</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID值</p> </td> 
  </tr> 
 </tbody> 
</table>

**请求正文示例：**

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua",
                "authToken": "EauthTokenWorkfrontRocks1234_"
            }
```

**响应正文示例**

```
{
    "id": <NEW SUBSCRIPTION ID>,
    "version": <NEW SUBSCRIPTION VERSION>
}
```

| 响应代码 | 描述 |
|---|---|
| 201（已创建） | 已成功创建事件订阅。 |
| 400（错误请求） | 订阅资源的URL字段被视为无效。 |
| 401（未授权） | 提供的sessionID为空或被视为无效。 |
| 403（禁止访问） | 与提供的sessionID匹配的用户没有管理员访问权限。 |

将订阅资源作为请求正文传递（内容类型为“application/json”）会导致为指定的对象创建事件订阅。 响应代码201 （已创建）表示已创建订阅。 201以外的响应代码表示已创建订阅&#x200B;**NOT**。

>[!NOTE]
>
> “Location”响应标头包含新创建的事件订阅的URI。

**响应标头示例：**

| 响应标头 | 示例 |
|---|---|
| Content-Length | `→0` |
| 日期 | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| 位置 | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| 服务器 | `→Apache-Coyote/1.1` |

## 查询事件订阅

查询Workfront的HTTP时，使用GET方法。 可通过两种方式查询事件订阅：按订阅ID查询（请参阅下文）或查询所有事件订阅。

### 查询所有事件订阅

您可以查询客户的所有事件订阅，或使用以下各项管理响应。 您还可以使用以下选项管理响应：

* **page**：查询参数选项，用于指定要返回的页数。 默认值为1。
* **limit**：查询参数选项，用于指定每页返回的结果数。 默认值为100，最大值为1000。

列出特定客户的所有事件订阅的请求语法如下：

**请求URL**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**请求标头：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>标题名称</p> </th> 
   <th> <p>标头值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID值</p> </td> 
  </tr> 
 </tbody> 
</table>

**响应代码**

| 响应代码 | 描述 |
|---|---|
| 200（确定） | 返回的请求包含为与提供的sessionID匹配的客户找到的所有事件订阅。 |
| 401（未授权） | 提供的sessionID为空。 |
| 403（禁止访问） | 与提供的sessionID匹配的用户没有管理员访问权限。 |


**响应标头示例**

| 响应标头 | 示例 |
|---|---|
| Content-Type | `→application/json;charset=UTF-8` |
| 日期 | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| 服务器 | `→Apache-Coyote/1.1` |
| 传输编码 | `→chunked` |


**响应正文示例**

```
{
    "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
    "date_created": "2024-04-11T17:10:10.305981",
    "date_modified": "2024-04-11T17:10:10.305981",
    "version": "v2",
    "dateVersionUpdated": "2025-01-15T04:04:04.407945"
    "customerId": "504f9640000013401be513579fbebffa",
    "objId": null,
    "objCode": "PROJ",
    "url": "http://requestb.in/ua5hi2ua",
    "eventType": "UPDATE",
    "authToken": "authTokenWorkfrontRocks1234_"
    "subscription_url": {
        "url": "http://requestb.in/ua5hi2ua",
        "date_created": "2024-04-11T15:56:14.169489",
        "successes": 11,
        "failures": 2,
        "disabled_at": null,
        "frozen_at": null
   }
}
```

位置

* **page**&#x200B;和&#x200B;**limit**&#x200B;是请求中提供的值，如果未提供值，则为默认值
* **page_count**&#x200B;是可查询的页面总数。
* **total_count**&#x200B;是与查询匹配的订阅总数。

### 按事件订阅ID查询

您可以按事件订阅ID查询事件订阅。 列出事件订阅的请求语法如下：

**请求URL**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**请求标头**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>标题名称</p> </th> 
   <th> <p>标头值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID值</p> </td> 
  </tr> 
 </tbody> 
</table>

**响应代码**

| 响应代码 | 描述 |
|---|---|
| 200（确定） | 返回的请求具有匹配提供的订阅ID的事件订阅。 |
| 401（未授权） | 提供的sessionID为空。 |
| 403（禁止访问） | 与提供的sessionID匹配的用户没有管理员访问权限。 |


**响应正文示例**



```
{
    "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
    "date_created": "2024-04-11T17:10:10.305981",
    "date_modified": "2024-04-11T17:10:10.305981",
    "version": "v2",
    "dateVersionUpdated": "2025-01-15T04:04:04.407945"
    "customerId": "504f9640000013401be513579fbebffa",
    "objId": null,
    "objCode": "PROJ",
    "url": "http://requestb.in/ua5hi2ua",
    "eventType": "UPDATE",
    "authToken": "authTokenWorkfrontRocks1234_"
    "subscription_url": {
        "url": "http://requestb.in/ua5hi2ua",
        "date_created": "2024-04-11T15:56:14.169489",
        "successes": 11,
        "failures": 2,
        "disabled_at": null,
        "frozen_at": null
   }
}
```


## 事件订阅版本控制

Workfront提供两个版本的活动订阅。

升级或降级事件订阅的功能确保在对事件结构做出更改时，现有订阅不会中断，从而允许您测试和升级到新版本，而不会在事件订阅中出现间隙。

有关事件订阅版本控制的详细信息，包括版本和重要日期之间的具体差异，请参阅[事件订阅版本控制](/help/quicksilver/wf-api/general/event-subs-versioning.md)。

>[!NOTE]
>
>将事件订阅升级或降级到另一个版本时，您在版本更改后的五分钟内，会收到每个事件交付的重复事件。 重复项包括事件订阅版本1和版本2中的一个。 这可确保不会因更改事件订阅版本而错过任何事件。

### 单个订阅版本更改

更改单个订阅的版本的请求语法为：

**请求URL**

```
PUT https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>/version 
```

**示例请求正文**

```
{
    "version": "v2" 
}
```


**示例响应正文(200)**

```
{
    "id": <SUBSCRIPTION ID>,
    "version": "v2" 
}
```

**可能的响应代码**

* 200
* 400
* 404


### 多个订阅版本更改

此端点按订阅列表或所有客户的订阅标记更改多个订阅的版本。

更改单个订阅的版本的请求语法为：

**请求URL**

```
PUT https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/version
```

**请求正文示例**

* 请求订阅列表正文

  ```
  {
      "subscriptionIds": [<SUBSCRIPTION ID 1>, <SUBSCRIPTION ID 2>],
      "version": "v2" 
  }
  ```

* 请求所有客户订阅的正文

  ```
  {
      "allCustomerSubscriptions": true,
      "version": "v2" 
  }
  ```

**示例响应正文(200)**

```
{
    "subscription_ids": [<SUBSCRIPTION ID 1>, <SUBSCRIPTION ID 2>, ...],
    "version": "v2" 
}
```

**可能的响应代码**

* 200
* 400

## 事件订阅筛选

事件订阅筛选可用于确保您仅接收相关消息。 为您的订阅创建过滤器可能会显着减少您的端点需要使用的消息数。

例如，仅当事件有效负载的&#x200B;**newState**&#x200B;将&#x200B;**taskStatus**&#x200B;定义为&#x200B;**current**&#x200B;时，才能将&#x200B;**UPDATE - TASK**&#x200B;事件订阅设置为触发。

>[!IMPORTANT]
>
>以下属性适用于事件订阅筛选

* 当筛选器字段的值为非空时，只会将具有包含筛选器键和值的&#x200B;**newState**&#x200B;的消息发送到订阅的URL
* 您可以按对象的&#x200B;**newState**&#x200B;和/或&#x200B;**oldState**&#x200B;中包含的自定义数据进行筛选
* 仅根据过滤器是否等于特定值来评估过滤器
* 如果您的筛选器语法不正确或与有效负载的&#x200B;**newState**&#x200B;中包含的任何数据都不匹配，则不会返回验证消息以指示发生了错误
* 无法在当前存在的订阅上更新筛选器；必须使用新的筛选器参数创建新订阅。
* 多个筛选器可应用于单个订阅，并且仅在满足所有筛选器条件时才交付订阅。
* 将多个筛选器应用于单个订阅相当于使用&#x200B;**AND**&#x200B;逻辑运算符。
* 只要每个事件订阅之间有一个或多个事件订阅字段参数不同，就可以将多个事件订阅应用于单个对象。
* 将多个事件订阅分配给单个对象时，与该对象关联的所有事件订阅都可以返回到单个端点。 此实践可用作逻辑运算符&#x200B;**OR**&#x200B;的等效替代项，无法使用筛选器参数设置该运算符。
* 以下字段不可过滤：

   * DOCU.groups
   * RECORD.data
   * RECORD_TYPE.data
   * RECORD_TYPE字段

### 使用比较运算符

您可以指定比较字段以及过滤器字段。 在此至字段中使用比较运算符以筛选比较结果。 例如，您可以创建一个UPDATE - TASK订阅，该订阅仅在任务状态不等于current时发送有效负载。 您可以使用以下比较运算符：

#### eq： equal

如果发生的更改与筛选器中的`fieldValue`完全匹配，则此筛选器允许传递消息。 `fieldValue`值区分大小写。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "eq"
        }
    ]
}
```

#### ne：不等于

如果发生的更改与筛选器中的`fieldValue`不完全匹配，则此筛选器允许传递消息。 `fieldValue`值区分大小写。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "ne"
        }
    ]
}
```

#### gt：大于

如果指定`fieldName`上的更新大于`fieldValue`的值，此筛选器允许邮件通过。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gt"
        }
    ]
}
```

#### gte：大于或等于

如果指定`fieldName`上的更新大于或等于`fieldValue`的值，则此筛选器允许消息通过。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gte"
        }
    ]
}
```

#### lt：小于

如果指定`fieldName`上的更新小于`fieldValue`的值，此筛选器允许邮件通过。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lt"
        }
    ]
}
```

#### lte：小于或等于

如果指定`fieldName`上的更新小于或等于`fieldValue`的值，则此筛选器允许消息通过。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lte"
        }
    ]
}
```

#### 包含

如果发生的更改在筛选器中包含`fieldValue`，则此筛选条件允许传递消息。 `fieldValue`值区分大小写

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        }
    ]
}
```

#### containsOnly

此过滤器允许消息仅在完整的选定值集与过滤器中的fieldValue完全匹配时传递，而不管顺序如何。 不能有额外的值或缺少的值。

>[!NOTE]
>
>这用于数组类型（多选）字段。 以下示例订阅仅当`groups`字段完全包含“Choice 3”和“Choice 4”时，才允许传递消息，并且没有其他值或缺少值，与顺序无关。 如果在`fieldValue`中指定了字符串或整数而不是数组，则仅当`groups`字段只包含一个选项并且该选项与`fieldValue`中指定的字符串或整数完全匹配时，订阅才允许消息通过。


```
{
    "objCode": "PROJ",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedProjects",
    "filters": [
        {
            "fieldName": "groups",
            "fieldValue": [
                "Choice 3",
                "Choice 4"
            ],
            "state": "newState",
            "comparison": "containsOnly"
        }
    ]
}
```

#### notContains

仅当指定的字段(`fieldName`)不包含指定的值(`fieldValue`)时，此过滤器才允许传递消息。

>[!NOTE]
>
>这用于数组类型（多选）或字符串字段。 如果字段为字符串，我们将检查指定的值是否未包含在字符串中（例如，“New”不在字符串“Project - Updated”中）。 如果字段是数组并且指定的字段值是字符串或整数，我们将检查数组是否不包含指定的值（例如，“Choice 1”不在[“Choice 2”、“Choice 3”]中）。 以下示例订阅仅在`groups`字段不包含字符串“Group 2”时才允许传递消息。

```
{
    "objCode": "PROJ",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedProjects",
    "filters": [
        {
            "fieldName": "groups",
            "fieldValue": "Group 2",
            "state": "newState",
            "comparison": "notContains"
        }
    ]
}
```

#### 更改

仅当指定的字段(`fieldName`)在oldstate和newstate中具有不同的值时，此过滤器才允许消息通过。 更新指定字段(`fieldName`)以外的其他字段将不会返回该更改。

>[!NOTE]
>
>下面的筛选器数组中的未生效`fieldValue`。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "",
            "comparison": "changed"
        }
    ]
}
```

#### state

此连接器使过滤器应用于已创建或更新的对象的新状态或旧状态。 当您想知道在何处对某个对象进行了更改时，此功能非常有用。
无法在CREATE `oldState`上执行`eventTypes`。

>[!NOTE]
>
>下面带有给定过滤器的订阅将只返回任务名称在`again`上包含`oldState`的消息，该名称与更新任务之前所包含的内容相同。
>&#x200B;>此功能的用例是查找从一个对象更改到另一个对象的对象代码消息。 例如，查找从“Research Some name”更改为“Research TeamName Some name”的所有任务

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains",
            "state": "oldState"
        }
    ]
}
```

### 使用嵌套筛选器

事件订阅支持使用嵌套字段名称对事件的嵌套字段进行筛选。 例如，要筛选其中`newState.data.customField1 = 'myCustomeFieldValue'`的消息，可以创建以下带筛选器的订阅：

```
{
    "objCode": "RECORD",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedRecords",
    "filters": [
        {
            "fieldName": "data",
            "fieldValue": {
                    "customField1": "myCustomFieldValue"
            },
            "comparison": "eq",
            "state": "newState"
        }
    ]
}
```

也可以处理双重嵌套的过滤器。

```
"filters": [
    {
        "fieldName": "data",
        "fieldValue": {
            "fields": {
                "children": {
                    "customerId":"customer1234",
                    "name":"New Campaign"
                }
            }
        },
        "comparison": "eq",
        "state": "newState"
    }
],
"filterConnector": 'AND'
```

### 使用连接器字段

订阅有效负载上的`filterConnector`字段允许您选择应如何应用过滤器。 默认值为“AND”，其中过滤器必须全部为`true`才能使订阅消息通过。 如果指定了“OR”，则只有一个过滤器必须匹配订阅消息才能通过。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        },
        {
            "fieldName": "name",
            "fieldValue": "also",
            "comparison": "contains"
        }
    ],
    "filterConnector": "AND"
}
```

## 删除事件订阅

删除Workfront的HTTP时，请使用DELETE方法。 按订阅ID删除单个事件订阅的请求语法如下所示：

**请求URL：**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**请求标头：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>标题名称</p> </th> 
   <th> <p>标头值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> sessionID值 </p> </td> 
  </tr> 
 </tbody> 
</table>

**响应代码：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>响应代码</p> </th> 
   <th> 描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200（无内容）</td> 
   <td>服务器已成功删除与提供的subscriptionID匹配的事件订阅。</td> 
  </tr> 
  <tr> 
   <td>401（未授权）</td> 
   <td>提供的sessionID为空。</td> 
  </tr> 
  <tr> 
   <td>403（禁止访问）</td> 
   <td>与提供的sessionID匹配的用户没有管理员访问权限。</td> 
  </tr> 
  <tr> 
   <td>404（未找到）</td> 
   <td>服务器找不到与为删除提供的订阅ID匹配的事件订阅。</td> 
  </tr> 
 </tbody> 
</table>

**响应标头示例：**

| 响应标头 | 示例 |
|---|---|
| 日期 | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| 服务器 | `→Apache-Coyote/1.1` |


**响应正文示例：** N/A

## 事件有效负载示例

用户收到的有效负载会因对象类型而异，但存在一个一致的格式，用于交付这些变化的有效负载。

例如，以下属性在所有事件负载中保持一致：

* 事件类型
* subscriptionId
* oldState
* newState
* eventTime

尽管格式一致，但属性中包含的值在不同的对象和对象类型之间有所不同。

下面显示了UPDATE事件和CREATE事件的负载示例。 请注意，在UPDATE示例中，oldState对象和newState对象是相同的，而在CREATE示例中，oldState对象是空的（不是NULL）。

以下是UPDATE事件的有效负载示例：

<!-- [Copy](javascript:void(0);) -->

```
{
                  "eventType": "UPDATE",
                   "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                   "eventTime": {
                       "nano": 998000000,
                       "epochSecond": 1507319336
                   },
                   "eventVersion": "v2",
                   "subscriptionVersion": "v2",
                   "newState": {
                "ID": "59d7ddf7000002322d791eb08bafddfb", 
                       "name": "EventSub Test updated",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:56.980-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,       "categoryID": null,
                      "status": "CUR",
                      "parameterValues": {}
                   },
                   "oldState": {
                       "ID": "59d7ddf7000002322d791eb08bafddfb",
                       "name": "EventSub Test 180fd595-63fb-4fa9-bd47-58bf6e53d964",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:07.792-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,<
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,
                       "categoryID": null,
                       "status": "CUR",
                       "parameterValues": {}
                   }
                }
```

以下是CREATE事件的有效负载示例：

<!-- [Copy](javascript:void(0);) -->

```
{
                "eventType": "CREATE",
                "subscriptionId": "4028e3815ebf03a7015ebfa53b6d0002",
                "eventTime": {
                "nano": 232000000,
                "epochSecond": 1506453831
                },
                "eventVersion": "v2",
                "subscriptionVersion": "v2",
                "newState": {
                "ID": "59caa946000000e07b0afc3383230c67",
                "name": "EventSub Test fe16d470-0a40-4290-92f4-6a0389fb536c",
                "objCode": "PROJ",
                "entryDate": "2017-09-26T13:23:50.746-0600",
                "accessorIDs": ["544820df0000142362741fc0c368de19"],
                "lastUpdateDate": "2017-09-26T13:23:50.927-0600",
                "groupID": "544820df0000140f6a9c1faa7cacadd3",
                "sponsorID": null,
                "description": null,
                "plannedCompletionDate": "2017-09-26T09:00:00.000-0600",
                "enteredByID": "544820df0000142362741fc0c368de19",
                "ownerID": "544820df0000142362741fc0c368de19",
                "templateID": null,
                "priority": 0,
                "companyID": null,
                "portfolioID": null,
                "referenceNumber": 1750,
                "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                "customerID": "544820df0000135b7719dcca654391f6",
                "currency": null,
                "categoryID": null,
                "status": "CUR",
                "parameterValues": {}
                },
                "oldState": {}
            }
```

## Base 64编码

如果事件订阅因事件订阅中包含的特殊字符与网络设置之间冲突而被拒绝，则可以使用Base64编码传递事件订阅。 Base64是一组编码方案，可以将任意数据转换为ASCII字符串格式。 需要注意的是，Base64不是一种安全加密形式。

### Base 64编码字段

base64Encoding字段是一个可选字段，用于启用事件订阅负载的Base64编码。 默认值为false，可能的值为： true、false和“ ”（空白）。

### 使用base64Encoding字段的请求示例

如果使用设置为true的base64Encoding字段发出请求，则有效负载中的&#x200B;**newState**&#x200B;和&#x200B;**oldState**&#x200B;对象将作为base 64编码字符串交付。 如果base64Encoding字段设置为false、保留为空或未包含在请求中，则返回的有效负载将不会在base 64中进行编码。

以下是使用base64Encoding字段的请求示例：

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua"",
                "authToken": "EauthTokenWorkfrontRocks1234_",
                "base64Encoding": "true"
            }
```

### base 64编码中的响应有效负载示例

<!-- [Copy](javascript:void(0);) -->

```
                {
                "eventType": "UPDATE",
                "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                "eventTime": {
                "nano": 998000000,
                "epochSecond": 1507319336
                },
                "eventVersion": "v2",
                "subscriptionVersion": "v2",
                "newState": "ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ==",
                "oldState": "ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="
                }
 
```

## 用于查询所有事件订阅的已弃用方法

以下API端点已弃用，不应用于新实施。 我们还建议将旧实施转换为上述&#x200B;**查询事件订阅**&#x200B;部分中的方法。

您可以查询由sessionID值指定的客户的所有事件订阅。 列出特定客户的所有事件订阅的请求语法如下URL：

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list
```

**请求标头：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>标题名称</p> </th> 
   <th> <p>标头值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> sessionID值 </p> </td> 
  </tr> 
 </tbody> 
</table>

**响应代码：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>响应代码</p> </th> 
   <th> 描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200（无内容）</td> 
   <td>该请求已成功返回为用户找到的所有事件订阅。</td> 
  </tr> 
  <tr> 
   <td>401（未授权）</td> 
   <td>提供的sessionID为空。</td> 
  </tr> 
  <tr> 
   <td>403（禁止访问）</td> 
   <td>与提供的sessionID匹配的用户没有管理员访问权限。</td> 
  </tr> 
 </tbody> 
</table>



### 响应正文示例

<!-- [Copy](javascript:void(0);) -->

```
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customer_id": "504f9640000013401be513579fbebffa",
                "obj_id": "ObjId1234",
                "obj_code": "TASK",
                "url": "http://test.test.net/test/1234",
                "event_type": "UPDATE",
                "auth_token": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customer_d": "504f9640000013401be513579fbebffa",
                "obj_id": null,
                "obj_code": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "event_type": "UPDATE",
                "auth_token": "authTokenWorkfrontRocks1234_"
                }                
                ]
```
