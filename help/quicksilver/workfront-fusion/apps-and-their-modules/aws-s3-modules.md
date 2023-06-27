---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: AWS S3模块
description: 此 [!DNL Adobe Workfront Fusion AWS] S3模块允许您对S3存储桶执行操作。
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 1%

---

# AWS S3模块

此 [!DNL Adobe Workfront Fusion AWS] S3模块允许您对S3存储桶执行操作。

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

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!UICONTROL AWS S3] 模块，您必须拥有 [!DNL Amazon Web Service] 帐户。

## Connect [!DNL AWS] 到 [!DNL Workfront Fusion] {#connect-aws-to-workfront-fusion}

连接 [!DNL AWS S3] 到 [!DNL Workfront Fusion] 您必须连接 [!DNL AWS] 目标帐户 [!DNL Workfront Fusion]. 为此，您首先需要在中创建API用户 [!DNL AWS] [!UICONTROL IAM].

1. 登录到您的 [!DNL AWS] [!UICONTROL IAM] 帐户。
1. 导航到 **[!UICONTROL 身份和访问管理]** > **[!UICONTROL 访问管理]** > **[!UICONTROL 用户]**.

1. 单击 **[!UICONTROL 添加用户]**.
1. 输入新用户的名称，然后选择 **[!UICONTROL 程序化访问]** 中的选项 [!UICONTROL 访问类型] 部分。
1. 单击 **[!UICONTROL 直接附加现有策略]**，然后搜索 **[!UICONTROL AmazonS3FullAccess]** 在搜索栏中。 出现时单击它，然后单击 **[!UICONTROL 下一个]**.

1. 继续浏览其他对话框屏幕，然后单击 **[!UICONTROL 创建用户]**.
1. 复制提供的 **[!UICONTROL 访问密钥ID]** 和 **[!UICONTROL 访问密钥]**.

1. 转到 [!DNL Workfront Fusion] 然后打开 [!DNL AWS S3] 模块的 **[!UICONTROL 创建连接]** 对话框。
1. 输入 [!UICONTROL 访问密钥ID] 和 [!UICONTROL 访问密钥] 步骤7至相应的字段，然后单击 **[!UICONTROL 继续]** 以建立连接。

已建立连接。 您可以继续设置模块。

## [!DNL AWS S3] 模块及其字段

配置时 [!DNL AWS S3] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL AWS S3] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [操作](#actions)
* [搜索](#searches)

### 操作

* [[!UICONTROL 创建分段]](#create-bucket)
* [[!UICONTROL 获取文件]](#get-file)
* [[!UICONTROL 上传文件]](#upload-file)
* [[!UICONTROL 进行API调用]](#make-an-api-call)

#### [!UICONTROL 创建分段]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL AWS] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名称] </td> 
   <td> <p>输入新存储段的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL区域] </td> 
   <td> <p>选择您的区域端点。 欲了解更多信息，请参见 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">区域端点</a> 在AWS文档中。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件]

从存储桶下载文件。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL AWS] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL区域] </td> 
   <td> <p>选择您的区域端点。 欲了解更多信息，请参见 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">区域端点</a> 在 [!DNL AWS] 文档。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Bucket] </td> 
   <td> <p>选择要从中下载文件的存储桶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL路径]</p> </td> 
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
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL AWS] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL区域] </td> 
   <td> <p>选择您的区域端点。 欲了解更多信息，请参见 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">区域端点</a> 在 [!DNL AWS] 文档。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL文件夹]（可选） </p> </td> 
   <td> <p>指定要将文件上传到的目标文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择一个源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Headers]（可选）</p> </td> 
   <td> <p> 插入请求标头。 可用的标头可在以下位置找到： <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3] 文档 — [！UICONTROLPUT]对象</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 进行API调用]

欲详细了解 [!DNL Amazon S3] API，请参见 [[!DNL Amazon S3] [!UICONTROL REST] API简介](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL AWS] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL区域] </td> 
   <td> <p>选择您的区域端点。 欲了解更多信息，请参见 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">区域端点</a> 在 [!DNL AWS] 文档。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL URL]</td> 
   <td> <p>URL输入主机URL。 路径必须相对于<code> https://s3.&lt;selected-region>.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的[！UICONTROL HTTP]请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的[！UICONTROL HTTP]请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL标头]</td> 
   <td> <p>添加请求标头。 您可以使用以下常用请求标头。 有关更多请求标头，请参阅 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3] API文档</a>.</p> <p>[!DNL Workfront Fusion] 自动添加授权标头。</p> 
    <table style="table-layout:auto">
     <col> 
     <col> 
     <thead> 
      <tr> 
       <th>标头名称</th> 
       <th> <p> 描述</p> </th> 
      </tr> 
     </thead> 
     <tbody> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL Content-Length]</p> </td> 
       <td> <p>根据RFC 2616的消息长度（不带标头）。 加载XML的[！UICONTROLPUT]和操作（如日志记录和ACL）需要此标头。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL Content-Type]</p> </td> 
       <td> <p>资源的内容类型（如果请求内容位于正文中）。 示例: <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL Content-MD5]</p> </td> 
       <td> <p>根据RFC 1864，base64编码了消息的128位MD5摘要（没有标头）。 此标头可用作消息完整性检查，以验证数据是否与最初发送的数据相同。 尽管它是可选的，但我们建议使用[！UICONTROL Content-MD5]机制作为端到端完整性检查。 有关[！UICONTROL REST]请求身份验证的详细信息，请转到 <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">[！UICONTROL REST]身份验证</a> 在 <i>[!DNL Amazon] Simple Storage Service开发人员指南</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL日期]</p> </td> 
       <td> <p>根据请求者的当前日期和时间。 示例: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. 当您指定 <code>Authorization </code>标头，您必须指定 <code>x-amz-date</code> 或 <code>Date </code>标头。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL Expect]</p> </td> 
       <td> <p>当您的应用程序使用[！UICONTROL 100-continue]时，它会在收到确认后才发送请求正文。 如果根据标头拒绝消息，则不会发送消息正文。 仅当您发送正文时，才能使用此标头。</p> <p>有效值： [！UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL主机]</p> </td> 
       <td> <p>对于路径样式请求，值为 <code>s3.amazonaws.com</code>. 对于虚拟样式请求，值为 <code>BucketName.s3.amazonaws.com</code>. 有关更多信息，请参阅 <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">虚拟托管</a> 在 <i>[!DNL Amazon] Simple Storage Service开发人员指南</i>.</p> <p>HTTP 1.1需要此标头（大多数工具包会自动添加此标头）；HTTP/1.0请求则可选。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>使用签名版本4验证请求时，此标头提供请求有效负载的哈希。 以块形式上传对象时，将该值设置为 <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> 以指示签名仅涵盖标头，并且没有任何有效负载。 有关更多信息，请参阅 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">授权标头的签名计算：在多个块中传输有效负载（分块上传）([!DNL AWS] 签名版本4)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL x-amz-date]</p> </td> 
       <td> <p>根据请求者的当前日期和时间。 示例: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. 当您指定 <code>Authorization </code>标头，您必须指定 <code>x-amz-date</code> 或 <code>Date </code>标头。 如果同时指定两者，则为指定的值 <code>x-amz-date</code> 标题优先。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[！UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>此标头可用于以下方案：</p> 
        <ul> 
         <li>为提供安全令牌 [!DNL Amazon DevPay] 操作。 使用的每个请求 [!DNL Amazon DevPay] 需要两个 <code>x-amz-security-token</code> 标头：一个用于产品令牌，一个用于用户令牌。 时间 [!DNL Amazon S3] 接收经过身份验证的请求，将计算的签名与提供的签名进行比较。 用于计算签名的多值标头格式不正确，可能会导致身份验证问题。</li> 
         <li>使用临时安全凭据时提供安全令牌。 使用从IAM获得的临时安全凭据发出请求时，必须使用此标头提供安全令牌。 要了解有关临时安全凭据的更多信息，请转到发出请求。</li> 
        </ul> <p>使用的请求需要此标头 [!DNL Amazon DevPay] 和使用临时安全凭据签名的请求。</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL查询字符串]</td> 
   <td> <p>添加所需的查询字符串，如参数或表单字段。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注释:   <p>使用条件语句(例如 <code>if</code> 在JSON中，将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜索

* [[!UICONTROL 列出文件]](#list-files)
* [[!UICONTROL 列出文件夹]](#list-folders)

#### [!UICONTROL 列出文件]

从指定位置返回文件列表。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL AWS] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL区域] </td> 
   <td> <p>选择您的区域端点。 欲了解更多信息，请参见 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">区域端点</a> 在 [!DNL AWS] 文档。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Bucket] </td> 
   <td> <p>选择 [!DNL Amazon S3] 要搜索文件的存储段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL前缀]（可选）</p> </td> 
   <td> <p> 要在其中查找文件的文件夹的路径，例如 <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出文件夹]

从指定位置返回文件夹列表。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL AWS] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL区域] </td> 
   <td> <p>选择您的区域端点。 欲了解更多信息，请参见 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">区域端点</a> 在AWS文档中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Bucket] </td> 
   <td> <p>选择 [!DNL Amazon S3] 要搜索文件夹的分段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL前缀]（可选）</p> </td> 
   <td> <p> 要在其中查找文件夹的文件夹的路径，例如 <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
