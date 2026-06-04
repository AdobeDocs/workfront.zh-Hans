---
title: Adobe Workfront规划API基础知识
description: Adobe Workfront Planning API的目标是通过引入通过HTTP运行的REST-ful架构来简化与Planning的构建集成。 本文档假定您熟悉REST和JSON响应，并介绍了Planning API采用的方法。
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
TQID: https://experienceleague.adobe.com/SGwYFV5aZJGwfUy7ejVTaOkn0v4Dt-HJLI5hDWKVhMo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 2232
ht-degree: 2%

---

# Adobe Workfront规划API基础知识

{{planning-important-intro}}

<!--

Lilit asked me to hide everything in this current article and replace it with her version of it. I kept just the Field type and search modifier section. The rest of the article is a re-write of the original from Lilit. 

She also said we need to reword how we organize the version features, after we get more versions released but for now, she calls out what's different in V1 than the current (V2) with almost every feature. 

-->

Adobe Workfront Planning API的目标是通过引入通过HTTP运行的RESTful架构来简化与Planning的构建集成。 本文档假设您熟悉REST和JSON响应。

有关完整的端点引用、请求/响应架构和特定于版本的详细信息，请参阅[Workfront Planning API开发人员文档](https://developer.adobe.com/wf-planning)。

## 身份验证

Workfront计划API使用OAuth 2.0进行身份验证。 凭据通过Adobe Developer Console进行设置。

根据您的集成类型，我们支持以下两个流程：

* **服务器到服务器身份验证(JWT)**：用于无用户交互的自动集成和后端服务。 使用OAuth服务器到服务器凭据（客户端凭据授予 — 您的应用程序使用其客户端ID和密码直接进行身份验证以获取访问令牌，而无需用户登录或同意步骤）。

  有关信息，请参阅[服务器到服务器身份验证](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/)。

* **用户身份验证（授权码流）**：用于代表特定用户进行操作的集成。 使用OAuth Web应用程序或单页应用程序凭据（授权代码授予 — 用户登录并同意，之后您的应用程序会收到授权代码，然后它会交换访问令牌）。

  有关信息，请参阅[用户身份验证](https://developer.adobe.com/developer-console/docs/guides/authentication/UserAuthentication/)。

要开始配置，请在Adobe Developer Console中创建一个项目，然后添加Workfront规划API以获取凭据。

要设置凭据，请在Workfront中创建OAuth2应用程序。

有关信息，请参阅[为Workfront集成创建OAuth2应用程序](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)。

>[!NOTE]
>
>Workfront Planning不支持`/login`端点和API密钥身份验证。 请勿使用`sessionID`或`apiKey`参数。


## API版本控制

Planning API通过URL路径进行版本控制。

以下是当前支持的版本：

<!--

(*****************add deprecation date column above, when we have one*****************)

-->

| 版本 | 发行日期 |
|-----------|----------------|
| 版本1 | 2024 年 7 月 |
| 版本2 | 2026年5月 |

>[!NOTE]
>
>适用于Workfront Fusion的Workfront规划连接器尚未更新到API版本2，在进一步通知之前，它将继续使用版本1。

有关当前支持的版本的详细信息，请参阅文章[Workfront Planning API开发人员文档](https://developer.adobe.com/wf-planning)。

我们建议在所有集成中明确定向某个版本：

```
https://{customer-domain}/maestro/api/v2/...
```

发布新的主要版本后，在告知弃用日期之前，以前的版本将继续可用。

按照Workfront发行说明操作，及时了解API更改。


## URL结构和操作

通过将HTTP请求发送到对象的唯一URI来控制对象。 操作由HTTP方法指定。

| 方法 | 操作 |
|----------|----------------------------------------------------------------------|
| GET | 按ID检索单个对象，或搜索/列出对象 |
| POST | 创建新对象 |
| PUT | 替换现有对象（完全更新） |
| PATCH | 部分更新现有对象（仅修改提供的字段） |
| 删除 | 删除对象 |

>[!NOTE]
>
>**版本1中不支持** `PATCH`。 对所有更新使用`PUT`。


有关完整的端点路径和请求/响应示例，请参阅[developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning)上的&#x200B;**API引用**。

## HTTP状态代码

Planning API返回标准HTTP状态代码：

| 代码 | 含义 |
|------------------------|-------------------------------------------------|
| 200 OK | 成功的GET、PUT或PATCH |
| 201已创建 | POST成功（已创建资源） |
| 204无内容 | 成功DELETE |
| 207多状态 | 批量操作已完成，但结果有好有坏，有些项目成功，有些项目失败。 有关详细信息，请查看单个项目响应。 |
| 400错误请求 | 无效请求 — 有关详细信息，请参阅错误响应 |
| 401未授权 | 身份验证令牌缺失或无效 |
| 403禁止访问 | 已验证权限不足 |
| 404未找到 | 资源不存在 |
| 409冲突 | 写入冲突，资源被另一个请求修改。 请使用最新版本重试。 |
| 429请求过多 | 超出速率限制 |

>[!NOTE]
>
>**版本1注意：**&#x200B;版本1为所有成功的操作（包括POST和DELETE）返回`200 OK`。


## 错误处理

Planning API会以一致的格式返回错误。 每个错误响应包括人工可读消息、机器可读错误代码和支持升级请求ID。

示例错误响应：

```
json
{
  "title": "Validation failed",
  "status": 400,
  "detail": "Request validation failed. See 'errors' for details.",
  "errorCode": "VALIDATION_FAILED",
  "requestId": "req-123",
  "errors": [
    { "field": "name", "message": "must not be blank" }
  ]
}
```

使用`errorCode` （不是`status`）来推动程序化错误处理。 它提供了故障的最具体分类。

>[!NOTE]
>
>**版本1注意：**&#x200B;版本1错误响应使用数字`type`字段（例如`40001`）而不是字符串`errorCode`，并将详细信息包装在`report`对象中而不是顶级`detail`字段中。

## 过滤记录

在记录搜索请求中使用`filter`参数可仅返回符合特定条件的记录。 对于POST请求，`filter`是请求正文中的JSON属性。 对于GET请求，`filter`是包含JSON编码的筛选器组的查询参数。 过滤器使用具有显式逻辑运算符的类型复合结构。

```
json
{
  "filter": {
    "operator": "AND",
    "conditions": [
      { "fieldId": "<fieldId>", "condition": "IS", "value": "Active" },
      { "fieldId": "<fieldId>", "condition": "CONTAINS", "value": "marketing" }
    ]
  }
}
```

可以使用`AND` / `OR`运算符嵌套筛选器以生成复合条件：

```
json
{
  "filter": {
    "operator": "OR",
    "conditions": [
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "BETWEEN", "value": ["2024-03-31T20:00:00.000Z", "2024-04-01T20:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "active" }
        ]
      },
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "IS_BETWEEN", "value": ["2024-04-15T00:00:00.000Z", "2024-04-16T00:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "planned" }
        ]
      }
    ]
  }
}
```

>[!NOTE]
>
>**版本1注意：**&#x200B;版本1在`filters`对象中使用Mongo样式无类型运算符。 运算符以`$`为前缀（例如`$and`、`$or`、`$is`、`$contains`、`$isBetween`）。 在请求正文中传递分页参数(`offset`、`limit`)和`recordTypeId`，而不是作为URL路径和查询参数传递。


## 字段类型和搜索修饰符

您可以使用带有字段的修饰符和过滤器来控制在结果中返回哪些数据。

有关示例，请参阅[Workfront Planning API开发人员文档](https://developer.adobe.com/wf-planning/)。

### 使用搜索修饰符

Workfront Planning支持以下搜索修饰符：


<table style="table-layout:auto"> 
  <colgroup><col class="c1"><col class="c2"><col class="c3"><col class="c4"></colgroup>
  <thead>
    <tr>
      <th>修改者</th>
      <th>示例</th>
      <th>描述</th>
      <th>可能值</th>
    </tr>
  </thead>
  <tbody>
    <tr><td class="modifier">CONTAINS</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："CONTAINS"，"value"："product"}</td><td>返回其字段值包含过滤器的记录</td><td class="possible">"新产品发布"</td></tr>
    <tr><td class="modifier">DOES_NOT_CONTAIN</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："DOES_NOT_CONTAIN"，"value"："product"}</td><td>返回字段值不包含过滤器的记录</td><td class="possible">"新启动项"</td></tr>
    <tr><td class="modifier">是</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS"，"value"："new product launch"}</td><td>返回字段值与过滤器完全匹配的记录</td><td class="possible">"新产品发布"</td></tr>
    <tr><td class="modifier">IS_NOT</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_NOT"，"value"："product"}</td><td>返回字段值与过滤器不完全匹配的记录</td><td class="possible">"新产品发布"</td></tr>
    <tr><td class="modifier">IS_EMPTY</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_EMPTY"}</td><td>返回字段值为空的记录</td><td class="possible">“”或null</td></tr>
    <tr><td class="modifier">IS_NOT_EMPTY</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_NOT_EMPTY"}</td><td>返回字段值不为空的记录</td><td class="possible">"新产品发布"</td></tr>
    <tr><td class="modifier">GREATER_THAN</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："GREATER_THAN"，"value"："10"}</td><td>返回字段值大于筛选器的记录</td><td class="possible">"11"</td></tr>
    <tr><td class="modifier">GREATER_THAN_OR_EQUAL</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："GREATER_THAN_OR_EQUAL"，"value"："10"}</td><td>返回字段值大于或等于过滤器的记录</td><td class="possible">"10", "11"</td></tr>
    <tr><td class="modifier">LESS_THAN</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："LESS_THAN"，"value"："10"}</td><td>返回字段值小于筛选器的记录</td><td class="possible">"9"</td></tr>
    <tr><td class="modifier">LESS_THAN_OR_EQUAL</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："LESS_THAN_OR_EQUAL"，"value"："10"}</td><td>返回字段值小于或等于过滤器的记录</td><td class="possible">"9", "10"</td></tr>
    <tr><td class="modifier">IS_BETWEEN</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_BETWEEN"，"value"：["2024-01-01"，"2024-12-31"]}</td><td>返回字段值介于两个筛选值之间的记录</td><td class="possible">["2024-03-01","2024-06-30"]</td></tr>
    <tr><td class="modifier">IS_NOT_BETWEEN</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_NOT_BETWEEN"，"value"：["2024-01-01"，"2024-12-31"]}</td><td>返回字段值不在两个筛选值之间的记录</td><td class="possible">["2023-01-01","2025-06-30"]</td></tr>
    <tr><td class="modifier">IS_AFTER</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_AFTER"，"value"："2024-01-01"}</td><td>返回日期字段值在筛选器之后的记录</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_BEFORE</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_BEFORE"，"value"："2024-12-31"}</td><td>返回日期字段值在筛选器之前的记录</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_ANY_OF</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_ANY_OF"，"value"：["Active"，"Planned"]}</td><td>返回字段值与筛选器列表中的任意值匹配的记录</td><td class="possible">["Active"，"Planned"，"Complete"]</td></tr>
    <tr><td class="modifier">IS_NONE_OF</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_NONE_OF"，"value"：["Active"，"Planned"]}</td><td>返回字段值不与筛选器列表中的值匹配的记录</td><td class="possible">[“活动”，“计划”]</td></tr>
    <tr><td class="modifier">HAS_ANY_OF</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："HAS_ANY_OF"，"value"：["Tag1"，"Tag2"]}</td><td>返回其多值字段包含任何筛选器值的记录</td><td class="possible">["Tag1"，"Tag2"]</td></tr>
    <tr><td class="modifier">HAS_ALL_OF</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："HAS_ALL_OF"，"value"：["Tag1"，"Tag2"]}</td><td>返回多值字段包含所有筛选值的记录</td><td class="possible">["Tag1"，"Tag2"]</td></tr>
    <tr><td class="modifier">IS_EXACTLY</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："IS_EXACTLY"，"value"：["Tag1"]}</td><td>返回其多值字段仅包含筛选值而不包含其他值的记录</td><td class="possible">["Tag1"]</td></tr>
    <tr><td class="modifier">HAS_NONE_OF</td><td class="example">{"fieldId"："&lt;id&gt;"，"condition"："HAS_NONE_OF"，"value"：["Tag1"]}</td><td>返回其多值字段不包含任何筛选器值的记录</td><td class="possible">["Tag1"]</td></tr>
  </tbody>
</table>


>[!NOTE]
>
>版本1注释： V1修饰符名称使用`$-prefixed camelCase` （例如`$contains`、`$isNot`、`$isEmpty`、`$greaterThan`、`$greaterThanOrEqual`、`$lessThan`、`$lessThanOrEqual`、`$isBetween`、`$isNotBetween`、`$isAnyOf`、`$hasAllOf`）。 每个修饰符的行为相同。


## 按字段类型支持的筛选条件

| 字段类型 | 支持的条件 |
|-----------------------------|--------------------------------------------------------------------------------------------------------------|
| 文本，长文本 | 包含、DOES_NOT_CONTAIN、IS、IS_NOT、IS_EMPTY、IS_NOT_EMPTY |
| 数字、百分比、货币 | IS、IS_NOT、GREATER_THAN、GREATER_THAN_OR_EQUAL、LESS_THAN、LESS_THAN_OR_EQUAL、IS_EMPTY、IS_NOT_EMPTY |
| 日期 | IS、IS_NOT、IS_AFTER、IS_BEFORE、IS_BETWEEN、IS_NOT_BETWEEN、IS_EMPTY、IS_NOT_EMPTY |
| 单选 | IS、IS_NOT、IS_ANY_OF、IS_NONE_OF、IS_EMPTY、IS_NOT_EMPTY |
| 多选，用户 | HAS_ANY_OF、HAS_ALL_OF、IS_EXACTLY、HAS_NONE_OF、IS_EMPTY、IS_NOT_EMPTY |
| 布尔 | 是 |
| 公式 | 包含、DOES_NOT_CONTAIN、IS、IS_NOT、IS_EMPTY、IS_NOT_EMPTY |
| 创建者 | IS、IS_NOT、IS_ANY_OF、IS_NONE_OF |
| 更新者 | IS、IS_NOT、IS_ANY_OF、IS_NONE_OF、IS_EMPTY、IS_NOT_EMPTY |
| created-at | IS、IS_NOT、IS_AFTER、IS_BEFORE、IS_BETWEEN、IS_NOT_BETWEEN |
| 更新时间 | IS、IS_NOT、IS_AFTER、IS_BEFORE、IS_BETWEEN、IS_NOT_BETWEEN、IS_EMPTY、IS_NOT_EMPTY |
| 引用 | HAS_ANY_OF、HAS_ALL_OF、IS_EXACTLY、HAS_NONE_OF、IS_EMPTY、IS_NOT_EMPTY |
| 查找 | 取决于链接的字段类型 |

>[!NOTE]
>
>**版本1注释：**&#x200B;版本1使用前缀为`$`的运算符名称（例如`$contains`、`$greaterThan`、`$isAnyOf`、`$hasAllOf`）。 每种字段类型支持的条件集是相同的。

## 按人员字段筛选

人员字段筛选器(`user`、`created-by`、`updated-by`、`approved-by`)接受Adobe IMS用户ID和Workfront用户ID。 纯字符串值将解释为Adobe IMS用户ID。

要设置标识符类型以检查Workfront用户ID，您需要显式传递`id`和`idType`参数。 对于Workfront用户ID，`idType`支持的值为“`WF`”；对于Adobe IMS用户ID，支持的值为“`IMS`”。

```
{ 
  "filter": { 
   "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<userFieldId>", 
        "condition": "HAS_ANY_OF", 
        "value": [ 
          { "id": "63e3b13000078c1795146248182d15dc", "idType": "WF" } 
        ] 
      } 
    ] 
  } 
} 
```

>[!NOTE]
>
> 版本1注意： V1仅支持按用户的IMS ID进行筛选。

## 按外部ID筛选外部引用字段

外部引用字段将记录链接到其他Adobe系统（如Workfront项目或AEM Assets）中的对象。 在内部，Planning将Planning记录ID分配给这些对象。 要直接按其原始对象ID筛选此类字段，请将`"matchExternalId": true`添加到筛选条件。

此标志仅对`referenceOptions.isExternal`为`true`的引用字段有效；对于非外部引用字段将忽略此标志。 如果无法解析单个字符串值，则请求将失败，并显示`400 Bad Request`。 如果提供了列表值，则未解析的条目将传递未更改并且只是不匹配而已。

```
{ 
  "filter": { 
    "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<externalReferenceFieldId>", 
        "condition": "IS_ANY_OF", 
        "value": [ 
          "5f6a4f6e00000123456789abcdef0123", 
          "/content/dam/wknd/en/adventures/bali-surf-camp" 
        ], 
        "matchExternalId": true 
      } 
    ] 
  } 
} 
```

>[!NOTE]
>
>版本1注意： V1不支持按外部对象ID进行筛选。

## 外部连接字段

Planning记录类型可以承载外部引用字段，这些字段将记录链接到其他Adobe系统中的对象，而不是其他Planning记录类型。

要通过API创建外部引用字段，请将新`REFERENCE`字段上的`referenceOptions.recordTypeId`设置为所需外部记录类型的ID。 服务器自动从目标记录类型派生`referenceOptions.isExternal=true`和连接元数据(`connectionName, objectName`)。

支持的外部对象类型包括Workfront对象（项目、任务、项目、项目群、项目组合、公司、组、团队、用户）和AEM Assets（资源、内容片段）。

>[!NOTE]
>
>版本1注意： V1不支持创建外部连接字段。


## 排序

通过在请求中包含`sort`数组来按任何字段对结果进行排序：

```
json
{
  "sort": [
    { "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" },
    { "fieldId": "F658afcbd4a0273c67c346fd5", "direction": "desc" }
  ]
}
```

按顺序评估多个排序字段。 在分页时始终应用排序，以确保跨页面排序一致。

要对结果分组，请在排序时包含一个组数组：

```
{ 
  "sort": [{ "fieldId": "F001", "direction": "asc" }], 
  "group": [{ "fieldId": "F002", "direction": "asc" }] 
} 
```

>[!NOTE]
>
>版本1注意： V1使用`sorting` （不是`sort`）、`groupingFieldIds` （字段ID数组，不是`group`对象）和现已弃用的`rowOrderViewId`来应用现有视图的行顺序。 版本中不支持这些V1参数

## 场投影

要限制响应中返回的字段，请使用逗号分隔列表的`fieldIds`或`fieldAliases`查询参数。 这减小了响应有效负载的大小，建议用于高容量集成或对延迟敏感的集成。

>[!NOTE]
>
>**版本1注释：**&#x200B;版本1使用`?attributes=`进行投影（例如`?attributes=data,createdBy`），而不是`?fieldIds=`或`?fieldAliases=`。

## 分页

Planning API支持分页响应以管理大型数据集。

* **基于游标的分页**&#x200B;用于工作区、记录类型、字段和视图。 传递上一个响应中的`cursor`值以检索下一页。 基于光标的响应包括hasMore标志，用于指示是否有更多页面。
* **基于页面的分页**&#x200B;用于记录搜索。 使用`page`和`size`作为查询参数。 在分页时始终应用排序，以确保跨页面排序一致。 请注意，分页是基于零的，因此要检索第二页的结果，请使用“`page=1`”作为参数。

例如，使用以下请求从记录搜索中检索包含500条记录的第二页：

```
POST /v2/record-types/{recordTypeId}/records/search?page=1&size=500 
{ 
  "sort": [{ "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" }], 
  "filter": { "operator": "AND", "conditions": [ 
    { "fieldId": "<fieldId>", "condition": "IS", "value": "active" } 
  ] } 
} 
```

所有分页的响应都包括一个结构化包络，指示是否还有更多结果可用。 在分页时始终应用排序，以确保跨页面排序一致。

>[!NOTE]
>
> **版本1注释：** V1使用请求正文中传递的`offset`和`limit`（默认为500，最大为2,000）。 要检索记录2001-4000，请在请求正文中设置“`offset`”：“`2000`”，“`limit`”：“`2000`”。 响应返回一个带有`totalCount`字段的平面记录数组。

## 批量操作

Planning API支持在单个请求中批量创建、更新、修补和删除记录。 有关终结点路径、请求格式和每个操作的记录限制，请参阅[developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning)上的&#x200B;**API引用**。

>[!NOTE]
>
>**版本1注意：**&#x200B;批量操作在版本1中不可用。


## 权限

实体的权限通过专用权限API进行管理，独立于资源端点本身。 这允许您读取当前权限、管理共享列表以及独立于数据操作处理访问请求。 有关详细信息，请参阅文章[Workfront规划API](https://developer.adobe.com/wf-planning)中的“API引用”部分。

>[!NOTE]
>
>**版本1注意：**&#x200B;版本1未公开公共权限API。 权限级别直接嵌入到资源响应DTO中。

## 将Planning API与Workfront自定义表单结合使用

您可以从Workfront自定义表单中的外部查找字段调用Planning API，以直接在Workfront对象中显示Planning数据。 有关详细信息，请参阅[自定义表单中的外部查找字段示例](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md)。

## 相关资源

有关更多与API相关的文档，另请参阅以下文章：

* [Workfront Planning API](https://developer.adobe.com/wf-planning)开发人员文档和参考
* [Adobe Workfront Planning入门](/help/quicksilver/planning/general/planning-overview.md)
* [Adobe Workfront Planning访问概述](/help/quicksilver/planning/access/access-overview.md)
* [为Workfront集成创建OAuth2应用程序](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)

<!--

Our version of this article before Lilit replaced it with the above: 

The goal for the Adobe Workfront Planning API is to simplify building integrations with Planning by introducing a REST-ful architecture that operates over HTTP. This document assumes you are familiar with REST and JSON responses and describes the approach taken by the Planning API.  

A familiarity with the Workfront Planning schema will assist you in understanding the database relationships that can be utilized to pull data out of Workfront Planning for integration purposes. 

You can call the planning API from an External lookup field in a Workfront custom form.

For more information on External lookup fields, see [Examples of the External lookup field in a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>When using the Planning API, all user-related information will be returned using the Adobe Identity Management System (IMS) user ID, and not the Workfront user ID.
>
>For information, see [Manage users in the Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).  

## Workfront Planning API versions

* Version 1 - released in July 2024 

  For more information, see the section [Workfront Planning API Version 1](#workfront-planning-api-version-1) in this article. 

* Version 2 - released in May 2026

  For more information, see the section [Workfront Planning API Version 2](#workfront-planning-api-version-2) in this article.


## Workfront Planning API Version 1

Workfront Planning API Version 1 was released in July 2024.

The following sections described functionality that was made available in the Workfront API Version 1. 

All future API version will contain the same functionality, unless otherwise specified. 

### Operations 

Objects are manipulated by sending an HTTP request to their unique URI. The operation to be performed is specified by the HTTP method. 

The standard HTTP methods correspond to the following operations: 

* **GET** - Retrieves an object by ID, searches for all objects by a query 
* **POST** - Inserts a new object 
* **PUT** - Edits an existing object 
* **DELETE** - Deletes an object 

For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

### Field types and search modifiers used with them 

You can use modifiers and filters with fields to control what data will be returned in results. 

For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

#### Using search modifiers 

Workfront Planning supports the following search modifiers: 

<table>
    <tr>
        <td><b>Modifier</b></td>
        <td><b>Example</b></td>
        <td><b>Description</b></td>
        <td><b>Possible Values</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>Returns records whose field value contains the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Returns records where the field value does not contain the filter  </td>
        <td>"New Launch"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Returns records whose field value exactly match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Returns records whose field value exactly is not match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is empty  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is not empty  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Returns records whose field value is greater than the filter  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is greater than or equal the filter  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Returns records whose field value is less than the filter  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is less than or equal the filter </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is after the filter  </td>
        <td>"2024-05-15T20:00:00.000Z"  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is before the filter </td>
        <td>"2024-05-12T20:00:00.000Z" </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is between the filter  </td>
        <td><ul><li>"2024-05-12T20:00:00.000Z" </li><li>"2024-05-14T20:00:00.000Z" </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is not between the filter  </td>
        <td><ul><li>"2024-05-09T20:00:00.000Z"  </li><li>"2024-05-17T20:00:00.000Z"  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is any of the filter  </td>
        <td><ul><li>"active" </li><li>"completed" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is none of the filter </td>
        <td><ul><li>"finished"  </li><li>"fixed"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has any of the filter  </td>
        <td><ul><li>["active", "fixed"]  </li><li>["fixed", "completed", "finished"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has all of the filter  </td>
        <td><ul><li>["active", "completed"]   </li><li>["active", "completed", "finished"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has none of the filter </td>
        <td>["fixed", "finished"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is exactly the filter  </td>
        <td>["active", "completed"]  </td>
    </tr>
</table>
 
#### Field types 

Below is the list of supported field types and what search modifiers can be used with each of those field types  

| Field Type | Supported search modifiers |
|---|---|
| text |$contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| long-text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| number | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| percentage | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| currency | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| date | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| single-select | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| multi-select | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| boolean | $is |
| user | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| formula | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| created-by | $is, $isNot, $isAnyOf, $isNoneOf |
| created-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| updated-by | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| updated-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| reference | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| lookup | Depends on the linked field |

### Using "And" and "Or" statements 

In the API call you can have filters that are based on several criteria combined by $and" and "$or" statements  

```
{
  "recordTypeId": "recordTypeId",
  "offset": "integer",
  "limit": "integer",
  "filters": [
    {
      "$or": [
        {
          "launch_date": {
            "$isBetween": [
              "2024-03-31T20:00:00.000Z",
              "2024-04-01T20:00:00.000Z"
            ]
          }
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-03-31T20:00:00.000Z",
                  "2024-04-01T20:00:00.000Z"
                ]
              }
            },
            {
              "status": "active"
            }
          ]
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-04-15T00:00:00.000Z",
                  "2024-04-16T00:00:00.000Z"
                ]
              }
            },
            {
              "status": "planned"
            }
          ]
        }
      ]
    }
  ]
}
```

### Using the fields request parameter 

You can use the fields request parameter to specify a comma-separated list of specific fields that should be returned. These field names are case-sensitive.  

For example, the request 

`/v1/records/search?attributes=data,createdBy`

```
{
    "records": [
        {
            "id": "Rc6527ecb35df57c441d92ba00",
            "createdBy": "61a9cc0500002f9fdaa7a6f824f557e1",
            "createdAt": null,
            "updatedBy": null,
            "updatedAt": null,
            "customerId": null,
            "imsOrgId": null,
            "recordTypeId": null,
            "data": {
                "F666c0b58b6fee61a2ea6ea81": [
                    {
                        "externalId": null,
                        "id": "Rc665728ff95730b58bc757b13",
                        "value": null
                    },
..
```

returns a response similar to the following: 

  
```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### Sorting query results in the API 

You can sort your results by any field if you append the following to your API call: 


`/v1/records/search`

Request body:

```
{
    "recordTypeId": "Rt6527ecb25df57c441d92b9fa",
    "filters": [],
    "sorting": [
        {
            "fieldId": "F6527ecb25df57c441d92b9fc",
            "direction": "asc"
        },
        {
            "fieldId": "F658afcbd4a0273c67c346fd5",
            "direction": "desc"
        }
    ],
    "limit": 500,
    "offset": 0,
    "rowOrderViewId": "V6527ecb75df57c441d92ba03",
    "groupingFieldIds": []
}
```

### Query limits and paginated responses 

By default, Planning API requests return 500 results, starting from the beginning of the list. To override the default limitation for number of results, you can use the `limit` parameter in your requests and set it to a different number, up to 2000 results.  

We recommend that you consider using paginated responses for large datasets by adding the `offset` parameter to your requests. Paginated responses allow you to specify the location of the first result that should be returned. 

For example, if you want to return the results 2001-4000, you can use the following request. This example returns 2000 records that are in active status, starting from the 2001st result: 

`POST /v1/records/search`


Request body: 

```
{ 
    "recordTypeId": "recordTypeId", 
    "offset": "2001", 
    "limit": "2000", 
    "filters": [ 
        { "status": "active" } 
    ] 
} 
```

To make sure your results are properly paginated, use a sorting parameter. This allows the results to be returned in the same order, so that the pagination does not repeat or skip results. 

For more information on sorting, see [Sorting query results in the API](#sorting-query-results-in-the-api) in this article.


Lilit did not want this organized like this - keeping this for reference: 

## Workfront Planning API Version 2

Version of the Workfront Planning API was released in May 2026. 

In addition to all the information contained in Version 1, the following enhancements were added in Version 2: 

* Search by the user's Workfront ID field instead of the user's IMS ID.

    This is applicable to custom People fields, as well as system fields such as Created By and Last Updated By fields.

* Ability to search by external connections (Workfront or AEM objects) via the API.

* Ability to link cross-workspace shared records through API. 

* Support all CRUD operations for workspaces, record types, fields, and views. 

* Enable permissions sharing for all sharable entities via API. 

    This includes workspaces, record types, and views. (***********and in the future also records and fields.*********)

* Support for uploading record thumbnail through API. 

-->