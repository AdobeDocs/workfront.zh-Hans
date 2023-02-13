---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: AWS S3模块
description: 的 [!DNL Adobe Workfront Fusion AWS] S3模块允许您对S3存储段执行操作。
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1381'
ht-degree: 0%

---

# AWS S3模块

的 [!DNL Adobe Workfront Fusion AWS] S3模块允许您对S3存储段执行操作。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!UICONTROL AWS S3] 模块，您必须具有 [!DNL Amazon Web Service] 帐户。

## 连接 [!DNL AWS] to [!DNL Workfront Fusion] {#connect-aws-to-workfront-fusion}

连接 [!DNL AWS S3] to [!DNL Workfront Fusion] 必须连接 [!DNL AWS] 帐户 [!DNL Workfront Fusion]. 为此，您首先需要在 [!DNL AWS] [!UICONTROL IAM].

1. 登录到 [!DNL AWS] [!UICONTROL IAM] 帐户。
1. 导航到 **[!UICONTROL 身份和访问管理]** > **[!UICONTROL 访问管理]** > **[!UICONTROL 用户]**.

1. 单击 **[!UICONTROL 添加用户]**.
1. 输入新用户的名称并选择 **[!UICONTROL 程序化访问]** 选项 [!UICONTROL 访问类型] 中。
1. 单击 **[!UICONTROL 直接附加现有策略]**，然后搜索 **[!UICONTROL AmazonS3FullAccess]** 中。 出现时单击它，然后单击 **[!UICONTROL 下一个]**.

1. 继续浏览其他对话框屏幕，然后单击 **[!UICONTROL 创建用户]**.
1. 复制提供的 **[!UICONTROL 访问密钥ID]** 和 **[!UICONTROL 密钥访问密钥]**.

1. 转到 [!DNL Workfront Fusion] 打开 [!DNL AWS S3] 模块 **[!UICONTROL 创建连接]** 对话框。
1. 输入 [!UICONTROL 访问密钥ID] 和 [!UICONTROL 密钥访问密钥] 从步骤7到相应的字段并单击 **[!UICONTROL 继续]** 建立连接。

连接已建立。 您可以继续设置模块。

## [!DNL AWS S3] 模块及其字段

配置 [!DNL AWS S3] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL AWS S3] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [操作](#actions)
* [搜索](#searches)

### 操作

* [[!UICONTROL 创建存储段]](#create-bucket)
* [[!UICONTROL 获取文件]](#get-file)
* [[!UICONTROL 上传文件]](#upload-file)
* [[!UICONTROL 进行API调用]](#make-an-api-call)

#### [!UICONTROL 创建存储段]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL AWS] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">连接 [!DNL AWS] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL名称] </td> 
   <td> <p>输入新存储段的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL区域] </td> 
   <td> <p>选择您的区域端点。 有关详细信息，请参阅 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">区域端点</a> (在AWS文档中)。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件]

从存储段下载文件。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL AWS] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">连接 [!DNL AWS] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL区域] </td> 
   <td> <p>选择您的区域端点。 有关详细信息，请参阅 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">区域端点</a> 在 [!DNL AWS] 文档。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存储段] </td> 
   <td> <p>选择要从中下载文件的存储段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL路径]</p> </td> 
   <td> <p>输入文件的路径。 示例: <code>/photos/2019/February/image023.jpg</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上传文件]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL AWS] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">连接 [!DNL AWS] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL区域] </td> 
   <td> <p>选择您的区域端点。 有关详细信息，请参阅 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">区域端点</a> 在 [!DNL AWS] 文档。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL文件夹]（可选） </p> </td> 
   <td> <p>指定要将文件上传到的目标文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL标头]（可选）</p> </td> 
   <td> <p> 插入请求标头。 可在 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3] 文档 — [!UICONTROLPUT]对象</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 进行API调用]

详细讨论 [!DNL Amazon S3] API，请参阅 [[!DNL Amazon S3] [!UICONTROL REST] API简介](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL AWS] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">连接 [!DNL AWS] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL区域] </td> 
   <td> <p>选择您的区域端点。 有关详细信息，请参阅 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">区域端点</a> 在 [!DNL AWS] 文档。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>URL输入主机URL。 路径必须相对于<code> https://s3.&lt;selected-region>.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的[!UICONTROL HTTP]请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的[!UICONTROL HTTP]请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL标头]</td> 
   <td> <p>添加请求标头。 您可以使用以下常用请求标头。 有关更多请求标头，请参阅 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3] API文档</a>.</p> <p>[!DNL Workfront Fusion] 自动添加授权标头。</p> 
    <table style="table-layout:auto">
     <col> 
     <col> 
     <thead> 
      <tr> 
       <th>标题名称</th> 
       <th> <p> 描述</p> </th> 
      </tr> 
     </thead> 
     <tbody> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Length]</p> </td> 
       <td> <p>根据RFC 2616，消息的长度（不含标头）。 [!UICONTROLPUT]和加载XML的操作（如日志记录和ACL）需要此标头。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Type]</p> </td> 
       <td> <p>资源的内容类型（如果请求内容位于正文中）。 示例: <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-MD5]</p> </td> 
       <td> <p>base64根据RFC 1864对消息的128位MD5摘要（不包含标头）进行了编码。 此标头可用作消息完整性检查，以验证数据是否与最初发送的数据相同。 尽管它是可选的，但我们建议使用[!UICONTROL Content-MD5]机制作为端到端完整性检查。 有关[!UICONTROL REST]请求身份验证的更多信息，请转到 <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">[!UICONTROL REST]身份验证</a> 在 <i>[!DNL Amazon] 《简单存储服务开发人员指南》</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL日期]</p> </td> 
       <td> <p>根据请求者的当前日期和时间。 示例: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. 当您指定 <code>Authorization </code>标题时，必须指定 <code>x-amz-date</code> 或 <code>Date </code>标题。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL预期]</p> </td> 
       <td> <p>当您的应用程序使用[!UICONTROL 100-continue]时，它在收到确认之前不会发送请求正文。 如果根据标头拒绝消息，则不会发送消息正文。 仅当您发送正文时，才能使用此标头。</p> <p>有效值：[!UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL主机]</p> </td> 
       <td> <p>对于路径样式请求，值为 <code>s3.amazonaws.com</code>. 对于虚拟样式请求，其值为 <code>BucketName.s3.amazonaws.com</code>. 有关更多信息，请参阅 <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">虚拟托管</a> 在 <i>[!DNL Amazon] 《简单存储服务开发人员指南》</i>.</p> <p>HTTP 1.1需要此标头（大多数工具包会自动添加此标头）；对于HTTP/1.0请求而言，它是可选项。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>使用签名版本4验证请求时，此标头会提供请求有效负载的哈希。 在以块为单位上传对象时，将值设置为 <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> 表示签名仅覆盖标头且没有有效负载。 有关更多信息，请参阅 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">授权标头的签名计算：以多个块传输有效负载（分块上传）([!DNL AWS] 签名版本4)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-date]</p> </td> 
       <td> <p>根据请求者的当前日期和时间。 示例: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. 当您指定 <code>Authorization </code>标题时，必须指定 <code>x-amz-date</code> 或 <code>Date </code>标题。 如果同时指定这两个值，则为 <code>x-amz-date</code> 标头优先。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>此标头可用于以下情况：</p> 
        <ul> 
         <li>为 [!DNL Amazon DevPay] 操作。 使用 [!DNL Amazon DevPay] 需要两个 <code>x-amz-security-token</code> 标题：一个用于产品令牌，一个用于用户令牌。 When [!DNL Amazon S3] 接收经验证的请求，其将计算的签名与提供的签名进行比较。 用于计算签名的格式不正确的多值标头可能会导致身份验证问题。</li> 
         <li>使用临时安全凭据时提供安全令牌。 在使用您从IAM获得的临时安全凭据发出请求时，必须使用此标头提供安全令牌。 要了解有关临时安全凭据的更多信息，请转到发出请求。</li> 
        </ul> <p>对于使用 [!DNL Amazon DevPay] 和使用临时安全凭据进行签名的请求。</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL查询字符串]</td> 
   <td> <p>添加所需的查询字符串，如参数或表单字段。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。</p> <p>注释:   <p>使用条件语句时，例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜索

* [[!UICONTROL 列表文件]](#list-files)
* [[!UICONTROL 列表文件夹]](#list-folders)

#### [!UICONTROL 列表文件]

从指定位置返回文件列表。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL AWS] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">连接 [!DNL AWS] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL区域] </td> 
   <td> <p>选择您的区域端点。 有关详细信息，请参阅 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">区域端点</a> 在 [!DNL AWS] 文档。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存储段] </td> 
   <td> <p>选择 [!DNL Amazon S3] 存储段，以搜索文件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL前缀]（可选）</p> </td> 
   <td> <p> 在中查找文件的文件夹路径，例如 <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列表文件夹]

从指定位置返回文件夹列表。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL AWS] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">连接 [!DNL AWS] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL区域] </td> 
   <td> <p>选择您的区域端点。 有关详细信息，请参阅 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">区域端点</a> (在AWS文档中)。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存储段] </td> 
   <td> <p>选择 [!DNL Amazon S3] 存储段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL前缀]（可选）</p> </td> 
   <td> <p> 在中查找文件夹的文件夹路径，例如 <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
