---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: http-modules
title: HTTP &gt;发出基本授权请求模块
description: Adobe Workfront Fusion除了需要Adobe Workfront许可证之外，还需要Adobe Workfront Fusion许可证。
author: Becky
feature: Workfront Fusion
exl-id: df8b53de-1af2-4026-b7dd-ff5133b4aac2
source-git-commit: 58db2129dd764d24b0a681735c2405be402d8b43
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 0%

---

# [!UICONTROL HTTP] >[!UICONTROL 发出基本授权请求] 模块

此 [!DNL Adobe Workfront Fusion] 模块允许您配置具有HTTP基本授权的HTTP请求，并将其提交到服务器。 接收的HTTP响应随后包含在输出包中。

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!UICONTROL HTTP] >[!UICONTROL 发出基本授权请求] 模块配置

当您配置 [!UICONTROL HTTP] >[!UICONTROL 发出基本授权请求] 模块， [!DNL Adobe Workfront Fusion] 显示下面列出的字段。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL凭据]</td> 
   <td> <p>选择包含基本身份验证凭据的密钥，或单击 <strong>[!UICONTROL Add]</strong> 将凭据添加到新密钥。 </p> <p>注意：您可以添加更多凭据，以便轻松地在每个连接之间切换。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL评估所有状态为错误（2xx和3xx除外）] </td> 
   <td> <p>使用此选项设置错误处理。</p> <p>有关更多信息，请参阅 <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">在中处理错误 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>输入要向发送请求的URL，如API端点、网站等。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL方法]</p> </td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头] </td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。例如， <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询字符串]</td> 
   <td> <p> 输入所需的查询键值对。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Body type]</p> </td> 
   <td> <p>HTTP Body是在HTTP事务消息中发送的数据字节（如果有任何要使用的数据字节，则紧靠标头后）。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>即使在开发人员文档未指定要发送的数据的情况下，原始主体类型通常也适用于大多数HTTP主体请求。</p> <p>在[!UICONTROL内容类型]字段中指定解析数据的形式。</p> <p>尽管选择了内容类型，数据仍以开发人员文档规定或要求的任何格式输入。</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>此正文类型是使用 <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>对于 <code>[!UICONTROL application/x-www-form-urlencoded]</code>，则发送到服务器的HTTP消息正文本质上是一个查询字符串。 键和值以键值对进行编码，键值对之间用 <code>&amp;</code> 和 <code>=</code> 键和值之间。 </p> <p>对于二进制数据，请使用 <code>multipart/form-data</code> 中。</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>示例: </b></span></span> 
       <p>生成的HTTP请求格式示例：</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>[!UICONTROL Multipart/form-data]是用于发送文件和数据的HTTP多部分请求。 它通常用于将文件上传到服务器。</p> <p>添加要在请求中发送的字段。 每个字段必须包含键值对。</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Text]</strong> </p> <p>输入要在请求正文中发送的键和值。</p> </li> 
       <li> <p><strong>[!UICONTROL文件]</strong> </p> <p>输入键，并指定要在请求正文中发送的源文件。</p> <p>映射要从上一个模块上传的文件(例如[!UICONTROL HTTP] &gt;[!UICONTROL Get a File]或[!UICONTROL Google Drive] &gt;[!UICONTROL Download a File)]，或手动输入文件名和文件数据。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Parse响应]</p> </td> 
   <td> <p>启用此选项可自动解析响应并转换JSON和XML响应，这样您就无需使用[!UICONTROL JSON] &gt; [!UICONTROL Parse JSON]或[!UICONTROL XML] &gt; [!UICONTROL Parse XML]模块。</p> <p>在使用解析后的JSON或XML内容之前，请手动运行该模块一次，以便该模块能够识别响应内容，并允许您在后续模块中映射该内容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL超时] </td> 
   <td> <p>以秒为单位指定请求超时(1-300)。 默认为40秒。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL与其他HTTP模块共享Cookie]</td> 
   <td> <p> 启用此选项，可将服务器中的Cookie与方案中的所有HTTP模块共享。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL自签名证书]</td> 
   <td> <p> 如果您希望使用自签名证书的TLS，请上传您的证书。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拒绝使用未验证（自签名）证书的连接] </td> 
   <td> <p>启用此选项可拒绝使用未验证的TLS证书的连接。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL遵循重定向]</td> 
   <td> <p> 启用此选项，可通过3xx响应来遵循URL重定向。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL按照所有重定向] </td> 
   <td> <p>启用此选项可使用所有响应代码遵循URL重定向。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL禁用与数组相同的多个查询字符串键的序列化]</p> </td> 
   <td> <p>默认情况下， [!DNL Workfront Fusion] 处理与数组相同的URL查询字符串参数键的多个值。 例如， <code>www.test.com?foo=bar&amp;foo=baz</code> 将转换为 <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. 激活此选项可禁用此功能。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL请求压缩内容]</td> 
   <td> <p> 启用此选项可请求网站的压缩版本。</p> <p>添加 <code>[!UICONTROL Accept-Encoding]</code> 请求压缩内容的标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL使用互相TLS]</td> 
   <td> <p>启用此选项可在HTTP请求中使用相互TLS。</p> <p>有关相互TLS的更多信息，请参阅 <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">在的HTTP模块中使用相互TLS  </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
