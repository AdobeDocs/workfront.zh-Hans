---
content-type: api
navigation-topic: general-api
title: 事件订阅API
description: 事件订阅API
author: John
feature: Workfront API
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: c52f1839d3d00c71c6d567084dafd586d161d8fb
workflow-type: tm+mt
source-wordcount: '2203'
ht-degree: 3%

---


# 事件订阅API

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

对事件订阅支持的Adobe Workfront对象执行操作时，您可以将Workfront配置为向所需的端点发送响应。 这意味着第三方应用程序在发生Workfront交互后不久便可以通过Workfront API接收来自交互的更新。 通常，您可能会在记录的数据更改后的不到5秒内收到Webhook通知。 客户平均在记录的数据更改后不到1秒钟就会收到Webhook通知。  

要通过防火墙接收事件订阅负载，您必须将以下IP地址添加到您的允许列表:

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

以下主题支持事件订阅API:

## 事件订阅支持的对象

事件订阅支持以下Workfront对象。

* 分配
* 公司
* 仪表板
* 文档
* 费用
* 小时
* 问题
* 注释
* 项目组合
* 项目群
* 项目
* 报告
* 任务
* 模板
* 时间表
* 用户

有关事件订阅对象支持的字段列表，请参阅 [事件订阅资源字段](../../wf-api/api/event-sub-resource-fields.md).

## 事件订阅身份验证

要创建、查询或删除事件订阅，您的Workfront用户需要满足以下条件：

* “系统管理员”的访问级别
* apiKey

   >[!NOTE]
   >
   >如果您的用户已在使用Workfront的API，则您的用户应该已经拥有apiKey。 您可以通过以下HTTP请求检索apiKey:

**请求URL:**

```
PUT https://<HOSTNAME>/attask/api/v7.0/USER?action=getApiKey&username=<USERNAME>&password=<PASSWORD>
```

**请求标头：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>标题名称</p> </th> 
   <th> <p>标题值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>内容类型</p> </td> 
   <td> <p>text/html</p> </td> 
  </tr> 
 </tbody> 
</table>

**响应代码：**

| 响应代码 | 描述 |
|---|---|
| 200(OK) | 已成功处理请求，应在响应正文中返回用户的现有apiKey。 |
| 401（未授权） | 服务器确认请求，但无法处理该请求，因为请求的apiKey/用户无权发出此请求。 |

{style=&quot;table-layout:auto&quot;}

**响应正文示例：**

```
{
               "data"{
               "result": "rekxqndrw9783j4v79yhdsakl56bu1jn"
               }
      }
```

>[!NOTE]
>
> 如果您是首次使用Workfront API，则需要生成一个apiKey，您可以通过以下链接执行此操作：


```
PUT https://<HOSTNAME>/attask/api/v7.0/USER/generateApiKey?username=<USERNAME>&password=<PASSWORD>
```

## 形成订阅资源

订阅资源包含以下字段。

* objId（可选）

   * **字符串**  — 为其触发事件的指定objCode对象的ID。 如果未指定此字段，则用户将接收指定类型的所有对象的事件。

* objCode（必需）

   * **字符串**  — 订阅更改的对象的objCode。 下表列出了objCode的可能值。

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <thead> 
       <tr> 
        <th><p>对象</p></th> 
        <th><p>objCode</p></th> 
       </tr> 
      </thead> 
      <tbody> 
       <tr> 
        <td scope="col">分配</td> 
        <td scope="col"><p>ASSGN</p></td> 
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
        <td scope="col">多库 </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>费用</p></td> 
        <td scope="col">EXPNS</td> 
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
        <td scope="col"><p>PROJ</p></td> 
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
        <td scope="col"><p>TMPL</p></td> 
       </tr> 
       <tr> 
        <td scope="col">时间表</td> 
        <td scope="col">TSHET</td> 
       </tr> 
       <tr> 
        <td scope="col">用户</td> 
        <td scope="col">用户</td> 
       </tr> 
      </tbody> 
     </table>

* eventType（必需）

   * **字符串**  — 一个值，表示对象订阅的事件类型。 可用的事件类型包括：

      * 创建
      * 删除 
      * 更新

* url（必需）

   * **字符串**  — 通过HTTP将订阅事件有效负载发送到的端点的URL。

* authToken（必需）

   * **字符串** - OAuth2载体令牌，用于使用“URL”字段中指定的URL进行身份验证。 

## 创建事件订阅API请求

在确保用户具有管理员访问权限并形成订阅资源后，您便可以创建事件订阅。

使用以下语法来构建URL。

**请求URL:**


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
   <th> <p>标题值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>内容类型</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
  <tr> 
   <td> <p>授权</p> </td> 
   <td> <p>apiKey值</p> </td> 
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
| 400（请求错误） | 订阅资源的URL字段被视为无效。 |
| 401（未授权） | 提供的apiKey为空或视为无效。 |
| 403（禁止） | 与提供的apiKey匹配的用户没有管理员访问权限。 |

将订阅资源作为请求正文传递（其内容类型为“application/json”）会导致为指定的对象创建事件订阅。 响应代码为201（已创建）表示已创建订阅。 201以外的响应代码表示订阅是 **NOT** 创建。

>[!NOTE]
 “位置”响应标头包含新创建事件订阅的URI。

**响应标头示例：**

| 响应标头 | 示例 |
|---|---|
| Content-Length | `→0` |
| 日期 | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| 位置 | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| 服务器 | `→Apache-Coyote/1.1` |

## 查询事件订阅

查询Workfront HTTP时，请使用GET方法。 有两种方法可查询事件订阅：按订阅ID查询（请参阅下文）或查询所有事件订阅。

### 查询所有事件订阅

您可以按照apiKey值的指定查询客户的所有事件订阅。 您还可以使用以下选项管理响应：

* **页面**:用于指定要返回的页数的查询参数选项。 默认值为1。
* **限制**:查询参数选项，以指定每页返回的结果数。 默认值为100，最大值为1000。

列出特定客户所有事件订阅的请求语法如下：

**请求URL:**

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
   <th> <p>标题值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>授权</p> </td> 
   <td> <p>apiKey值</p> </td> 
  </tr> 
 </tbody> 
</table>

**响应代码：**

| 响应代码 | 描述 |
|---|---|
| 200(OK) | 返回的请求，其中包含为与提供的apiKey匹配的客户找到的所有事件订阅。 |
| 401（未授权） | 提供的apiKey为空。 |
| 403（禁止） | 与提供的apiKey匹配的用户没有管理员访问权限。 |


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

* **页面** 和 **限制** 是请求中提供的值，还是未提供值的默认值
* **page_count** 是可查询的页面总数。
* **total_count** 是与查询匹配的订阅总数。

### 按事件订阅ID进行查询

您可以按事件订阅的ID查询事件订阅。 列出事件订阅的请求语法如下：

**请求URL:**

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
   <th> <p>标题值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>授权</p> </td> 
   <td> <p>apiKey值</p> </td> 
  </tr> 
 </tbody> 
</table>

**响应代码：**

| 响应代码 | 描述 |
|---|---|
| 200(OK) | 返回的请求包含与提供的订阅ID匹配的事件订阅。 |
| 401（未授权） | 提供的apiKey为空。 |
| 403（禁止） | 与提供的apiKey匹配的用户没有管理员访问权限。 |


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

## 事件订阅过滤

事件订阅过滤功能可用于确保您仅接收相关消息。 为订阅创建过滤器可能会显着减少端点需要使用的消息数量。

例如， **更新 — 任务** 事件订阅只能在 **newState** 事件有效负载的 **taskStatus** as **当前**.

>[!IMPORTANT]
以下属性适用于事件订阅过滤

* 当过滤器字段具有非空值时， **newState** 包含过滤器键和值会发送到订阅的URL
* 您可以按 **newState** 和/或 **oldState**&#x200B;对象
* 过滤器仅根据它们是否等于特定值来评估
* 如果过滤器语法不正确或与 **newState** 在有效负载中，将不会返回验证消息，以指示发生错误
* 当前存在的订阅无法更新过滤器；必须使用新筛选器参数创建新订阅。
* 多个过滤器可应用于单个订阅，并且仅在满足所有过滤条件时才会提供订阅。
* 将多个过滤器应用于单个订阅的做法与使用 **和** 逻辑运算符。
* 只要一个或多个事件订阅字段参数在每个事件订阅之间不同，就可以将多个事件订阅应用于单个对象。
* 当将多个事件订阅分配给单个对象时，与该对象关联的所有事件订阅都可以返回到单个端点。 此实践可用作逻辑运算符的等效替代方法 **或** 无法使用过滤器参数设置。

### 使用比较运算符

您可以指定比较字段和过滤器字段。 在此对字段中使用比较运算符可筛选比较结果。 例如，您可以创建UPDATE - TASK订阅，该订阅仅在任务状态不等于当前时发送有效负荷。 您可以使用以下比较运算符：

#### eq:等于

此过滤器允许在发生的更改与 `fieldValue` 完全在过滤器中。 的 `fieldValue` 值区分大小写。

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

#### ne:不等于

此过滤器允许在发生的更改与匹配时发送消息 `fieldValue` 完全在过滤器中。 的 `fieldValue` 值区分大小写。

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

#### gt:大于

此过滤器允许在指定的 `fieldName` 大于的值 `fieldValue`.

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

#### get:大于或等于

此过滤器允许在指定的 `fieldName` 大于或等于的值 `fieldValue`.

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

#### lt:小于

此过滤器允许在指定的 `fieldName` 小于的值 `fieldValue`.

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

#### lte:小于或等于

此过滤器允许在指定的 `fieldName` 小于或等于 `fieldValue`.

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

如果发生的更改包含 `fieldValue` 中。 的 `fieldValue` 值区分大小写

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

此过滤器仅允许在指定的字段(`fieldName`)在oldstate和newstate中具有不同的值。 正在更新除指定字段以外的其他字段(`fieldName`)将不会返回该更改。

>[!NOTE]
`fieldValue` 在下面的筛选器数组中不起作用。

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

此连接器将过滤器应用于已创建或更新对象的新状态或旧状态。 当您想要了解在何处进行了从某个内容到另一个内容的更改时，此功能非常有用。
`oldState` 在CREATE上不可能 `eventTypes`.

>[!NOTE]
下面的订阅和给定的过滤器将仅返回任务名称包含的消息 `again` 在 `oldState`，在对任务进行更新之前的状态。
这种方法的一个用例是查找objCode消息，这些消息从一个内容更改为另一个内容。 例如，要了解从“Research Some Name”（研究团队名称）更改为“Research TeamName Some name”（研究团队名称某些名称）的所有任务

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

的 `filterConnector` 字段，可选择应用过滤器的方式。 默认值为“AND”，其中过滤器必须全部为 `true` 以使订阅消息通过。 如果指定了“OR”，则只有一个过滤器必须匹配才能通过订阅消息。

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

删除Workfront HTTP时，请使用DELETE方法。 按订阅ID删除单个事件订阅的请求语法如下：

**请求URL:**

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
   <th> <p>标题值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>授权</p> </td> 
   <td> <p> 用户的apiKey </p> </td> 
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
   <td>服务器成功删除了与提供的subscriptionID匹配的事件订阅。</td> 
  </tr> 
  <tr> 
   <td>401（未授权）</td> 
   <td>提供的apiKey为空。</td> 
  </tr> 
  <tr> 
   <td>403（禁止）</td> 
   <td>与提供的apiKey匹配的用户没有管理员访问权限。</td> 
  </tr> 
  <tr> 
   <td>404（未找到）</td> 
   <td>服务器找不到与为删除提供的subscriptionID匹配的事件订阅。</td> 
  </tr> 
 </tbody> 
</table>

**响应标头示例：**

| 响应标头 | 示例 |
|---|---|
| 日期 | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| 服务器 | `→Apache-Coyote/1.1` |


**响应正文示例：** 不适用

## 事件负载示例

用户收到的负载因对象类型而异，但传递这些不同负载的格式是一致的。

例如，以下属性在所有事件负载中保持一致：

* eventType
* subscriptionId
* oldState
* newState
* eventTime

尽管格式一致，但属性中包含的值在不同对象和对象类型之间有所不同。

下面显示了UPDATE事件和CREATE事件的有效负载示例。 请注意，在UPDATE示例中，oldState对象和newState对象是相同的，而在CREATE示例中，oldState对象为空（非NULL）。

以下是UPDATE事件的有效负荷示例：

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

以下是CREATE事件的有效负荷示例：

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

## 基本64编码

如果由于事件订阅中包含的特殊字符与网络设置发生冲突而拒绝事件订阅，则可以使用Base64编码传递事件订阅。 Base64是一组编码方案，可将任意数据转换为ASCII字符串格式。 请务必注意，Base64不是一种安全加密形式。

### 基64编码字段

base64Encoding字段是用于启用事件订阅负载的Base64编码的可选字段。 默认值为false，可能的值为：true、false和“ ”（空白）。

### 使用base64Encoding字段的请求示例

如果使用将base64Encoding字段设置为true发出请求，则 **newState** 和 **oldState** 有效负载中的对象将作为基本64编码字符串进行传递。 如果base64Encoding字段设置为false、留空或未包含在请求中，则返回的有效负载将不会在base 64中进行编码。

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

### 基于64编码的响应负载示例

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

以下API端点已弃用，不应用于新实施。 我们还建议将旧实施转换到 **查询事件订阅** 部分。

您可以按照apiKey值的指定查询客户的所有事件订阅。 列出特定客户所有事件订阅的请求语法如下所示：

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
   <th> <p>标题值</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>授权</p> </td> 
   <td> <p> 用户的apiKey </p> </td> 
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
   <td>请求成功返回了为用户找到的所有事件订阅。</td> 
  </tr> 
  <tr> 
   <td>401（未授权）</td> 
   <td>提供的apiKey为空。</td> 
  </tr> 
  <tr> 
   <td>403（禁止）</td> 
   <td>与提供的apiKey匹配的用户没有管理员访问权限。</td> 
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
