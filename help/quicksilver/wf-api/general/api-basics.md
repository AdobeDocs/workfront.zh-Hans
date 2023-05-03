---
content-type: api
navigation-topic: general-api
title: API 基础知识
description: API 基础知识
author: Becky
feature: Workfront API
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: 01f5970fc17f9390d48b00541c912d21ba77c0a4
workflow-type: tm+mt
source-wordcount: '4475'
ht-degree: 0%

---


# API 基础知识

Adobe Workfront API的目标是通过引入通过HTTP运行的REST风格架构来简化与Workfront的集成构建。 本文档假定您熟悉REST和JSON响应，并介绍了Workfront API采用的方法。

熟悉Workfront架构将有助于您了解可用于将数据从Workfront中提取以用于集成的数据库关系。

## 限制和准则

为确保Workfront按需系统性能的一致性，每个客户最多可以有10个并发API线程。 沙盒环境具有相同的限制，允许客户和合作伙伴在将代码发布到生产环境之前准确测试API调用。

对于生产、预览和测试驱动器环境，最终用户请求的URI长度上限为8892字节，因为这些请求将通过Workfront CDN(Akamai)进行路由。 此限制仅适用于通过CDN路由的URI。

>[!NOTE]
>
>此限制不适用于沙盒环境，因为沙盒环境未通过CDN路由。

### 免责声明

在生产环境中运行API之前，应在Workfront测试版环境中对API的任何使用进行测试。 如果任何客户使用API处理Workfront合理认为对按需软件造成负担的流程（即该流程会对其他客户的软件性能造成重大负面影响），则Workfront保留请求客户终止该流程的权利。 如果客户不遵守规定并且问题持续存在，Workfront将保留终止该流程的权利。

## REST基础知识

本节简要介绍如何与Workfront REST API进行交互，以遵循以下REST原则：

### 对象URI

系统中的每个对象都会获得一个唯一的URI，其中包含对象类型和ID。 以下示例显示描述三个唯一对象的URI:

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

对象类型不区分大小写，可以是缩写的ObjCode（如proj）或替代对象名称（项目）。

有关有效ObjCode的列表，请参阅  [API Explorer](../../wf-api/general/api-explorer.md).

### 操作

通过向对象的唯一URI发送HTTP请求来处理对象。 要执行的操作由HTTP方法指定。

标准HTTP方法与以下操作相对应：

* **GET**  — 按ID检索对象、按查询搜索所有对象、运行报告或执行命名查询
* **POST**  — 插入新对象
* **PUT**  — 编辑现有对象
* **DELETE**  — 删除对象

为了解决客户端缺陷或协议长度限制问题，可以使用方法参数覆盖HTTP行为。 例如，可以通过发布以下URI来实施GET操作：
<pre>GET/attask/api/v15.0/project?id=4c78...54d0&amp;method=get<br>GET/attask/api/v15.0/project/4c78...54d0?method=get</pre>

### 个回应

每个请求都会收到JSON格式的响应。 如果请求成功，则响应具有数据属性；如果出现问题，则具有错误属性。 例如，请求

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

返回与以下内容类似的JSON响应：


<pre>{<br>    "data":[<br>        {<br>            "percentComplete":0,<br>            "status":"CUR",<br>            "优先级":2,<br>            "name":“全新项目”，<br>            "ID":"4c7c08b20000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>通过浏览器的地址栏执行GET请求时，无需在请求中包含sessionID。

为PUT、POST和DELETE请求添加了特殊安全性。 导致写入数据库或从数据库中删除的任何请求，只能在 **sessionID=abc123** 包含在URI中。 以下示例显示如何查找DELETE请求：
<pre>GET/attask/api/v15.0/project?id=4c78...54d0&amp;method=delete&amp;sessionID=abc123<br>GET/attask/api/v15.0/project/4c78...54d0?method=delete&amp;sessionID=abc123</pre>

### 身份验证

API对每个请求进行身份验证，以确保客户端有权查看或修改请求的对象。

通过传递会话ID来执行身份验证，该会话ID可以使用以下方法之一提供：

#### 请求标头身份验证

首选的身份验证方法是传递名为SessionID的请求标头，该标头包含会话令牌。 这样做有安全的优势 [跨站点请求伪造(CSRF)](http://en.wikipedia.org/wiki/Cross-site_request_forgery) 攻击和不干扰URI以进行缓存。

以下是请求标头的示例：

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### 请求参数身份验证

您可以通过传递名为sessionID的请求参数进行身份验证，如以下示例所示： 

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0?sessionID=abc1234
```

#### 基于Cookie的身份验证

API使用与Web UI用于系统的相同的基于Cookie的身份验证。 其中，如果客户端使用Web UI登录Workfront，则从同一浏览器中发出的任何AJAX调用都会使用相同的身份验证。

>[!NOTE]
>
>为了防止CSRF（跨站点请求伪造）攻击的可能性，此身份验证方法仅可用于只读操作。

## 登录

>[!IMPORTANT]
Workfront不再建议使用 `/login` 端点或API密钥。 请改用以下身份验证方法之一：
* 使用JWT进行服务器身份验证
* 使用OAuth2进行用户身份验证
>
有关设置这些身份验证方法的说明，请参阅 [为Workfront集成创建OAuth2应用程序](../../administration-and-setup/configure-integrations/create-oauth-application.md)
有关在Workfront中使用服务器身份验证的说明，请参阅 [使用JWT流程配置和使用贵组织的自定义OAuth 2应用程序](../../wf-api/api/oauth-app-jwt-flow.md)
有关在Workfront中使用用户身份验证的说明，请参阅 [使用授权代码流配置和使用贵组织的自定义OAuth 2应用程序](../../wf-api/api/oauth-app-code-token-flow.md)

>[!NOTE]
本节所述的程序仅适用于尚未载入Adobe业务平台的组织。 如果贵组织已载入Workfront业务平台，则通过Workfront API登录Adobe将不可用。
有关根据贵组织是否已载入Adobe业务平台而不同的程序列表，请参阅 [基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

使用有效的用户名和密码，您可以使用以下请求获取会话ID:

```
POST /attask/api/v15.0/login?username=admin&password=user
```

这会设置一个Cookie来验证将来的请求，并返回具有新创建的sessionID、已登录用户的用户ID和其他会话属性的JSON响应。

>[!NOTE]
如果您的指定API用户也是管理员，Workfront强烈建议您使用API密钥登录。

**生成API密钥**

当您以该用户身份登录系统时，可以生成API密钥，如以下示例所示：


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**检索之前生成的API密钥**

您还可以通过运行getApiKey来检索之前为特定用户生成的API密钥：


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

然后，您可以使用此结果来验证任何API调用，方法是将“apiKey”添加为具有此值的请求参数，以代替sessionID或用户名和密码。 这从安全角度是有益的。

以下请求是使用apiKey从项目检索数据的示例：

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**使API密钥失效**

如果apiKey值已被泄露，您可以运行“clearApiKey”以使当前API密钥失效，如以下示例所示：

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

清除后，您可以再次运行getApiKey以生成新的API密钥。

### 注销

会话完成后，您可以使用以下请求将用户注销，从而阻止进一步访问sessionID。

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

要注销的sessionID可以指定为Cookie、请求标头或请求参数。

注销用户：

1. 导航到您的登录屏幕，但不登录。
1. 将URL更改为/attask/api/v15.0/project/search。\
   请注意，找不到该页面。
1. 替换单词 *搜索* 使用login?username=admin&amp;password=user，替换您的用户名和密码 *管理员* 和*用户\
   *此会话作为Cookie存储在浏览器中，无需在每个后续GET请求中重述。

1. 将URL更改回 **/attask/api/v15.0/project/search**.
1. 请注意提供的响应。

执行PUT、POST和DELETE请求时，必须始终包含在登录后提供的sessionID。

## GET行为

使用HTTPGET方法检索一个或多个对象并运行报表。

### 检索对象

您可以使用修饰符和过滤器增强对对象的搜索。

#### 使用对象ID检索对象

如果您知道对象的ID，则可以通过访问对象的唯一URI来检索该对象。 例如，请求

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

返回与以下类似的响应：

<pre>{<br>    "percentComplete":0,<br>    "status":"CUR",<br>    "优先级":2,<br>    "name":“全新项目”，<br>    "ID":"4c7c08b20000002de5ca1ebc19edf2d5" <br>}</pre>


您可以通过指定ID请求参数并提供ID列表（以逗号分隔）来检索同一请求中的多个对象，如以下示例所示：


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

请注意， /attask/api/v15.0/project?id=...请求与 `/attask/api/v15.0/project/...` 请求。

#### 使用URI检索对象

如果要按ID以外的条件检索对象，可以搜索URI。

例如，您可以使用以下请求返回系统中所有项目的列表：

```
GET /attask/api/v15.0/project/search
```

您可以使用请求参数作为名称 — 值对指定过滤器。 例如，以下示例显示了一个可找到所有当前项目的请求：

```
GET /attask/api/v15.0/project/search?status=CUR
```

以下请求会查找尚未完成且分配给名为John的用户的所有任务。

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### 使用搜索修饰符

下表列出了可与Workfront API一起使用的一些修饰符。

| **修改者** | **描述** | **示例** |
|---|---|---|
| eq | 返回状态为“已关闭”的结果 | <pre>...status=cls&amp;status_Mod=eq...</pre> |
| ne | 返回不处于“已关闭”状态的结果 | <pre>...status=cls&amp;status_Mod=ne...</pre> |
| get | 返回完成百分比大于或等于50的结果 | <pre>...percentComplete=50&amp;percentComplete_Mod=get...</pre> |
| lte | 返回完成百分比小于或等于50的结果 | <pre>...percentComplete=50&amp;percentComplete_Mod=lte...</pre> |
| isnull | 返回描述为Null的结果 | <pre>...description_Mod=isnull...</pre> |
| notnull | 返回描述不为Null的结果 | <pre>...description_Mod=notnull...</pre> |
| 包含 | 返回名称包含“Workfront”的结果 | <pre>...name=Workfront&amp;name_Mod=contains...</pre> |
| 介于 | 返回过去7天内具有登入日期的结果 | <pre>...entryDate=$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between...</pre> |

{style="table-layout:auto"}

>[!NOTE]
搜索请求区分大小写。 如果您收到错误，请确保  **修改(_M)** 和 **范围(_R)** 大小写正确。

#### 使用OR语句

您可以通过添加包含“OR”的参数以及用于指示过滤器或一系列过滤器级别的数字来增强搜索。

OR语句只返回API调用中满足OR语句筛选条件的记录。 OR语句级别中不包含过滤器。

例如，如果要筛选

* 名称包含“Planning”或
* 名为“FixedAssets” AND的组合中的任务分配给名称包含“Steve”OR的人员
* 具有名为“最终任务”的父任务的任务

然后，将以下API调用及其多个OR语句结合使用：
<pre>GET/attask/api/v15.0/task/search?name=Planning<br>&amp;name_Mod=contains<br>或(&amp;O):1:portfolio:name=FixedAssets<br>或(&amp;O):1:组合：name_Mod=eq<br>或(&amp;O):1:assignedTo:name=Steve<br>或(&amp;O):1:assignedTo:name_Mod=cicontains<br>或(&amp;O):2:parent:name=final Task<br>或(&amp;O):2:parent:name_Mod=eq
</pre>

#### 使用过滤器参数

使用URL参数进行搜索过滤器的一个潜在陷阱是，Workfront在检查不同的身份验证方法（例如，用户名、密码、apiKey、Cookie）之前会解析某些参数。 发生这种情况时，参数不会用作调用中的过滤器。 

要避免出现此问题，您可以将这些值置于具有JSON格式的过滤器参数中。 例如，如果要筛选用户名testuser，而不是使用 
<pre>/attask/api/v15.0/user/search?username=testuser@workfront.com</pre>在过滤器中传递URL参数，如以下示例所示：
<pre>/attask/api/v15.0/user/search?filters={"username":"testuser@workfront.com"}</pre>

#### 使用映射请求参数

默认情况下，从搜索返回的数据是JSON数组。 根据您的用例，将结果作为JSON对象按ID编入索引可能会更有效。 可以使用映射请求参数完成此操作。 例如，请求 
<pre>/attask/api/v15.0/task/search?map=true</pre>返回由ID索引的响应，如下所示：
<pre>{<br>    "data":{<br>        "4c9a97db0000000f13ee446b9aead9b":{<br>            "percentComplete":0,<br>            "status":“新”，<br>            "name":"第一项任务",<br>            "ID":"4c9a97db0000000f13ee446b9aead9b",<br>            "taskNumber":1 <br>        },<br>        "4ca28ba600002024cd49e75bd43cf601":{<br>            "percentComplete":0,<br>            "status":"INP:A",<br>            "name":"第二项任务",<br>            "ID":"4ca28ba600002024cd49e75bd43cf601",<br>            "taskNumber":2 <br>        } <br>    } <br>}</pre>

#### 使用字段请求参数

默认情况下，检索对象仅返回最常用的字段子集。

您可以使用字段请求参数指定返回的特定字段列表（以逗号分隔）。 例如，请求
<pre>/attask/api/v15.0/task/search?fields=plannedStartDate，priority</pre>返回与以下类似的响应：
<pre>{<br>    "优先级":2,<br>    "name":"第一项任务",<br>    "ID":"4c7c08fa0000002ff924e298ee148df4",<br>    "planedStartDate":"2010-08-30T09":00:00:00-0600” <br>}</pre>

>[!NOTE]
这些字段名称区分大小写。

有关可能的字段引用列表，请参阅  [API Explorer](../../wf-api/general/api-explorer.md)

#### 搜索嵌套对象

您可以搜索嵌套对象。 默认情况下，返回的嵌套对象只包含名称和ID。 例如，要获取所有问题及其所有者，请使用以下请求：
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>如果需要更多信息，可以使用冒号语法请求嵌套字段。 例如，以下请求会搜索所有问题以及所有者的姓名、ID、标题和电话号码
<pre>/attask/api/v15.0/issue/search?fields=owner:title，owner:phoneNumber</pre>和会返回以下内容： 
<pre>{<br>    "name":“重要问题”，<br>    "ID":"4c78285f00000908ea8cfd66e084939f",<br>    "owner":{<br>        "title":“运营专家”，<br>        "phoneNumber":《555-1234》，<br>        "name":“管理员用户”、<br>        "ID":"4c76ed7a0000054c172b2c2d9f7f81c3" <br>    } <br>}</pre>

#### 检索嵌套收藏集

您可以检索对象的嵌套集合。 例如，要获取包含其所有任务的项目，请使用以下请求：
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>以下请求获取任务分配：
<pre>/attask/api/v15.0/task/search?fields=assignments</pre>

#### 搜索多个嵌套字段

默认情况下，只返回每个任务的名称和ID，但可以使用冒号语法指定其他嵌套字段。 要查看相关对象或集合的所有可用字段，只需在对象/集合引用中附加一个冒号和星号即可。
<pre>/attask/api/v15.0/task/search?fields=assignments:*</pre>

#### 检索自定义数据

您可以使用前缀“DE：”检索自定义数据字段。 例如，要请求具有名为“CustomText”的参数的项目，请使用以下请求：
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>会返回
<pre>{<br>    "name":"自定义数据项目",<br>    "ID":"4c9a954f0000001afad0687d7b1b4e43",<br>    "DE:CustomText":"任务b" <br>}</pre>您还可以通过请求parameterValues字段来检索对象的所有自定义数据。 例如， 
<pre>/attask/api/v15.0/project/search?fields=parameterValues</pre>返回与以下内容类似的数据：
<pre>{<br>    "name":"自定义数据项目",<br>    "ID":"4c9a954f0000001afad0687d7b1b4e43",<br>    parameterValues:{ <br>        "DE:CustomText":"任务b", <br>        "DE:CustomNumber":1.4, <br>        "DE:CustomCheckBoxs":["first","second","third"] <br>    } <br>}</pre>

#### 使用命名查询

某些对象类型具有命名的搜索，这些搜索通常会执行，通过将查询的名称附加到对象类型URI的末尾，即可使用。 例如，以下请求会检索用户当前被分配到的工作项（任务和问题）：
<pre>/attask/api/v15.0/work/myWork</pre>命名查询支持请求字段参数以检索其他字段。 某些命名查询还接受其他过滤器。 有关允许的命名查询对象的列表，请参阅[API资源管理器](../../wf-api/general/api-explorer.md)中该对象的“操作”选项卡。

#### 使用计数过滤器

您可以指定希望由给定搜索返回的结果数。 这样，服务器就可以更快地处理请求并节省带宽。 例如，请求
<pre>GET/attask/api/v15.0/project/count?status=CUR</pre>以下格式返回结果数：
<pre>{<br>    "count":3 <br>}</pre>与发送完整对象相比，此结果的下载量要小得多。 筛选器语法与搜索命令相同。

### 请求报告

您可以执行报表请求，其中只需要使用一个或多个分组聚合某些字段。 如以下示例所示，报表语法与SOAP API的语法相同：
<pre>GET/attask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>返回以下结果
<pre>{<br>    “第一个项目”：{ <br>        "sum_hours":15 <br>    }, <br>     “第二个项目”：{ <br>        "sum_hours":30 <br>    } <br>}</pre>添加$$ROLLUP=true参数在每个分组级别包含总计：
<pre>{<br>    “第一个项目”：{ <br>        "sum_hours":15 <br>    }, <br>    “第二个项目”：{ <br>        "sum_hours":30 <br>    }, <br>    "$$ROLLUP":{ <br>        "sum_hours":45 <br>    } <br>}</pre>

### 在API中对查询结果排序

如果在API调用中附加以下内容，则可以按任意字段对结果进行排序：

&amp;entryDate_Sort=asc

例如，如果要按任务计划起始日期排序，请删除entryDate并将其替换为planededCompletionDate。

这适用于Workfront中的大多数字段。

### 考虑查询限制

在查询对象时，应特别考虑相关对象的关系和搜索限制。 例如，如下表所示，项目查询最多可返回2,000个项目。 这2,000个项目被视为“主要对象”。 如果在项目中查询“任务”字段，则“任务”字段（作为集合）将成为主对象“项目”的辅助对象。 “任务”字段的查询可以包含项目中的数千个任务。 返回的对象（项目和任务）总数不能超过50,000个。

为确保获得最佳性能，下表显示了对搜索请求的限制。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>查询结果</th> 
   <th>限制</th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td width="200">默认结果数</td> 
   <td>100</td> 
   <td> 如果查询筛选器中未指定任何限制（即$LIMIT），则结果可能最多包含100个主对象。 <br>请参阅 <a href="#using-paginated-responses" class="MCXref xref">使用分页响应</a> 有关如何覆盖此限制的说明。 </td> 
  </tr> 
  <tr> 
   <td>最大结果数</td> 
   <td>2,000</td> 
   <td>查询过滤器（即$LIMIT）返回的结果最多不超过2000个。 有关更多信息，请参阅“分页响应”。</td> 
  </tr> 
  <tr> 
   <td>最大字段深度</td> 
   <td>4</td> 
   <td>在确定要显示的字段时，不能超过四个级别，离要查询的对象。</td> 
  </tr> 
  <tr> 
   <td>最大对象数</td> 
   <td>50,000</td> 
   <td>结果集不能包括50000个主对象和辅助对象。</td> 
  </tr> 
  <tr> 
   <td>最大字段数</td> 
   <td nowrap>1,000,000</td> 
   <td>当结果集少于50000个对象时，结果最多可能包含1,000,000个字段。</td> 
  </tr> 
  <tr> 
   <td>最大批次创建/更新数</td> 
   <td>100</td> 
   <td>批创建或更新的最大限制为100。</td> 
  </tr> 
 </tbody> 
</table>

### 使用分页响应 {#using-paginated-responses}

要覆盖“结果的默认数量”查询限制并允许200个结果，您可以包括 `$$LIMIT=200` 过滤器，如以下示例所示：
<pre>GET/attask/api/v15.0/project/search?$$LIMIT=200</pre>

为确保系统中其他租户的可靠性和性能，每个查询允许的结果上限为2000个对象。 尝试指定更大的限制将导致 `IllegalArgumentException` 错误消息。 

因此，我们建议您考虑对大型数据集使用分页响应。 要指定应返回的第一个结果，请添加 `$$FIRST` 过滤器。 例如，以下请求会为查询返回结果201-250:
<pre>GET/attask/api/v15.0/project/search?$$FIRST=200&amp;$LIMIT=50</pre>

请注意，在上例中， `$$FIRST=200` 返回第201个结果。 `$$FIRST=0` 会返回第一个结果。 将$$FIRST值视为您要在返回结果之前跳过的结果数可能会有所帮助。

要确保对结果进行正确分页，请使用排序参数。 这样可以按相同顺序返回结果，以便分页不会重复或跳过结果。 例如，要使用对象ID排序，请使用 `ID_Sort=asc`.

### 创建访问规则

您可以创建访问规则以确定谁可以访问对象。 以下是您可以设置的访问规则示例：

要设置项目以便仅与ID为“abc123”的用户共享该项目，请使用以下请求：
<pre>GET/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxx?method=put &amp;updates={ accessRules:[ {accessorID:'abc123',accessorObjCode:“USER”，coreAction:'VIEW'} ] }</pre>或者，要仅与新人员共享并保持现有权限不变，请执行以下操作：
<pre>GET/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>要检索现有访问规则，请执行以下操作：
<pre>GET/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## POST行为

POST插入新对象。 语法与PUT相同，但有少数例外。 由于新对象尚不存在，因此它没有ID。 因此，URI不包括ID。

### 创建对象

以下示例用于请求创建新项目：
<pre>POST/attask/api/v15.0/project?name=New Project</pre>响应包括新创建的项目及其新ID和指定的任何其他字段。

### 复制对象

某些对象支持复制。 对于这些对象类型，可以通过使用copySourceID参数发布来创建新对象。 例如，以下请求会复制给定的项目并为其提供一个新名称：

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### 上传文档

您可以通过以下API URL上传文档：
<pre>POST/attask/api/v15.0/upload</pre>API要求内容类型为multipart/form-data。 文件的参数名称必须为uploadedFile。 服务器会返回以下JSON数据：
<pre>{<br>    "handle":"4c7c08fa0000002ff924e298ee148df4"<br>}</pre>创建Workfront文档时，可以使用句柄并发布到以下URL:
<pre>POST/attask/api/v15.0/document?updates={<br>    名称：aFileName，<br>    句柄：abc...123，（文件上传中的句柄）<br>    docObjCode:PROJ（或TASK、OPTASK等）<br>    objID:abc...123,<br>    currentVersion:{version:v1.0,fileName:aFileName}<br>}</pre>

## PUT行为

PUT用于更新现有对象。

PUT的响应与GET相同。 在这两种情况下，服务器都会在更新后返回对象的新状态。 所有用于更改对GET请求的响应的规则也都适用于PUT，例如指定要返回的其他字段、自定义数据等。

### 编辑对象

对象的更新始终由ID使用对象的唯一URI来完成。 要更新的字段指定为请求参数。 例如，要更改项目名称，您可以发送类似于以下内容的请求：
<pre>PUT/attask/api/v15.0/project/4c7...?name=New Project Name <br>PUT/attask/api/v15.0/project?id=4c7...&amp;name=新建项目名称</pre>由于更新需要ID，因此如果服务器上不存在对象，则此操作将失败（不插入）。

### 指定JSON编辑

如以下示例中所示，您可以使用更新请求参数指定要使用JSON语法更新的字段：
<pre>PUT/attask/api/v15.0/project/4c7...?更新= <br>{<br>     名称："新建项目名称", <br>     状态："CUR", <br>     ... <br>}</pre>

### 进行嵌套更新

某些对象具有可更新的私有集合。 例如，以下示例演示了如何覆盖给定任务的现有分配：
<pre>PUT/attask/api/v15.0/task/4c7...?更新= <br>{<br>    分配：[ <br>        { <br>            assignedToID:“222...54d0, <br>            assignmentPercent:50.0 <br>        },{ <br>            roleID:“111...54d0”<br>        } <br>    ] <br>}</pre>

>[!NOTE]
虽然对顶级进行的更新是稀疏的，但对集合或嵌套对象的更新会完全替换现有集合。 要在不影响对象的情况下编辑任务上的单个分配，请对该分配使用PUT，而不是对任务使用。

以下示例将项目设为公共服务台队列。 请注意，现有队列属性将被替换。
<pre>PUT/attask/api/v15.0/project/4c7...?更新= <br>{ <br>    queueDef:{ <br>        isPublic:1 <br>    } <br>}</pre>

### 使用操作请求参数

某些对象支持除简单编辑之外可执行的其他操作。 您可以使用操作请求参数指定这些操作。 例如，以下请求会重新计算给定项目的时间轴：
<pre>PUT/attask/api/v15.0/project/4c7...?action=calculateTimeline<br><br>或<br><br>PUT/attask/api/v15.0/project/4c7.../calculateTimeline </pre>

### 移动对象

下面演示了将任务从一个项目移动到另一个项目的语法：
<pre>PUT/attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>下面提供了每个操作类型的示例：(??)
<pre>PUT/attask/api/v15.0/project/1234/approveApproval<br><br>PUT/attask/api/v15.0/project/1234/calculateFinance<br><br>PUT/attask/api/v15.0/project/1234/calculateTimeline<br><br>PUT/attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT/attask/api/v15.0/project/1234/recallApproval<br><br>PUT/attask/api/v15.0/project/1234/rejectApproval<br><br>PUT/attask/api/v15.0/task/1234/move<br><br>PUT/attask/api/v15.0/workitem/1234/markViewed</pre>只有移动操作需要标识其他属性才能指定要移动工作项的项目。

以下是每个操作类型的示例： 
<pre>PUT/attask/api/v15.0/project/1234?method=put&amp;updates={accessRules:[{accessorID:'abc123',accessorObjCode:“USER”，coreAction:'VIEW'}]}</pre>

### 共享对象

以下示例演示了与团队共享项目的语法：
<pre>PUT/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxx&amp;accessorObjCode=TEAMOB</pre>在编辑对象时，您可以通过执行类似以下示例的PUT并发送更新来替换对象上的所有访问规则：
<pre>PUT/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxxxxxxxxx',accessorObjCode:'TEAMOB',coreAction:'VIEW'}]}</pre>以下示例显示了将任务从一个项目移动到另一个项目的语法：
<pre>PUT/attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>

## DELETE行为

DELETE会删除对象。 在每种情况下，URI都可能包含参数force=true ，以使服务器删除指定的数据及其受属数据。 在以下示例中，通过对URI执行HTTPDELETE方法来删除任务：
<pre>DELETE/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE/attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0?force=true <br>DELETE/attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0?force=true</pre>

## 批量更新

批量更新语句在单个API调用中同时更新多个对象。 批量创建API调用的构建方式与常规更新调用类似，如以下示例所示：
<pre>PUT/attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxx</pre>这会产生与以下内容类似的返回：
<pre>数据：[{<br>    ID:"53ff8d3d003b438b57a8a784df38f6b3",<br>    名称："Test_Project_1",<br>    objCode:"PROJ",<br>    percentComplete:0,<br>    planedCompletionDate:"2014-08-28T11":00:00:00-0400”，<br>    planedStartDate:"2014-08-28T11":00:00:00-0400”，<br>    优先级：0,<br>    protedCompleteDate:"2014-08-28T16":12:00:00-0400”，<br>    状态："CUR"<br>},<br>{<br>    ID:"53ff8d49003b43a2562aa34eea3b6b10",<br>    名称："Test_Project_2",<br>    objCode:"PROJ",<br>    percentComplete:乌西，<br>    planedCompletionDate:"2014-08-28T11":00:00:00-0400”，<br>    planedStartDate:"2014-08-28T11":00:00:00-0400”，<br>    优先级：0,<br>    protedCompleteDate:"2014-08-28T16":12:00:00-0400”，<br>    状态："CUR"<br>}]</pre>您还可以执行类似以下内容的批量更新：
<pre>PUT/attask/api/v15.0/proj?Umethod=PUT&amp;updates=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_Edit"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_2_Edit"}]&amp;api=123xxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>这会产生与以下内容类似的返回：
<pre>数据：[ {<br>     ID:"53ff8e15003b461d4560f7f65a440078",<br>     名称："Test_Project_1_Edit",<br>     objCode:"PROJ",<br>     percentComplete:0,<br>     planedCompletionDate:"2014-08-28T11":00:00:00-0400”，<br>     planedStartDate:"2014-08-28T11":00:00:00-0400”，<br>     优先级：0,<br>     protedCompleteDate:"2014-08-28T16":16:00:00-0400”，<br>     状态："CUR"<br>},<br>{<br>    ID:"53ff8e19003b46238a58d303608de502",<br>    名称："Test_Project_2_Edit",<br>    objCode:"PROJ",<br>    percentComplete:0,<br>    planedCompletionDate:"2014-08-28T11":00:00:00-0400”，<br>    planedStartDate:"2014-08-28T11":00:00:00-0400”，<br>    优先级：0,<br>    protedCompleteDate:"2014-08-28T16":16:00:00-0400”，<br>    状态："CUR"<br>}]</pre>如果您希望在同一事务中执行所有操作，请将“atomic=true”作为请求参数添加到批量API调用中。 这样，如果任何操作都失败，所有操作都将回滚。

>[!NOTE]
原子批处理操作只能返回“成功：true”或错误。
