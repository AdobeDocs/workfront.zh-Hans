---
title: DocuSign模块
description: 此 [!DNL Adobe Workfront Fusion DocuSign] 模块允许您监视和检索信封状态、搜索和检索信封，或下载并发送文档以登录 [!DNL DocuSign] 帐户。
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: a6ebfe6f-dc3f-41f7-8129-bbc5775cff33
source-git-commit: 632952e91ebe2ae5caa370c310cfd5e7180232b7
workflow-type: tm+mt
source-wordcount: '1895'
ht-degree: 0%

---

# DocuSign模块

此 [!DNL Adobe Workfront Fusion] [!DNL DocuSign] 模块允许您监视和检索信封状态、搜索和检索信封，或下载并发送文档以登录 [!DNL DocuSign] 帐户。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!DNL DocuSign] 模块，您必须具有 [!DNL DocuSign] 帐户。

## Connect [!DNL DocuSign] 到 [!DNL Workfront Fusion] {#connect-docusign-to-workfront-fusion}

为创建连接 [!DNL DocuSign] 模块：

1. 单击 **[!UICONTROL 添加]** 旁边的 [!UICONTROL 连接] 框。 [!DNL DocuSign] 模块。
1. 输入以下内容：

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL连接名称]</p> </td> 
      <td>输入新名称 [!DNL DocuSign] 连接</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL帐户类型]</td> 
      <td>选择您要连接的帐户是生产帐户还是演示帐户。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按照中的说明继续 [创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md#connect).

## [!DNL DocuSign] 模块及其字段

配置时 [!DNL DocuSign] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL DocuSign] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)

### 触发器

#### [!UICONTROL 观看信封]

当信封被发送、投放、签署、完成或拒绝时，此触发器模块会启动一个场景。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL DocuSign] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL帐户] </td> 
   <td> <p>选择包含要监视的记录的帐户。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件类型]</td> 
   <td> <p> 选择要监视的事件类型。</p> 
    <ul> 
     <li>[！UICONTROL文档已完成]</li> 
     <li>[！UICONTROL文档被拒绝]</li> 
     <li>[！UICONTROL文档已发送]</li> 
     <li>[！UICONTROL文档已签名]</li> 
     <li>[！UICONTROL收件箱中的新文档]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL输出字段]</p> </td> 
   <td> <p>选择要包含在模块输出中的字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>输入或映射您希望模块在每个方案执行周期内使用的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 自定义API调用]](#custom-api-call)
* [[!UICONTROL 下载文档]](#download-a-document)
* [[!UICONTROL 阅读信封]](#read-an-envelope)
* [[!UICONTROL 将文件上传到信封]](#upload-a-file-to-an-envelope)
* [[!UICONTROL 创建新信封]](#create-a-new-envelope)
* [[!UICONTROL 将收件人添加到信封]](#add-recipient-to-envelope)
* [[!UICONTROL 添加自定义字段]](#add-custom-field)
* [[!UICONTROL 修改自定义字段]](#modify-custom-field)
* [[!UICONTROL 发送信封]](#send-envelope)

#### [!UICONTROL 自定义API调用]

此操作模块允许您执行自定义API调用。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL DocuSign] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL帐户]</td> 
   <td>输入或映射要用于访问 [!DNL DocuSign] API。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL URL]</td> 
   <td> <p>键入您希望模块与之交互的Web服务器上的地址。</p> <p>您可以键入相对URL，这意味着您不必包含协议(例如 <code>http://</code>)。 这向Web服务器表明交互正在服务器上进行。</p> <p>例如： <code>[!DNL /api/conversations].create</code></p>  </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。 这会确定请求的内容类型。</p> <p>例如，<code> {"Content-type":"application/json"}</code></p> <p>注意：如果您收到错误并且难以确定其来源，请考虑根据 [!DNL Workfront] 文档。 如果自定义API调用返回422 HTTP请求错误，请尝试使用“Content-Type”："text/plain"标头。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注释:  <p>使用条件语句(例如 <code>if</code> 在JSON中，将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td>输入或映射在一个执行周期内要处理的最大结果数。</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**示例：** 列出信封
>
>以下API调用返回 [!DNL DocuSign] 帐户：
>
>**URL**： `/v2.1/accounts/{accountId}/envelopes/`
>
>**方法**： `GET`
>
>**查询字符串**：
>
>* **键**： `from_date`
>
>* **值**： `YYYY-MM-DD`
>
>指定请求何时开始检查帐户中信封的状态更改。
>
>![](assets/example-docusign-setup-350x770.png)
>
>结果可在模块的“输出”中找到，位于“包”>“主体”>“信封”下。
>
>在我们的示例中，返回了6个信封：
>
>![](assets/docusign-example-output-350x677.png)

#### [!UICONTROL 下载文档]

此操作模块下载单个文档。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL DocuSign] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL帐户] </td> 
   <td> <p>选择包含要下载的文档的帐户。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL信封ID]</td> 
   <td> <p> 输入或映射要下载的信封ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL文档ID]</p> </td> 
   <td> <p>输入或映射要下载的文档的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL证书]</td> 
   <td>选择 <strong>[！UICONTROL是]</strong> 如果要在下载中包含信封签名证书。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文档（按用户ID）</td> 
   <td>选择 <strong>[！UICONTROL是]</strong> 如果您希望允许收件人按用户ID检索文档。 例如，如果用户包含在具有相同可见性的两个不同工艺路线订单中，则使用此选项将返回两个工艺路线中的所有单据。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL加密]</td> 
   <td>选择 <strong>[！UICONTROL是]</strong> 如果您希望对响应中返回的PDF字节进行加密，以将其用于您的上配置的所有密钥管理器， [!DNL DocuSign] 帐户。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL语言]</td> 
   <td>选择语言。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL显示更改]</td> 
   <td>当设置为 <strong>[！UICONTROL是]</strong>，返回的PDF的任何更改字段都会以黄色突出显示，可选签名或首字母以红色突出显示。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL水印]</td> 
   <td> <p>选择 <strong>[！UICONTROL否]</strong> 从PDF文档中删除水印。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 阅读信封]

该操作模块读取有关信封的信息 [!DNL DocuSign] 使用信封ID。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL DocuSign] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL帐户] </td> 
   <td> <p>选择包含要从中读取信息的文档的帐户。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL信封ID]</td> 
   <td> <p> 输入或映射ID，该ID包含要从中读取信息的文档。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td>选择要显示在模块输出中的属性。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将文件上传到信封]

此模块将指定文件上传到DocuSign中的现有信封。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL DocuSign] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL帐户] </td> 
   <td> <p>选择包含要上载文件的信封的帐户。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL信封ID]</td> 
   <td> <p> 输入或映射要上载文件的信封的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td>从上一个模块中选择源文件，或输入源文件的名称和数据。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建新信封]

该操作模块从模板创建新信封。 它会返回新信封的ID以及新信封的状态。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader">[！UICONTROL连接] </td>

<td> <p>有关将DocuSign帐户连接到Workfront Fusion的说明，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到Workfront Fusion</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在Adobe Workfront Fusion中创建方案</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[！UICONTROL帐户] </td>
   <td> <p>选择包含要上载文件的信封的帐户。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL模板]</td>
   <td> <p> 选择要从中创建新信封的模板。 基于您选择的[！UICONTROL帐户]提供了模板。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">
     [！UICONTROL After Creation]
   </td> 
   <td> <p>选择是将信封另存为草稿还是发送信封以供签名。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[！UICONTROL模板收件人]</td>
    <td>选择此信封的收件人</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将收件人添加到信封]

此操作模块将一个或多个收件人添加到现有信封。 如果信封已发送，收件人将收到一封电子邮件。 此模块对已完成的信封无效。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
    <td>[！UICONTROL连接] </td>
   <td> <p>有关将DocuSign帐户连接到Workfront Fusion的说明，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到Workfront Fusion</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在Adobe Workfront Fusion中创建方案</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[！UICONTROL帐户] </td>
   <td> <p>选择包含要添加收件人的信封的帐户。</p> </td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL信封ID]</td>
    <td>选择或映射要添加收件人的信封的ID。</td>
  </tr> 
  <tr data-mc-conditions="">
    <td role="rowheader">[！UICONTROL收件人类型]</td>
   <td> <p> 选择要添加到信封的收件人类型。</p> 
    <ul> 
     <li> <p>[！UICONTROL代理]</p> </li> 
     <li> <p>[！UICONTROL副本]</p> </li> 
     <li> <p>[！UICONTROL认证的交付]</p> </li> 
     <li> <p>[！UICONTROL现场签名者]</p> </li> 
     <li> <p>[！UICONTROL Intermediate]</p> </li> 
     <li> <p>[！UICONTROL签名者]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL电子邮件]</td>
   <td> <p>输入或映射要添加到信封中的收件人的电子邮件地址。</p> </td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL名称]</td>
   <td>输入或映射要添加到信封的收件人姓名。</td> 
  </tr> 
  <tr>
    <td>[！UICONTROL路由顺序]</td>
   <td> <p>输入或映射收件人的路由编号。 路由号码确定收件人接收和签署文档的顺序。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[！UICONTROL电子邮件正文]</td>
   <td>输入或映射发送给收件人的电子邮件的正文（内容）。</td> 
  </tr> 
  <tr>
    <td role="rowheader">[！UICONTROL电子邮件主题]</td>
   <td>输入或映射发送给收件人的电子邮件的主题。</td> 
  </tr> 
    <td role="rowheader">[！UICONTROL私人消息]</td>
   <td> <li> <p>只有选定的收件人会看到私密邮件和一般邮件。 私密消息长度限制为1,000个字符。</p> </li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL身份验证]</td> 
   <td> <p>选择要用于确认收件人身份的身份验证方法。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL无]</strong> </p> </li> 
     <li> <p><strong>[！UICONTROL访问代码]</strong> </p> <p>输入或映射访问代码。</p> </li> 
     <li> <p><strong>[！UICONTROL Phone]</strong> </p> <p>输入或映射电话号码</p> </li> 
     <li> <p><strong>[！UICONTROL短信]</strong> </p> <p>输入或映射电话号码</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添加自定义字段]

此操作模块向文档添加一个自定义字段

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL DocuSign] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL帐户] </td> 
   <td> <p>选择包含要添加自定义字段的文档的帐户。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL信封ID]</td> 
   <td> <p> 输入或映射包含要添加自定义字段的文档的信封的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL字段名称]</td> 
   <td>为要添加的新字段输入或映射名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL必填]</td> 
   <td>如果您希望添加的字段为必填字段，请启用此选项。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL显示字段]</td> 
   <td>如果希望字段可见，则启用此选项。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL值]</td> 
   <td>输入或映射添加字段的值（内容）。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 修改自定义字段]

此操作模块使用字段名称修改自定义字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL DocuSign] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL帐户] </td> 
   <td> <p>选择包含要修改自定义字段的文档的帐户。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL信封ID]</td> 
   <td> <p> 输入或映射包含要修改自定义字段的文档的信封的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL字段ID]</td> 
   <td>输入或映射要修改的字段的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL字段名称]</td> 
   <td>输入或映射要修改的字段的名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL必填]</td> 
   <td>如果希望修改的字段为必填字段，请启用此选项。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL显示字段]</td> 
   <td>如果希望字段可见，则启用此选项。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL值]</td> 
   <td>输入或映射修改字段的值（内容）。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 发送信封]

该操作模块会向其收件人发送草稿信封。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL DocuSign] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">Connect [!DNL DocuSign] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL帐户] </td> 
   <td> <p>选择包含要发送给其收件人的草稿信封的帐户。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL信封ID]</td> 
   <td> <p> 输入或映射要发送给其收件人的草稿信封的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>
