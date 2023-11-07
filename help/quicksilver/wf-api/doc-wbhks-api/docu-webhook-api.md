---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 文档Webhooks API
description: 文档Webhooks API
author: Becky
feature: Workfront API
role: Developer
exl-id: 7ac2c6c8-1cb8-49df-8d63-a6b47ad02a13
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '3646'
ht-degree: 3%

---


# 文档Webhooks API

Adobe Workfront Document Webhooks定义了一组API端点，Workfront通过这些API端点向外部文档提供商发出授权的API调用。 这允许任何人为任何文档存储提供商创建中间件插件。

基于webhook的集成的用户体验将与现有文档集成的用户体验类似，例如Google Drive、Box和Dropbox。 例如，Workfront用户将能够执行以下操作：

* 导航外部文档提供程序的文件夹结构
* 搜索文件
* 将文件链接到Workfront
* 将文件上载到外部文档提供商
* 查看文档的缩略图

## 参考实施

为了帮助快速启动新的Webhooks实施的开发，Workfront提供了一个参考实施。 此功能的代码可在以下位置找到： [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). 此实施基于Java，允许Workfront通过网络文件系统连接文档。

## 注册Webhook集成

Workfront管理员可以通过导航到Workfront中的设置>文档>自定义集成，为其公司添加自定义webhook集成。 在“设置”的“自定义集成”页面中，管理员可以查看现有文档Webhook集成的列表。 在此页面中，可以添加、编辑、启用和禁用集成。 要添加集成，请单击“添加集成”按钮。

### 可用字段

添加集成时，管理员将在以下字段中输入值：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>字段名称</th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>名称</td> 
   <td>此集成的名称。</td> 
  </tr> 
  <tr> 
   <td>基本 API URL</td> 
   <td> <p>回调API的位置。 调用外部系统时，Workfront只需将端点名称附加到此地址即可。 例如，如果管理员输入基本API URL " https://www.mycompany.com/api/v1 "，Workfront将使用以下URL获取文档的元数据：https://www.mycompany.com/api/v1/metadata?id=1234。</p> </td> 
  </tr> 
  <tr> 
   <td>请求参数</td> 
   <td> <p>要附加到每个 API 调用的查询字符串的可选值。例如，access_type=offline。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>身份验证类型</td> 
   <td>OAuth2或ApiKey</td> 
  </tr> 
  <tr> 
   <td>身份验证 URL</td> 
   <td> <p>（仅限OAuth2）用于用户身份验证的完整URL。 在OAuth配置过程中，Workfront会将用户导航到此地址。 注意：Workfront会将“state”参数附加到查询字符串中。 提供程序必须通过将它附加到Workfront重定向URI来将它传递回Workfront。</p> </td> 
  </tr> 
  <tr> 
   <td>令牌端点 URL</td> 
   <td> <p>（仅限OAuth2）用于检索OAuth2令牌的完整API URL。 它由webhook提供程序或外部文档提供程序托管</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>客户端 ID</td> 
   <td>（仅限OAuth2）此集成的OAuth2客户端ID</td> 
  </tr> 
  <tr> 
   <td>客户端密码</td> 
   <td> <p>（仅限OAuth2）此集成的OAuth2客户端密钥</p> </td> 
  </tr> 
  <tr> 
   <td>Workfront 重定向 URI</td> 
   <td>  <p>（仅限OAuth2）这是只读字段，由Workfront生成。 此值用于将该集成注册到外部文档提供商。 注意：如上所述，对于身份验证URL，提供程序必须在执行重定向时将“state”参数及其值附加到查询字符串。</p></td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td>  <p>（仅限ApiKey）用于向webhook提供程序进行授权的API调用。 webhook提供程序发布的API密钥。</p></td> 
  </tr> 
 </tbody> 
</table>

 

## 身份验证

Workfront文档webhook支持两种不同的身份验证形式：OAuth2和ApiKey。 在这两种情况下，Workfront在进行API调用时在标头中传递身份验证令牌。

### OAuth2

OAuth2允许Workfront代表用户向webhook提供程序发出授权的API调用。 在执行此操作之前，用户必须将其外部文档提供商帐户连接到Workfront并授予Workfront

代表他们行事的权限。 此握手过程仅针对每个用户发生一次。 以下是它的工作方式：

1. 用户开始将webhook集成连接到其帐户。 目前，可通过单击“添加文档”下拉列表>“添加服务”>自定义集成名称来完成此操作。
1. Workfront会为用户导航身份验证URL，这可能会提示用户登录到外部文档提供商。 此页面由webhook提供程序或外部文档管理系统托管。 在执行此操作时，Workfront会向身份验证URL添加“state”参数。 必须在以下步骤中，通过将相同的值附加到Workfront返回URI，将此值传递回Workfront。
1. 登录到外部系统后（或者如果用户已登录），用户将被带到“身份验证”页面，该页面解释Workfront正在请求访问权限以代表用户执行一组操作。
1. 如果用户单击“允许”按钮，浏览器将重定向到Workfront重定向URI ，并添加“code=`<code>`”到查询字符串。 根据OAuth2规范，此令牌的生命周期短。 查询字符串还必须具有以下“state=`<sent_by_workfront>`“。
1. Workfront处理此请求，并使用授权代码对令牌端点URL进行API调用。
1. 令牌端点URL返回刷新令牌和访问令牌。
1. Workfront存储这些令牌并完全为此用户预配webhook集成。
1. 从此刻起，Workfront将能够向webhook提供商发出授权的API调用。 进行这些调用时，Workfront将在HTTP请求标头中发送访问令牌，如下所示：

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. 如果访问令牌已过期，Workfront将调用令牌端点URL以检索新的访问令牌，然后尝试使用新的访问令牌再次尝试授权API调用。

### ApiKey

使用ApiKey向webhook提供程序进行授权API调用比OAuth2简单得多。 进行API调用时，Workfront只需在HTTP请求标头中传递ApiKey和Workfront用户名即可：

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Webhook提供程序可以使用用户名来应用特定于用户的权限。 当两个系统都使用单点登录(SSO)连接到LDAP时，这种方法效果最佳。

### 添加请求标头（可选）

除了使用OAuth2令牌或ApiKey进行身份验证之外，Workfront还可以为每个API调用向webhook提供程序发送一组预定义的标头。 Workfront管理员可以在注册或编辑Webook集成时进行此设置，如上面的部分所述。 请参阅注册Webhook集成。

例如，这可用于基本身份验证。 为此，Workfront管理员将在自定义集成对话框中添加以下请求标头信息：

   授权基本QWxhZGRpbjpvcGVuIHNlc2FtZQ==

其中，QWxhZGRpbjpvcGVuIHNlc2FtZQ==是“username：password”的base-64编码字符串。 请参阅基本身份验证。 如果添加了此标头，Workfront将会在HTTP请求标头中传递此标头，以及其他请求标头：

```
­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------

apiKey: 12345

username: johndoe@foo.com

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

## API规范

以下是webhook提供程序应该实施的API列表，以便文档webhook正常工作。

### 获取OAuth2令牌（仅需要OAuth2身份验证）

返回经过身份验证的用户的OAuth2刷新令牌和访问令牌。 当用户设置文档提供商时，将调用一次。 随后进行调用以获取更新的访问令牌。

HTTP请求POST/any/url

该URL是可配置的，并且对应于自定义集成设置页面上的令牌端点URL值。

**查询参数**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名称</th> 
   <th>必填</th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>grant_type</td> 
   <td>是</td> 
   <td> <p>值包括“authorization_code”或“refresh_token”。 指定的值指示将传递到此API调用的两个参数中的哪个：code或refresh_token。</p> </td> 
  </tr> 
  <tr> 
   <td>代码</td> 
   <td>根据</td> 
   <td> <p>用户单击“Grant”按钮后发送到Workfront的授权代码。 仅当授权类型为“authorization_code”时才需要此项。 授权码应为短期，通常在10分钟或更短时间内过期。</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token</td> 
   <td>根据</td> 
   <td> <p>仅当进行后续调用以检索新的access_token时，才需要此项，因为之前的access_token已过期。 发送此值时，请将grant_type参数设置为“refresh_token”。</p> </td> 
  </tr> 
  <tr> 
   <td>client_id</td> 
   <td>是</td> 
   <td>在Workfront中为此自定义集成配置的客户端ID。</td> 
  </tr> 
  <tr> 
   <td>clientsecret</td> 
   <td>是</td> 
   <td> Workfront中为此自定义集成配置的客户端密钥。</td> 
  </tr> 
 </tbody> 
</table>

 

**响应**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名称</th> 
   <th>类型 </th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>access_token </td> 
   <td>字符串</td> 
   <td> <p>用于代表用户进行授权API调用的令牌。 这应该会终止，以防止未授权的API调用。</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token </td> 
   <td>字符串</td> 
   <td> <p>长效令牌，用于通过调用此API方法检索新的access_token。</p> </td> 
  </tr> 
  <tr> 
   <td>expires_in </td> 
   <td>长</td> 
   <td>  <p>（可选）access_token过期之前的时间（以秒为单位），通常为3,600。</p></td> 
  </tr> 
 </tbody> 
</table>

 

**示例**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```


**响应**

```
{
"access_token":"ad8af5ad5ads759", 
"refresh_token":"9a0h5d87d808ads", 
"expires_id":"3600" 
}
```

### 获取文件或文件夹的元数据

返回指定文件或文件夹的元数据。

**URL**

GET/metadata？id=[文档或文件夹ID]

**查询参数**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名称 </th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>id</td> 
   <td>  <p>文件或文件夹的ID，由webhook提供程序引用。 这与Workfront的文档ID不同。 要获取根目录的元数据，请使用值“/”。</p><p>注意：该ID的最大长度为255个字符。</p></td> 
  </tr> 
 </tbody> 
</table>

 

**响应**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名称 </th> 
   <th>类型 </th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title </td> 
   <td>字符串 </td> 
   <td>文档或文件夹的名称</td> 
  </tr> 
  <tr> 
   <td>种类 </td> 
   <td>字符串 </td> 
   <td>指定此项是文件还是文件夹（“文件”还是“文件夹”）</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>字符串 </td> 
   <td>文件或文件夹的id。</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>字符串 </td> 
   <td> <p>用户在浏览器窗口中查看文档所使用的URL路径。 URL可以由文档提供程序或本机外部存储提供程序托管。</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>字符串 </td> 
   <td> <p>用户在浏览器窗口中下载文档所使用的URL路径。 URL可以由文档提供程序或本机外部存储提供程序托管。</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>字符串 </td> 
   <td>文件的MIME类型。 (可选)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>字符串 </td> 
   <td>上次修改此文件的时间（格式为RFC 3339时间戳）</td> 
  </tr> 
  <tr> 
   <td>大小</td> 
   <td>长</td> 
   <td>  文件的大小（以字节为单位）。 (可选)</td> 
  </tr> 
  <tr> 
   <td>只读</td> 
   <td>布尔型</td> 
   <td>  <p> 指示此文件或文件夹对于经过身份验证的用户是否为只读的。(可选)</p><p> </p></td> 
  </tr> 
 </tbody> 
</table>

**示例：** `https://www.acme.com/api/metadata?id=12345`

**响应**

```
{
"title":"My Document", 
"kind":"file"
"id":"12345", 
"viewLink":"https://www.acme.com/viewDocument?id=12345", 
"downloadLink":"https://www.acme.com/downloadDocument?id=12345",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size": "32554694"
}
```

>[!NOTE]
>
>所有API调用中的错误处理都应保持一致。 有关详细信息，请参阅下面的“错误处理”部分。

### 获取文件夹中的项目列表

返回给定文件夹的文件和文件夹的元数据。

**URL**

GET/files

**查询参数**

| 名称  | 描述 |
|---|---|
| parentId  | 文件夹ID。 要获取根目录的元数据，请使用值“/”。 |

{style="table-layout:auto"}

文档Webhooks API当前不支持分页。

**响应**

包含文件和文件夹列表的JSON。 每个项的元数据与/metadata端点返回的元数据相同。

**示例：** `https://www.acme.com/api/files?parentId=123456`

**响应**

```
[
{
"title":"Folder A",
"kind":"folder",
"id":"2lj23lkj",
"viewLink":"https://www.acme.com/viewDocument?id=2lj23lkj",
"downloadLink":"https://www.acme.com/downloadDocument?id=2lj23lkj",
"mimeType":"",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"" 
},
{
"title":"My Document",
"kind":"file",
"id":"da8cj234"
"viewLink":"https://www.acme.com/viewDocument?id=da8cj234",
"downloadLink":"https://www.acme.com/downloadDocument?id=da8cj234",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"32554694"
},
]
```

### 执行搜索

返回搜索返回的文件和文件夹的元数据。 这可以作为全文搜索或常规数据库查询来实现。 当用户从外部文件浏览器执行搜索时，Workfront会调用/search端点。

**URL**

GET/search

**查询参数**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名称 </th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>查询</td> 
   <td>搜索词或短语。</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>（可选）从中执行搜索的文件夹ID。 注意：这是Workfront中未来功能的占位符。 目前，Workfront不传递此参数。 </p> </td> 
  </tr> 
  </tbody> 
</table>

文档Webhooks API当前不支持分页。

 

**响应**

JSON，其中包含与查询匹配的文件和文件夹的元数据列表。 构成“匹配”的内容由webhook提供程序决定。 理想情况下，应该进行全文搜索。 执行基于文件名的搜索也可正常工作。

**示例：** `https://www.acme.com/api/search?query=test-query`

**响应**

```
[
{ File/Folder Metadata },
{ File/Folder Metadata }
]
```

### 获取文档的内容

返回文档的原始字节

**URL**

GET/下载

**查询参数**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名称 </th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>id</p> </td> 
   <td> 文档ID</td> 
  </tr> 
 </tbody> 
</table>

 

**响应**

文档的原始字节。

**示例：** `https://www.acme.com/api/download?id=123456`

### 获取文档的缩略图

返回文档的原始缩略图字节。

**URL**

GET/thumbnail

**查询参数**

| 名称  | 描述 |
|---|---|
| id  | 文档ID |
| 大小  |  缩略图的宽度 |

{style="table-layout:auto"}

 

**响应**

原始缩略图字节。

**示例：** `https://www.acme.com/api/thumbnail?id=123456`

### 上传文件 — 第1部分，共2部分

将文件上传到文档存储提供程序是一个两步过程，需要两个单独的API端点。 Workfront通过调用/uploadInit开始上传过程。 此端点返回一个文档ID，然后在上传文档字节时将其传递到/upload。 根据基础文档存储系统，可能需要创建一个长度为零的文档，然后稍后更新该文档的内容。

添加到此规范版本1.1中的文档ID和文档版本ID可用于从Workfront中检索额外信息。 例如，如果文档管理系统需要有关文档的额外信息，webhook实施代码可以使用文档ID使用Workfront的RESTful API检索该信息。 好的做法是，这些信息可能来自文档上的自定义数据字段，并且包含任务、问题或项目。

**URL**

POST/uploadInit

**查询参数**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名称 </th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>parentId </td> 
   <td>由webhook提供程序引用的父文件夹ID。</td> 
  </tr> 
  <tr> 
   <td>文件名 </td> 
   <td>文档的名称</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>Workfront文档ID（1.1版中添加）</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>Workfront文档版本ID（在版本1.1中添加）</td> 
  </tr> 
 </tbody> 
</table>

 

**响应**

文件的元数据，由/metadata端点定义。

**示例：** `https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b`

**响应**

`[file_metadata]` 包含文档提供商使用的新文档ID。

### 上传文件 — 第2部分（共2部分）

将文档的字节上载到webhook提供程序。

**URL**

PUT/upload

**查询参数**

| 名称  | 描述 |
|---|---|
| id  |  刚刚创建的文档ID。 |


 

**请求正文**

文档的原始内容字节。

**响应**

```
{
"result": "success"
}
```

或

```
{
"result": "fail"
}
```

**示例：** `https://www.acme.com/api/upload?id=1234` *[更新流中包含的文档字节]*

**响应**

```
{
"result":"success"
}
```

### 获取有关服务的信息 

（发布日期 — 待定）返回有关该服务的信息，如特性和功能。 Workfront将使用此信息自定义Workfront中的用户界面。 例如，如果webhook实施包含一些自定义操作，则JSON应在JSON中列出这些操作。 随后，用户将能够从Workfront调用这些操作。

**URL**

GET/serviceInfo

查询参数

无. 此外，对此端点的调用不应需要身份验证。

**响应**

包含有关此服务的信息的JSON

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名称</th> 
   <th>类型 </th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion </td> 
   <td>字符串 </td> 
   <td>由此服务实现的webhook版本。 这是此规范顶部列出的版本号。</td> 
  </tr> 
  <tr> 
   <td>版本 </td> 
   <td>字符串 </td> 
   <td>此服务的内部版本号。 此数字由webhook服务提供商确定，仅用于提供信息。<br><br></td> 
  </tr> 
  <tr> 
   <td>发布者 </td> 
   <td>字符串 </td> 
   <td>提供webhook实施的公司的名称。</td> 
  </tr> 
  <tr> 
   <td>availableendpoints</td> 
   <td>字符串 </td> 
   <td>包含由此服务实现的API端点的列表。 这可用于确保Workfront中的用户界面反映webhook提供程序提供的功能。 列表中的每一项都必须包含端点的名称（如“search”）。</td> 
  </tr> 
  <tr> 
   <td>customactions </td> 
   <td>字符串</td> 
   <td>  <p>包含由此webhook实现的自定义操作的列表。 每个列表项包括名称和显示名称。 显示名称将显示在Workfront的“文档操作”下拉列表中。 单击下拉列表中的项目将通过调用/customAction端点在webhook中调用操作。</p></td> 
  </tr> 
 </tbody> 
</table>

**示例：** https://www.acme.com/api/serviceInfo

**返回**

```
{
"webhook version": "1.2", "version": "1.0", "publisher": "Acme, LLC", "availableEndpoints": ["files", "metadata", "search", "download"

"thumbnail", "uploadInit", "upload" ], "customActions" [
{
"name": "archive", "displayName": "Archive" }, {

"name": "doSomethingElse", "displayName": "Do Something" }, ] }
```

### 创建文件夹

（在1.2版中添加）在给定目录中创建文件夹。
URL

POST/createFolder

**查询参数**

| 名称  | 描述 |
|---|---|
| parentId  | 应在其中创建文件夹的文件夹ID |
| name  | 新文件夹的名称 |

{style="table-layout:auto"}

 

**响应**

新创建文件夹的元数据，如/metadata端点定义。

**示例：** `POST https://www.acme.com/api/createFolder`

```
-------------------------------

parentId=1234

name=New Folder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

返回

```
{"title":"New Folder", 
 "kind":"folder""id":"5678",
 "viewLink":"",
 "downloadLink":"",
 "mimeType":"",
 "dateModified":"2014­06­05T17:39:45.251Z" 
 "size": "" 
 }
```

### 删除文档或文件夹

（发布日期 — 待定）删除外部系统中具有给定ID的文档或文件夹。 删除文件夹也会删除其内容。

URL

PUT/delete

**查询参数**

| 名称  | 描述 |
|---|---|
| documentId  | 要删除的文档ID |
| folderId  |  要删除的文件夹ID |

{style="table-layout:auto"}

响应JSON字符串，指示成功或失败，如下面的错误处理部分中所述。

**示例：** PUThttps://www.acme.com/api/delete id=1234

返回

```
{
"status": "success" 
}
```

返回

```
{
"status": "failure", "error": "File not found"
}
```


### 重命名文档或文件夹

（发布日期 — 待定）在外部系统中使用给定ID重命名文档或文件夹。

URL

PUT/rename

**查询参数**

| 名称  | 描述 |
|---|---|
| id | 要重命名的文档或文件夹ID |
| name  | 文档或文件夹的新名称 |

{style="table-layout:auto"}

 

个回应

指示成功或失败的JSON字符串，如下面的错误处理部分中所述。

**示例:**

`PUT https://www.acme.com/api/rename`

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

```
{
"status": "success" 
}returns
{
"status": "failure", error: "Folder cannot be renamed because a folder with that name already exists." 
}
```

### 执行自定义操作

（发布日期 — 待定）此端点将允许Workfront用户（或可能是自动工作流事件）在外部系统中执行操作。 /customAction端点接受“name”参数，该参数允许webhook提供程序实现多个自定义操作。

webhook提供程序通过在customActions下的/serviceInfo响应中包含操作来向Workfront注册自定义操作。 在设置>文档>自定义集成下设置或刷新webhook提供程序时，Workfront会加载此列表。\
![](assets/mceclip0-350x262.png)

用户可以通过选择“文档操作”下的部分来触发自定义操作\
![](assets/mceclip1-350x95.png)

**URL**

GET/customAction

**查询参数**

<table style="table-layout:auto">
 <col>
 <col>
 <thead>
  <tr>
   <th>名称 </th>
   <th>描述</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><p>name</p></td>
   <td><p>指定要执行的操作类型的标识符。 此值对应于/serviceInfo终结点返回的customAction值之一。</p></td>
  </tr>
  <tr>
   <td>documentId </td>
   <td>正在对其执行操作的Workfront文档ID。</td>
  </tr>
  <tr>
   <td>documentVersionId </td>
   <td> 正在对其执行操作的Workfront文档版本ID。</td>
  </tr>
 </tbody>
</table>

 

**响应**

指示成功或失败的JSON字符串，如下面的错误处理部分中所述。 出现故障时（即状态=“故障”），Workfront将向用户显示提供的错误消息。

**示例：** https://sample.com/webhooks/customName?name=archive&amp;documentId=5502082c003a4f30 ddec2fb2b739cb7c&amp;documentVersionId=54b598a700e2342d6971597a5df1a8d3

响应

```
{
"status": "success" 
}
```


## 错误处理

处理API请求时可能会出现问题。 应当在所有API端点中以一致的方式处理此问题。 发生错误时，webhook提供程序将执行以下操作：

* 在响应标头中包含错误代码。 错误代码包括：

   * 403 — 禁止访问。 指示请求令牌缺失或无效，或者与令牌关联的凭据无权访问指定的资源。 对于基于OAuth的webhook提供程序，Workfront将尝试检索新的访问令牌。
   * 404 — 未找到。 指示指定的文件或文件夹不存在。
   * 500 — 内部服务器错误。 任何其他类型的错误。

* 使用以下格式描述响应正文中的错误：


```
{
"status": "error"
"error": "Sample error message" 
}
```


## 测试

要验证文档webhook实施是否正常工作，请运行以下测试。 这些是手动测试，通过Workfront Web界面间接点击webhook实施的端点。

### 先决条件

要运行这些测试，您需要满足以下条件：

* 启用了高级文档管理(ADM)的Workfront帐户
* 此帐户中拥有系统管理员权限的Workfront用户
* Workfront可以访问其HTTP端点的文档Webhook实例

这些测试还假定您已经在Workfront中的“设置”>“文档”>“自定义集成”下注册了Document Webhook实例。

### 测试1：为用户预配Document Webhook服务

测试基于OAuth的Webhook提供程序的身份验证URL和令牌端点URL。

1. 在Workfront中，单击顶部导航栏中的“文档”链接，转到“文档”主页面。
1. 单击添加文档下拉列表，然后在添加服务下选择您的文档Webhook服务。
1. （仅限OAuth服务）完成上一步后，您将在弹出窗口中看到服务的OAuth2身份验证页面加载。 （注意：系统可能会提示您先登录服务。） 在身份验证页面中，通过单击信任或允许按钮授予Workfront对用户帐户访问权限。
1. 验证您的服务是否已添加到添加文档下拉列表中。 如果您最初没有看到该页面，请尝试刷新浏览器。

### 测试2：将文档链接到Workfront测试以下端点： /files、/metadata

1. 在Workfront中，单击顶部导航栏中的“文档”链接，转到“文档”主页面。
1. 在“添加文档”下选择文档Webhook服务。
1. 在该模式中，导航浏览文件夹结构。
1. 验证您是否能够正确导航文件夹结构。
1. 选择文档并将其链接到Workfront

### 测试3：导航到内容管理系统中的文档

测试以下端点： /metadata （尤其是viewLink）

1. 将文档链接到Workfront
1. 选择文档并单击“打开”链接。
1. 验证文档是否在新选项卡中打开。

### 测试4：导航到内容管理系统中的文档（登录）

测试以下端点： /metadata （尤其是viewLink）

1. 确保您已从内容管理系统注销。
1. 将文档链接到Workfront。
1. 选择文档并单击“打开”链接。
1. 验证内容管理系统的登录屏幕是否在新选项卡中加载。
1. 登录并验证您是否已转到文档

### 测试5：从内容管理系统下载文档

测试以下端点： /metadata（尤其是downloadLink）

1. 将文档链接到Workfront。
1. 选择文档并单击“下载”链接。
1. 验证下载是否开始。

### 测试6：搜索内容

测试以下端点： /search

1. 在Workfront中，单击顶部导航栏中的“文档”链接，转到“文档”主页面。
1. 在“添加文档”下选择文档Webhook服务。
1. 在该模式窗口中，执行搜索。
1. 验证搜索结果是否正确。

### 测试7：将文档从Workfront发送到内容管理系统

测试以下端点： /files、/uploadInit、/upload

1. 在Workfront中，单击顶部导航栏中的“文档”链接，转到“文档”主页面。
1. 将文档从计算机上传到Workfront
1. 转到文档详情页面
1. 从“文档操作”下拉列表中，选择“发送到……”下的Document Webhook服务
1. 转到所需的目标文件夹，然后单击保存按钮。
1. 验证文档是否已上传到内容管理系统中的正确位置。

### 测试8：在Workfront中查看缩略图

测试以下端点： /thumbnail

1. 将文档链接到Workfront。
1. 在列表中选择文档。
1. 验证缩略图是否显示在右侧面板中。

### 测试9：获取内容字节

测试以下端点： /download

1. 将文档链接到Workfront。
1. 转到文档详情页面。
1. 通过选择“文档操作”>“发送到……”>“Workfront”，将文档发送到Workfront。 这将在Workfront中创建一个新文档版本。
1. 通过单击下载链接，从Workfront下载文档。

### 测试10：刷新访问令牌（仅限OAuth2 Webhook提供程序）

测试以下端点：令牌端点URL

1. 为用户预配Document Webhook服务
1. 通过1 )等待用户访问令牌超时或2)在外部系统中手动使其失效，来使其失效。
1. 在Workfront中刷新访问令牌。 例如，您可以将文档链接到Workfront中来执行此操作。 如果您能够导航到文档并进行链接，则您将知道访问令牌已成功刷新。

>[!NOTE]
>
>目前，发送至……不可用于链接的文档。 Workfront将添加此参数。 您可以通过使用REST客户端(例如Postman)手动点击端点来测试/download端点。 或者，可以通过生成数字验证来测试/download端点。 要启用数字校对，请联系Workfront。

## 版本

* 版本1.0（发行日期：2015年5月）

   * 初始规范

* 版本1.1（发行日期 — 2015年6月）

   * 更新了/uploadInit — 添加了documentId和documentVersionId

* 版本1.2（发行日期：2015年10月）

   * 添加了/createFolder

