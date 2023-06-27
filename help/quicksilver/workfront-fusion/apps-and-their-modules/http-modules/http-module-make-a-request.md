---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: http-modules
title: HTTP &gt；生成请求模块
description: Adobe Workfront Fusion HTTP &gt；发出请求模块是一个通用模块，通过该模块可以配置HTTP请求并将其提交到服务器。 接收的HTTP响应随后包含在输出包中。
author: Becky
feature: Workfront Fusion
exl-id: 7857c395-ce84-480e-8fa2-065035ac5b95
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 0%

---

# [!UICONTROL HTTP] >[!UICONTROL 提出请求] 模块

>[!NOTE]
>
>Adobe Workfront Fusion需要 [!DNL Adobe Workfront Fusion] 除了许可证外， [!DNL Adobe Workfront] 许可证。

此 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL 创建请求模块] 是一个通用模块，用于配置HTTP请求并将其提交到服务器。 接收的HTTP响应随后包含在输出包中。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td>
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [Adobe Workfront Fusion许可证](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!UICONTROL HTTP] >[!UICONTROL 提出请求] 模块配置

当您配置 [!UICONTROL HTTP] >[!UICONTROL 提出请求] 模块， [!DNL Adobe Workfront Fusion] 显示下面列出的字段。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL将所有状态计算为错误（2xx和3xx除外）] </td> 
   <td> <p>使用此选项可设置错误处理。</p> <p>有关更多信息，请参阅 <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">中的错误处理 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL] </td> 
   <td> <p>输入要向其发送请求的URL，如API端点、网站等。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标头] </td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。例如， <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p> 输入所需的查询键值对。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL正文类型]</p> </td> 
   <td> <p>HTTP正文是在HTTP事务消息中传输的数据字节，紧跟在标头之后（如果有任何要使用的标头）。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL Raw]</strong> </p> <p>原始正文类型通常适用于大多数HTTP正文请求，即使在开发人员文档未指定要发送的数据的情况下也是如此。</p> <p>在[！UICONTROL内容类型]字段中指定解析数据的形式。</p> <p>尽管选择了内容类型，但还是会以开发人员文档规定或要求的任何格式输入数据。</p> </li> 
     <li> <p><strong>[！UICONTROL应用程序/x-www-form-urlencoded]</strong> </p> <p>此正文类型使用对[！UICONTROL]数据的POST <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>对象 <code>application/x-www-form-urlencoded</code>，发送到服务器的HTTP消息正文本质上是一个查询字符串。 键和值在键值对中进行编码，分隔方式为 <code>&amp;</code> 和 <code>=</code> 键和值之间。 </p> <p>对于二进制数据，使用 <code>[!UICONTROL multipart/form-data]</code> 而是。</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>示例: </b></span></span> 
       <p>生成的HTTP请求格式示例：</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[！UICONTROL Multipart/form-data]</strong> </p> <p>[！UICONTROL Multipart/form-data]是用于发送文件和数据的HTTP多部分请求。 它通常用于将文件上传到服务器。</p> <p>添加要在请求中发送的字段。 每个字段都必须包含键值对。</p> 
      <ul> 
       <li> <p><strong>[！UICONTROL文本]</strong> </p> <p>输入要在请求正文中发送的键和值。</p> </li> 
       <li> <p><strong>[！UICONTROL文件]</strong> </p> <p>输入密钥，并在请求正文中指定要发送的源文件。</p> <p>映射要从上一个模块上传的文件(如[！UICONTROL HTTP] &gt;[！UICONTROL Get a File]或[！UICONTROL Google Drive] &gt;[！UICONTROL Download a File)]，或手动输入文件名和文件数据。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL解析响应]</p> </td> 
   <td> <p>启用此选项可自动解析响应并转换JSON和XML响应，因此您无需使用[！UICONTROL JSON] &gt; [！UICONTROL Parse JSON]或[！UICONTROL XML] &gt; [！UICONTROL Parse XML]模块。</p> <p>在使用解析的JSON或XML内容之前，请手动运行一次模块，以便模块可以识别响应内容并允许您将其映射到后续模块。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL用户名]</p> </td> 
   <td> <p> 如果要使用基本授权发送请求，请输入用户名。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL密码] </td> 
   <td> <p>如果要使用基本授权发送请求，请输入密码。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL超时] </td> 
   <td> <p>以秒为单位指定请求超时(1-300)。 默认值为40秒。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL与其他HTTP模块共享Cookie]</td> 
   <td> <p> 启用此选项可将服务器中的Cookie与场景中的所有HTTP模块共享。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL自签名证书]</td> 
   <td> <p> 如果要使用自签名证书的TLS，请上传证书。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL拒绝使用未验证（自签名）证书的连接] </td> 
   <td> <p>启用此选项可拒绝使用未经验证的TLS证书的连接。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL遵循重定向]</td> 
   <td> <p> 启用此选项可在URL重定向之后显示3xx响应。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL遵循所有重定向] </td> 
   <td> <p>启用此选项可在URL重定向之后使用所有响应代码。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL禁用将多个相同的查询字符串键序列化为数组]</p> </td> 
   <td> <p>默认情况下， [!DNL Workfront Fusion] 处理作为数组的同一URL查询字符串参数键的多个值。 例如， <code>www.test.com?foo=bar&amp;foo=baz</code> 将转换为 <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. 激活此选项可禁用此功能。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL请求压缩内容]</td> 
   <td> <p> 启用此选项可请求网站的压缩版本。</p> <p>添加 <code>[!UICONTROL Accept-Encoding]</code> 标头以请求压缩的内容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL使用双向TLS]</td> 
   <td> <p>启用此选项可在HTTP请求中使用双向TLS。</p> <p>有关双向TLS的详细信息，请参见 <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">在中使用HTTP模块中的双向TLS [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**示例：** 此示例说明如何设置模块以提交 [!UICONTROL POST] 包含JSON有效负载的请求：
>
>![](assets/make-a-request-example-350x522.png)

>[!NOTE]
>
>为了确保您的 [!UICONTROL JSON] 有效，您可以使用以下可用的在线服务之一： [https://jsonlint.com/](https://jsonlint.com/). 您还可以使用 [!UICONTROL JSON] >[!UICONTROL 创建JSON模块] 以动态创建JSON并完成所有必要的转义。
>
>将JSON片段与表达式和项直接混合 [!UICONTROL 请求内容] 不建议使用字段，因为它可能会导致无效的JSON。
