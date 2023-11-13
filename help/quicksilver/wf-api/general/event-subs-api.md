---
content-type: api
navigation-topic: general-api
title: 事件订阅API
description: 事件订阅API
author: Becky
feature: Workfront API
role: Developer
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: c08bd3311892d24a9bd40af138169957f5ea2ca4
workflow-type: tm+mt
source-wordcount: '2126'
ht-degree: 4%

---


# 事件订阅API

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

当事件订阅支持的Adobe Workfront对象上发生操作时，您可以将Workfront配置为将响应发送到所需的端点。 这意味着第三方应用程序在更新发生后不久即可通过Workfront API接收来自Workfront交互的更新。 通常，您可以预期在记录数据更改后的5秒内收到webhook通知。 平均而言，客户会在距记录的数据更改不到1秒的时间内收到webhook通知。  

列入允许列表要通过防火墙接收事件订阅负载，必须将以下IP地址添加到您的：

**对于欧洲客户：**

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

* 任务
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

有关事件订阅对象支持的字段列表，请参阅 [事件订阅资源字段](../../wf-api/api/event-sub-resource-fields.md).

## 事件订阅身份验证

要创建、查询或删除事件订阅，您的Workfront用户需要满足以下条件：

* 要使用事件订阅，需要具有“系统管理员”访问级别。
* A `sessionID`  标头需要使用事件订阅API

  有关更多信息，请参阅 [身份验证](api-basics.md#authentication) 在 [API基础知识](api-basics.md).

## 形成订阅资源

订阅资源包含以下字段。

* objId（可选）

   * **字符串**  — 为其触发事件的指定对象代码的对象ID。 如果未指定此字段，则用户会收到指定类型的所有对象的事件。

* 对象代码（必需）

   * **字符串**  — 订阅更改的对象的对象代码。 下表中列出了objCode的可能值。

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
        <td scope="col">任务</td> 
        <td scope="col"><p>分配</p></td> 
       </tr> 
       <tr> 
        <td scope="col">公司 </td> 
        <td scope="col"><p>CMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">仪表板</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>文档</p></td> 
        <td scope="col">DOCU </td> 
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
        <td scope="col">工作区</td> 
       </tr> 
      </tbody> 
     </table>

* eventType（必需）

   * **字符串**  — 一个值，表示对象订阅的事件类型。 可用的事件类型包括：

      * 创建
      * 删除 
      * 更新

* url（必需）

   * **字符串**  — 通过HTTP向其发送订阅事件负载的端点的URL。

* authToken（必需）

   * **字符串** - OAuth2持有者令牌，用于使用“URL”字段中指定的URL进行身份验证。 

## 创建事件订阅API请求

在确保用户具有管理员访问权限并形成订阅资源后，便可以创建事件订阅。

使用以下语法构建URL。

**请求URL：**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
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

| 响应代码 | 描述 |
|---|---|
| 201（已创建） | 已成功创建事件订阅。 |
| 400（错误请求） | 订阅资源的URL字段被视为无效。 |
| 401（未授权） | 提供的sessionID为空或被视为无效。 |
| 403（禁止访问） | 与提供的sessionID匹配的用户没有管理员访问权限。 |

将订阅资源作为请求正文传递（内容类型为“application/json”）会导致为指定的对象创建事件订阅。 响应代码201 （已创建）表示已创建订阅。 201以外的响应代码表示订阅 **NOT** 已创建。

>[!NOTE]
>
> “Location”响应标头包含新创建的事件订阅的URI。

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

* **页面**：查询参数选项，用于指定要返回的页数。 默认值为1。
* **limit**：查询参数选项，用于指定每页返回的结果数。 默认值为100，最大值为1000。

列出特定客户的所有事件订阅的请求语法如下：

**请求URL：**

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

**响应代码：**

| 响应代码 | 描述 |
|---|---|
| 200（确定） | 返回的请求包含为与提供的sessionID匹配的客户找到的所有事件订阅。 |
| 401（未授权） | 提供的sessionID为空。 |
| 403（禁止访问） | 与提供的sessionID匹配的用户没有管理员访问权限。 |


**响应标头示例：**

| 响应标头 | 示例 |
|---|---|
| Content-Type | `→application/json;charset=UTF-8` |
| 日期 | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| 服务器 | `→Apache-Coyote/1.1` |
| 传输编码 | `→chunked` |


**响应正文示例：**

<!-- [Copy](javascript:void(0);) -->

```
                {
                "subscriptions":                
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": "ObjId1234",
                "objCode": "TASK",
                "url": "http://test.test.net/test/1234",
                "eventType": "UPDATE",
                "authToken": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
                ],
                "meta":
                {
                "page": 1,
                "page_count": 2,
                "limit": 100,
                "total_count": 150
                }
                }            
```

位置

* **页面** 和 **limit** 是请求中提供的值，如果未提供值，则使用默认值
* **page_count** 是可查询的页面总数。
* **total_count** 是符合查询的订阅总数。

### 按事件订阅ID查询

您可以按事件订阅ID查询事件订阅。 列出事件订阅的请求语法如下：

**请求URL：**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
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

**响应代码：**

| 响应代码 | 描述 |
|---|---|
| 200（确定） | 返回的请求具有匹配提供的订阅ID的事件订阅。 |
| 401（未授权） | 提供的sessionID为空。 |
| 403（禁止访问） | 与提供的sessionID匹配的用户没有管理员访问权限。 |


**响应正文示例：**

<!-- [Copy](javascript:void(0);) -->

```
{
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
```

## 事件订阅筛选

事件订阅筛选可用于确保您仅接收相关消息。 为您的订阅创建过滤器可能会显着减少您的端点需要使用的消息数。

例如， **更新 — 任务** 事件订阅只能设置为在 **newState** 的事件有效负载定义 **任务状态** 作为 **当前**.

>[!IMPORTANT]
>
以下属性适用于事件订阅筛选

* 当过滤器字段的值为非空时，仅限包含 **newState** 包含过滤器键和值，以发送到订阅的URL
* 您可以按中包含的自定义数据进行筛选 **newState** 和/或 **oldState**&#x200B;对象的
* 仅根据过滤器是否等于特定值来评估过滤器
* 如果您的筛选器语法不正确或与 **newState** 对于有效负载，将不会返回验证消息以指示发生了错误
* 无法在当前存在的订阅上更新筛选器；必须使用新的筛选器参数创建新订阅。
* 多个筛选器可应用于单个订阅，并且仅在满足所有筛选器条件时才交付订阅。
* 将多个过滤器应用于单个订阅是一种做法，相当于使用 **和** 逻辑运算符。
* 只要每个事件订阅之间有一个或多个事件订阅字段参数不同，就可以将多个事件订阅应用于单个对象。
* 将多个事件订阅分配给单个对象时，与该对象关联的所有事件订阅都可以返回到单个端点。 此做法可用作逻辑运算符的等效替代项 **或者** 无法使用筛选器参数进行设置的。

### 使用比较运算符

您可以指定比较字段以及过滤器字段。 在此至字段中使用比较运算符以筛选比较结果。 例如，您可以创建一个UPDATE - TASK订阅，该订阅仅在任务状态不等于current时发送有效负载。 您可以使用以下比较运算符：

#### eq： equal

此过滤器允许在发生的更改匹配时传递消息 `fieldValue` 在筛选器中。 此 `fieldValue` 值区分大小写。

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

此过滤器允许在发生的更改不匹配时发送消息 `fieldValue` 在筛选器中。 此 `fieldValue` 值区分大小写。

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

此过滤器允许在指定日期更新消息时传递消息 `fieldName` 大于的值 `fieldValue`.

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

此过滤器允许在指定日期更新消息时传递消息 `fieldName` 大于或等于 `fieldValue`.

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

此过滤器允许在指定日期更新消息时传递消息 `fieldName` 小于的值 `fieldValue`.

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

此过滤器允许在指定日期更新消息时传递消息 `fieldName` 小于或等于 `fieldValue`.

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

如果发生的更改包含 `fieldValue` 在过滤器中。 此 `fieldValue` 值区分大小写

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

#### 更改

此过滤器仅允许在指定字段(`fieldName`)在oldstate和newstate中具有不同的值。 正在更新指定字段以外的其他字段(`fieldName`)将不会返回该更改。

>[!NOTE]
>
`fieldValue` 在“滤镜”数组中，以下选项无效。

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
`oldState` 创建时不可能 `eventTypes`.

>[!NOTE]
>
下面带有给定过滤器的订阅将仅返回任务名称包含 `again` 在 `oldState`，对任务进行更新之前的状态。
此功能的用例是查找从一个对象更改到另一个对象的对象代码消息。 例如，查找从“Research Some name”更改为“Research TeamName Some name”的所有任务

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

### 使用连接器字段

此 `filterConnector` 利用订阅有效负载上的字段，可选择应如何应用过滤器。 默认值为“AND”，其中所有过滤器都必须是 `true` 订阅消息才能通过。 如果指定了“OR”，则只有一个过滤器必须匹配订阅消息才能通过。

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
   <th> 描述</th> 
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


**响应正文示例：** 不适用

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

如果使用设置为true的base64Encoding字段发出请求，则 **newState** 和 **oldState** 有效负载中的对象将作为base 64编码字符串交付。 如果base64Encoding字段设置为false、保留为空或未包含在请求中，则返回的有效负载将不会在base 64中进行编码。

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
                "newState": "ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ==",
                "oldState": "ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="
                }
 
```

## 用于查询所有事件订阅的已弃用方法

以下API端点已弃用，不应用于新实施。 我们还建议将旧实施转换为 **查询事件订阅** 章节。

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
   <th> 描述</th> 
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
