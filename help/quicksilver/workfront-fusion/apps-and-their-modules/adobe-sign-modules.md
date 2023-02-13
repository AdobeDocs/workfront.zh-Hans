---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Adobe Acrobat Sign模块
description: 使用 [!DNL Adobe Acrobat Sign] 模块，您可以启动 [!DNL Adobe Workfront Fusion] 基于 [!DNL Adobe] Acrobat Sign帐户、创建、读取或更新协议和其他记录、使用您设置的标准搜索记录并上传文档。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 01158218-31a6-4c68-a9b7-6a678a8f40c9
source-git-commit: 8bb97b08bb5991fadbf2627f4ebfdaa25ae337ce
workflow-type: tm+mt
source-wordcount: '6579'
ht-degree: 0%

---

# [!DNL Adobe Acrobat Sign] 模块

使用 [!DNL Adobe Acrobat Sign] 模块，您可以启动 [!DNL Adobe Workfront Fusion] 基于 [!DNL Adobe Acrobat Sign] 帐户、创建、读取或更新协议和其他记录、使用您设置的标准搜索记录，以及上传文档。

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

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Adobe Acrobat Sign] 连接器使用建议

的 [!DNL Adobe Sign ]应用程序使eSignature业务流程在 [!DNL Fusion] 更简单，更强大。

新用户 [!DNL Adobe Sign] 应密切注意一些对更新协议的限制。 协议通常在开始后不会更改。 我们建议的新用户 [!DNL Adobe Sign] 重点是使用协议创建模块创建新协议。 这样会 [!DNL Fusion] 更轻松、更好地使用 [!DNL Adobe Sign].

[!DNL Adobe Sign] 协议需要一个可与之合作的字段。 有一些方法可以执行此操作，但最简单、最常见的方法是上传临时文档，然后将该文档映射到您的协议。

![](assets/adobe-sign-recommendations-350x168.png)

## [!DNL Adobe Acrobat Sign] 模块及其字段

配置 [!DNL Adobe Acrobat Sign] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Adobe Acrobat Sign] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

<!--
* [Watch for agreements](#watch-for-agreements) 
* [Watch for events](#watch-for-events)
-->

+++ **[!UICONTROL 关注协议]**

此触发器模块会在创建或更新协议时启动方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
<td>有关连接 [!DNL Adobe Acrobat Sign] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></td>  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL过滤器]</td> 
   <td>选择您是要监视新记录、更新记录，还是同时监视这两者。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型] </td> 
   <td>选择希望记录监视的记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查找文本]</td> 
   <td> <p>输入要搜索的术语。 模块会返回将这些术语作为字段值包含在内的记录。</p> <p>有关在 [!DNL Adobe Acrobat Sign]，请参阅 <a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">Adobe Sign搜索 — 工作原理</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回协议的最大数量]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 关注事件]**

当发生您选择的事件时，此触发器模块会启动一个方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td>选择要使用的网页挂接，或单击 <b>[!UICONTROL Add]</b> 并填写以下字段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p>输入网页挂接的名称</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Adobe Acrobat Sign] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL作用域]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL帐户]</p> </li> 
     <li> <p>[!UICONTROL组]</p> </li> 
     <li> <p>[!UICONTROL用户]</p> </li> 
     <li> <p>[!UICONTROL资源]</p> <p>如果选择[!UICONTROL Resource]，请输入资源ID和资源类型。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL资源级别]</td> 
   <td> <p>选择要监视的资源类型。</p> 
    <ul> 
     <li> <p>[!UICONTROL协议]</p> </li> 
     <li> <p>[!UICONTROL小组件]</p> </li> 
     <li> <p>[!UICONTROL巨型符号]</p> </li> 
     <li> <p>[!UICONTROL库文档]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook订阅事件]</td> 
   <td>选择 [!DNL Adobe Sign] 您希望模块监视的事件。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL应用程序显示名称]</td> 
   <td>创建Webhook的应用程序的显示名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL应用程序名称]</td> 
   <td>创建Webhook的应用程序的显示名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL问题通知电子邮件]</td> 
   <td> <p>此设置仅适用于管理员帐户</p> <p>对于要向其发送问题通知电子邮件的每个电子邮件地址，单击 <b>[!UICONTROL Add]</b> 并输入电子邮件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL协议条件参数]</td> 
   <td>如果要添加任何条件参数，请选择 <b>[!UICONTROL Yes]</b> 在要向其添加参数的记录类型上，选择 <b>[!UICONTROL Yes]</b> 的任何参数。</td> 
  </tr> 
 </tbody> 
</table>

+++

### 操作

<!--
* [Create a record](#create-a-record) 
* [Create an agreement](#create-an-agreement) 
* [Create related records](#create-related-records) 
* [Custom API Call](#custom-api-call) 
* [List records](#list-records) 
* [Read a record](#read-a-record) 
* [Read related records](#read-related-records) 
* [Update a record](#update-a-record) 
* [Update related record](#update-related-record) 
* [Upload document](#upload-document)
-->

+++ **[!UICONTROL 创建记录]**

此操作模块会创建所选类型的新记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td>有关连接 [!DNL Adobe Acrobat Sign] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td>以标准JSON对象的形式添加请求的标头。例如， <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td> <p>选择要创建的记录类型。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL组]</b> </p> </li> 
     <li> <p><b>[!UICONTROL库文档]</b> </p> </li> 
     <li> <p><b>[!UICONTROL用户]</b> </p> </li> 
     <li> <p><b>[!UICONTROL Web窗体]（[!UICONTROL小组件]）</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL组信息]</td> 
   <td> <p>输入或映射组的[!UICONTROL Name]和[!UICONTROL ID]，并指示此组是否为帐户的默认组。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL库文档信息]</td> 
   <td> <p>填写以下字段：</p> 
    <ul> 
     <li> <p><b>[！要发送的UICONTROL文件]</b> </p> <p>对于要添加的每个文件，单击 <b>[!UICONTROL添加项目]</b> 并填写字段。</p> 
      <ul> 
       <li><b>[!UICONTROL临时文档ID]</b> <p>输入临时单据的ID</p> </li> 
       <li> <p><b>[!UICONTROL URL文件传输]</b> </p> <p>填写以下字段：</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>输入原始文件的mime类型。 多用途Internet邮件扩展(MIME)类型是允许软件识别在Internet上共享的不同类型数据的标签。 Web服务器和浏览器使用MIME类型来确定应对文件执行的操作。 例如，MIME类型为的文件 <code>text/html</code> 将在浏览器中以不同于MIME类型文件的方式处理 <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL名称]</b> </p> <p>输入文件的名称。</p> </li> 
         <li> <p><b>[!UICONTROL URL]</b> </p> <p>输入要发送的文件的URL。</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL Notarize]</b> </p> <p>选择此文档是否需要公证。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL库模板名称]</b> </p> <p>输入或映射库模板的名称</p> </li> 
     <li> <p><b>[!UICONTROL共享模式]</b> </p> <p>指定谁应有权访问库文档。</p> </li> 
     <li> <p><b>[!UICONTROL库文档状态]</b> </p> <p>选择文档是处于创作状态还是处于活动状态。</p> </li> 
     <li> <p><b>[!UICONTROL库模板类型]</b> </p> <p>对于要使用的每个库模板类型，单击 <b>[!UICONTROL添加项目]</b> ，然后选择模板类型。</p> </li> 
     <li> <p><b>[!UICONTROL上次事件日期]</b> </p> <p>输入在库文档中发生事件的最后日期。</p> <p>有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
     <li> <p><b>[!UICONTROL库文档状态]</b> </p> <p>选择库文档的状态。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL用户信息]</td> 
   <td> <p>填写以下字段：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL电子邮件]</b> </p> <p>输入用户的电子邮件地址。</p> </li> 
     <li> <p><b>[!UICONTROL是帐户管理员]</b> </p> <p>如果创建的用户是帐户管理员，请勾选此选项。</p> </li> 
     <li> <p><b>[!UICONTROL用户ID]</b> </p> <p>输入用户的唯一ID</p> </li> 
     <li> <p><b>[!UICONTROL帐户ID]</b> </p> <p>输入的唯一ID [!DNL Adobe Acrobat Sign] 与此用户关联的帐户。</p> </li> 
     <li> <p><b>[!UICONTROL名字]</b> </p> <p>输入用户的名字。</p> </li> 
     <li> <p><b>[!UICONTROL姓氏]</b> </p> <p>输入用户的姓氏</p> </li> 
     <li> <p><b>[!UICONTROL公司]</b> </p> <p>输入用户的公司名称。</p> </li> 
     <li> <p><b>[!UICONTROL缩写]</b> </p> <p>输入用户的首字母。</p> </li> 
     <li> <p><b>[!UICONTROL区域设置]</b> </p> <p>输入用户的区域设置。 这可确定UI的语言。 </p> </li> 
     <li> <p><b>[!UICONTROL Phone]</b> </p> <p>输入用户的电话号码</p> </li> 
     <li> <p><b>主组ID</b> </p> <p>输入新用户所在的群组。 如果未输入任何内容，则会将用户添加到帐户的默认组。</p> </li> 
     <li> <p><b>[!UICONTROL作业标题]</b> </p> <p>输入用户的作业标题。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Web窗体信息]</td> 
   <td> <p>填写以下字段</p> 
    <ul> 
     <li> <p><b>[!UICONTROL文件信息]</b> </p> <p>对于要添加到Web窗体的每个文件，单击添加并填写以下字段：</p> 
      <ul> 
       <li> <p>[!UICONTROL文件类型]</p> <p>[!UICONTROL Document]</p> </li> 
       <li> <p>[!UICONTROL Transient document]</p> </li> 
       <li> <p>[!UICONTROL URL文件信息]</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Web窗体名称]</b> </p> <p>输入Web窗体的名称。 此名称用于标识电子邮件和网站等位置的Web窗体。</p> </li> 
     <li> <p><b>[!UICONTROL Web窗体状态]</b> </p> <p>选择应创建新Web窗体的状态。</p> </li> 
     <li> <p><b>[!UICONTROL Web表单参与者集信息]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL成员信息]</b> </p> <p>对于要添加到参与者集的每个成员，单击 <b>[!UICONTROL添加项目]</b>. </p> 
        <ul> 
         <li> <p><b>[!UICONTROL电子邮件]</b> </p> <p>将此选项留空。</p> </li> 
         <li> <p><b>[!UICONTROL安全选项]</b> </p> <p>如果要添加用于验证此用户的安全选项，请选择 <b>[!UICONTROL Yes]</b>，然后选择安全选项并填写所需的任何字段。</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL角色]</b> </p> <p>选择角色。 此参与者集的所有成员都共享角色。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Web窗体其他参与者集信息]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL成员信息]</b> </p> <p>对于要添加到参与者集的每个成员，单击 <b>[!UICONTROL添加项目]</b>.</p> 
        <ul> 
         <li> <p><b>[!UICONTROL电子邮件]</b> </p> <p>将此选项留空。</p> </li> 
         <li> <p><b>[!UICONTROL安全选项]</b> </p> <p>如果要添加用于验证此用户的安全选项，请选择 <b>[!UICONTROL Yes]</b>，然后选择安全选项并填写所需的任何字段。</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL角色]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Web表单参与者ID] </b> </p> <p>输入Web窗体参与者的ID。</p> </li> 
       <li> <p><b>[!UICONTROL顺序]</b> </p> <p>指定此参与者集与Web窗体交互的顺序。 例如，订单值为1的参与者组必须先到达，而后必须到达2，依此类推。 订单编号必须以1开头，并且该系列中没有空白。 </p> </li> 
       <li> <p><b>[!UICONTROL提供程序参与者集信息]</b> </p> <p>如果参与者未知，请输入提供者是否必须提供该参与者的详细信息，然后输入一条消息，其中包含您为未知参与者提供的详细信息。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL身份验证失败信息]</b> </p> <p>如果要为用户提供失败或错误页面，请选择 <b>[!UICONTROL Yes]</b>，然后填写以下字段：</p> 
      <ul> 
       <li> <p><b>[!UICONTROL URL]</b> </p> <p>输入错误页面的URL</p> </li> 
       <li> <p><b>[!UICONTROL Deframe]</b> </p> <p>如果希望错误页面显示在Web窗体内，请启用此选项</p> </li> 
       <li> <p><b>[!UICONTROL Delay]</b> </p> <p>在用户被重定向到错误页面之前，输入延迟（以秒为单位）。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL CC信息]</b> </p> <p>对于在Web窗体上签署最终协议时要接收电子邮件的每个电子邮件地址，单击 <b>[!UICONTROL添加项目]</b> 并输入电子邮件地址。</p> </li> 
     <li> <p><b>[!UICONTROL完成信息]</b> </p> <p style="font-style: normal;">如果要为用户提供成功页面，请选择 <b>[!UICONTROL Yes]</b>，然后填写以下字段：</p> 
      <ul> 
       <li> <p><b>[!UICONTROL URL]</b> </p> <p>输入成功页面的URL</p> </li> 
       <li> <p><b>[!UICONTROL Deframe]</b> </p> <p>如果希望成功页面显示在Web窗体中，请启用此选项</p> </li> 
       <li> <p><b>[!UICONTROL Delay]</b> </p> <p>在用户被重定向到成功页面之前，输入延迟（以秒为单位）。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL组ID]</b> </p> <p>输入Web窗体所属的组的ID。 如果未输入任何内容，则Web窗体属于帐户用户的主组。</p> </li> 
     <li> <p><b>[!UICONTROL上次事件日期]</b> </p> <p>输入在Web窗体上发生最后一个事件的日期。 使用格式 <code>yyyy-MM-dd'T'HH:mm:ssZ</code>.</p> </li> 
     <li> <p><b>[!UICONTROL区域设置]</b> </p> <p>输入用户的区域设置。 这可确定UI的语言。 </p> </li> 
     <li> <p><b>[!UICONTROL安全选项]n</b> </p> <p>输入用于保护文档的密码。 您必须单独将此密码告知任何相关方。</p> </li> 
     <li> <p><b>[!UICONTROL Vaulting info]</b> </p> <p>如果已为文档保险存储设置帐户，并且根据协议启用了选项，则可以启用此选项以保管本协议。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 创建协议]**

此操作模块会创建协议，将其发出以供签名，并返回协议ID。

>[!NOTE]
>
>我们建议上传文档以作为临时文档进行签名，然后将其映射到 [!UICONTROL 要发送的文件] 字段 [!UICONTROL 创建协议] 模块。 有关示例，请参阅本文中的“上传文档”。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
<td>有关连接 [!DNL Adobe Acrobat Sign] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></td>  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td>以标准JSON对象的形式添加请求的标头。例如， <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！要发送的UICONTROL文件]</td> 
   <td> <p>对于要包含在协议中的每个项目，单击 <b>[!UICONTROL Add Item]</b> 并填写以下字段：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL文件类型]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL Document]</b> </p> <p>填写以下字段：</p> 
        <ul> 
         <li> <p><b>[!UICONTROL创建日期]</b> </p> <p>输入或映射以格式创建文档的日期 <code>yyyy-MM-dd'T'HH:mm:ssZ</code>. 例如， <code>2016-02-25T18:46:19Z</code> 表示UTC时间。</p> </li> 
         <li> <p><b>[!UICONTROL ID]</b> </p> <p>输入或映射文档的ID。</p> </li> 
         <li> <p><b>[!UICONTROL标签]</b> </p> <p>输入或映射文件的唯一标签。 对于自定义工作流，此操作会将文件映射到工作流定义中的相应文件元素。 在自定义工作流协议创建请求中必须指定此参数。</p> </li> 
         <li> <p><b>[!UICONTROL页数]</b> </p> <p>输入或映射文档中的页数。</p> </li> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>输入或映射原始文件的mime类型。 多用途Internet邮件扩展(MIME)类型是允许软件识别在Internet上共享的不同类型数据的标签。 Web服务器和浏览器使用MIME类型来确定应对文件执行的操作。 例如，MIME类型为的文件 <code>text/html</code> 将在浏览器中以不同于MIME类型文件的方式处理 <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL名称]</b> </p> <p>输入或映射文档的名称。<br></p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL库文档ID]</b> </p> <p>输入库文档的ID</p> </li> 
       <li> <p><b>[!UICONTROL临时文档ID]</b> </p> <p>输入临时单据的ID</p> </li> 
       <li> <p><b>[!UICONTROL URL文件传输]</b> </p> <p>填写以下字段：</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>输入原始文件的mime类型。 多用途Internet邮件扩展(MIME)类型是允许软件识别在Internet上共享的不同类型数据的标签。 Web服务器和浏览器使用MIME类型来确定应对文件执行的操作。 例如，MIME类型为的文件 <code>text/html</code> 将在浏览器中以不同于MIME类型文件的方式处理 <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL名称]</b> </p> <p>输入文件的名称。</p> </li> 
         <li> <p><b>[!UICONTROL URL]</b> </p> <p>输入要发送的文件的URL。</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL标签]</b> </p> <p>输入文件的标签。</p> </li> 
     <li> <p><b>[!UICONTROL Notarize]</b> </p> <p>启用此选项以指示文件必须经过公证。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL协议名称]</td> 
   <td>输入新协议的名称。 此名称用于在电子邮件和网站等位置标识协议。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL参与者集信息]</td> 
   <td> <p>对于要添加的每个参与者集，单击 <b>[!UICONTROL添加项目]</b> 并填写以下字段。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL成员]</b> </p> <p>对于要添加到参与者集的每个人员，单击 <b>[!UICONTROL添加项目]</b> 并输入该人的电子邮件地址。</p> </li> 
     <li> <p><b>[!UICONTROL顺序]</b> </p> <p>指定此参与者集应何时签署协议的顺序。 例如，订单值为1的参与者组必须先签名，然后必须先签名2，然后再签名，依此类推。 订单编号必须以1开头，并且该系列中没有空白。 </p> </li> 
     <li> <p><b>[!UICONTROL角色]</b> </p> <p>为此参与者集选择角色。 集中的所有参与者都将收到此角色。</p> </li> 
     <li> <p><b>[!UICONTROL ID]</b> </p> <p>输入或映射此参与者集的ID。</p> </li> 
     <li> <p><b>[!UICONTROL标签]</b> </p> <p>输入或映射参与者集的唯一标签。 对于自定义工作流，参与集中指定的标签应将其映射到自定义工作流中的参与步骤。</p> </li> 
     <li> <p><b>[!UICONTROL名称]</b> </p> <p>输入参与者集的名称。 此名称在协议中必须唯一。</p> </li> 
     <li> <p><b>[!UICONTROL私信]</b> </p> <p>输入或映射此参与者集的消息。 集合中的所有参与者都会收到此消息。</p> </li> 
     <li> <p><b>[!UICONTROL可见页面]</b> </p> <p>如果为此协议启用了有限的文档可见性，请指定哪些文件对此参与者集可见。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL签名类型]</td> 
   <td> <p>选择协议需要的签名类型。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL E-sign]</b> </p> <p>协议必须以电子方式签署。</p> </li> 
     <li> <p><b>[!UICONTROL Writted]</b> </p> <p>协议必须手工签署，且已签署的协议必须扫描并上传。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td> <p>选择此协议的状态。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL创作]</b> </p> <p>您仍可以编辑或添加字段到此协议。</p> </li> 
     <li> <p><b>[!UICONTROL草稿]</b> </p> <p>您可以在发送协议之前以增量方式构建此协议。</p> </li> 
     <li> <p><b>[！正在处理的UICONTROL]</b> </p> <p>此协议将立即发送。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CCs]</td> 
   <td> <p>您可以将此协议发送给不需要签署的相关方，如利益相关方。 他们在签名过程开始时会收到一封电子邮件，在收到最终签名时会收到另一封电子邮件。 他们还会收到协议的PDF副本。 </p> <p>对于您要在此协议上抄送的每个人员，单击 <b>[!UICONTROL添加项目]</b> 并填写以下字段：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL电子邮件]</b> </p> <p>输入或映射您要在协议中抄送的电子邮件地址。</p> </li> 
     <li> <p><b>[!UICONTROL标签]</b> </p> <p>输入或映射此电子邮件地址的标签，如工作流描述中所示</p> </li> 
     <li> <p><b>[!UICONTROL可见页面]</b> </p> </li> 
     <li> <p>如果为此协议启用了有限的文档可见性，请指定哪些文件对此参与者集可见。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL电子邮件选项]</td> 
   <td> <p>对于每种类型的电子邮件，选择是将此类电子邮件发送给所有参与者还是不发送。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL完成电子邮件]</b> </p> <p>在此协议完成、取消、过期或拒绝时发送电子邮件。</p> </li> 
     <li> <p><b>[!UICONTROL投放中的电子邮件]</b> </p> <p>委派或替换此协议时，会发送电子邮件。</p> </li> 
     <li> <p><b>[!UICONTROL协议启动电子邮件]</b> </p> <p>创建此协议或请求对其执行操作时，发送电子邮件。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL External ID]</td> 
   <td> <p>输入或映射此协议的ID。 您可以在创建协议时指定此参数，然后使用它在以后的模块或查询中查找协议。</p> <p>注意：外部ID值通过API对所有参与者都可见，因此不应使用它包含敏感令牌。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL合并字段信息]</td> 
   <td> <p>对于协议中要为其设置默认值的每个字段，单击 <b>[!UICONTROL添加项目]</b> 并输入默认值和字段名称。</p> <p>这些值将呈现给可编辑字段的签名者对于只读字段，在签名过程中提供的值将不可编辑。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL公证信息]</td> 
   <td> <p>填写以下字段：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Appoint]</b> </p> <p>输入或映射为公证本协议而进行的约会的建议日期和时间。</p> </li> 
     <li> <p><b>[!UICONTROL注意]</b> </p> <p>输入或映射您要包含的有关公证会议的任何注释。</p> </li> 
     <li> <p><b>[!UICONTROL Payment]</b> </p> <p>选择公证员是由签署者还是协议发件人支付。</p> </li> 
     <li> <p><b>[!UICONTROL公证类型]</b> </p> <p>选择公证员类型</p> 
      <ul> 
       <li> <p>[!UICONTROL Provider Verenator]</p> <p>公证员由公证员提供。</p> </li> 
       <li> <p>[!UICONTROL边公证员]</p> <p>公证员由客户提供。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL帖子签名选项]</td> 
   <td> <p>选择是否希望在签署协议后将签名者定向到成功页面。 如果您选择 <b>[!UICONTROL Yes]</b>，填写以下字段：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL重定向延迟]</b> </p> <p>输入或映射一个数字，表示在将签名者重定向到成功页面之前所经过的秒数。 如果此值大于0，则用户将首先看到标准 [!DNL Adobe Sign] 成功消息，之后延迟后将被重定向到您的成功页面。</p> </li> 
     <li> <p><b>[!UICONTROL重定向URL]</b> </p> <p>输入或映射一个可公开访问的URL，用户在成功完成签名过程后将被发送到该URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL安全选项]</td> 
   <td> <p>输入或映射用于保护PDF文档的辅助密码。 </p> <p>重要信息： [!DNL Adobe Sign] 将永远不共享此密码，因此您必须单独将其与任何相关方通信。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vaulting info]</td> 
   <td>如果已为文档保险存储设置帐户，并且根据协议启用了选项，则可以启用此选项以保管本协议。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 创建相关记录]**

此操作模块会创建链接到您选择的模块的记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Adobe Acrobat Sign] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自动添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择要将创建的记录与之关联的原始记录的记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agreement]/[!UICONTROL Library Document]/[!UICONTROL User]/[!UICONTROL Widget ID]</td> 
   <td>输入或映射要将创建的记录与其关联的对象的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL协议相关字段]</td> 
   <td> <p>选择要创建的相关字段类型</p> 
    <ul> 
     <li> <p><b>[!UICONTROL表单字段]</b> </p> <p>输入包含要创建的字段的模板ID</p> </li> 
     <li> <p><b>[!UICONTROL提醒]</b> </p> <p>填写以下字段：</p> 
      <ul> 
       <li> <p><b>[!UICONTROL收件人参与者ID]</b> </p> <p>对于要接收提醒的每个参与者，单击[!UICONTROL添加项目]，然后输入参与者的ID。</p> </li> 
       <li> <p><b>[!UICONTROL状态]</b> </p> <p>对于新记录，状态必须为[!UICONTROL Active]。</p> </li> 
       <li> <p><b>[!UICONTROL首次提醒延迟]</b> </p> <p>在发送第一个提醒之前输入延迟（以小时为单位）。 允许的最小值为1小时，最大值不能超过协议创建时间与协议到期时间（以小时为单位）的差值。 如果未设置此延迟，则第一个提醒将基于频度。</p> </li> 
       <li> <p><b>[!UICONTROL提醒频度]</b> </p> <p>设置发送提醒的频率。 如果未提供频率，则只发送一次提醒。</p> </li> 
       <li> <p><b>[!UICONTROL上次发送日期]</b> </p> <p>此字段由系统设置。</p> </li> 
       <li> <p><b>[!UICONTROL下次发送日期]</b> </p> <p>此字段必须为空或设置为[!UICONTROL ONCE]。</p> </li> 
       <li> <p><b>[!UICONTROL注意]</b> </p> <p>输入要包含在提醒中的注释。 这有助于告知参与者为何需要其参与。</p> </li> 
       <li> <p><b>[!UICONTROL开始提醒计数器来自]</b> </p> <p>选择是否根据在上创建协议的时间（提醒可用时）发送提醒。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL签名者身份报告]</b> </p> <p>输入用于保护PDF文档的密码。</p> </li> 
     <li> <p><b>[!UICONTROL视图]</b> </p> <p>输入以下字段</p> 
      <ul> 
       <li> <p><b>[!UICONTROL名称]</b> </p> <p>选择要创建的视图的名称。</p> </li> 
       <li> <p><b>[!UICONTROL自动登录用户]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 自动将用户登录到返回的URL。</p> </li> 
       <li> <p><b>[!UICONTROL帧父项]</b> </p> <p>输入或映射以逗号分隔的父域URL列表，其中可能会找到返回的URL。 如果留空，则 [!DNL Adobe Acrobat Sign] 页面在iframe中不可见。</p> </li> 
       <li> <p><b>[!UICONTROL区域设置]</b> </p> <p>输入要在中创建视图的语言。 </p> </li> 
       <li> <p><b>[!UICONTROL无Chrome标记]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 以显示嵌入的页面，而不显示导航页眉或页脚。</p> </li> 
       <li> <p><b>[!UICONTROL可以编辑文件]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 如果希望通过添加或删除文件来编辑文件上传部分。 这不是访问控制机制。 默认值为[!UICONTROL Yes]。</p> </li> 
       <li> <p><b>[!UICONTROL库文档]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 如果希望库文档链接可见。 默认值为[!UICONTROL Yes]。</p> </li> 
       <li> <p><b>[!UICONTROL本地文件]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 如果您希望显示本地文件上传按钮，请执行以下操作。 默认值为[!UICONTROL Yes]。</p> </li> 
       <li> <p><b>[!UICONTROL Web连接器]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 如果希望显示用于附加来自web源的文档的链接。 默认值为“是”。</p> </li> 
       <li> <p><b>[！已选择UICONTROL预览]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 将“撰写”页面设置为“创作”模式。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL成员共享]</b> </p> <p>对于要与其共享协议的每个成员，单击 <b>[!UICONTROL添加项目]</b> 并输入成员的电子邮件地址和发送给该成员的消息。</p> </li> 
     <li> <p>[!UICONTROL委派参与者集]</p> 
      <ul> 
       <li> <p><b>[!UICONTROL参与者集ID]</b> </p> <p>输入参与者集的ID</p> </li> 
       <li> <p><b>[!UICONTROL成员信息]</b> </p> <p>对于要添加的每个成员，单击[!UICONTROL添加项目]并输入该成员的电子邮件地址和电话信息。</p> </li> 
       <li> <p><b>[!UICONTROL私信]</b> </p> <p>输入消息。 参与者集的所有成员都会收到此消息。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL库视图信息]</td> 
   <td> <p>填写以下字段：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL名称]</b> </p> <p>输入库模板的名称。 此名称用于电子邮件和网站。</p> </li> 
     <li> <p><b>[!UICONTROL自动登录用户]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 自动将用户登录到返回的URL。</p> </li> 
     <li> <p><b>[!UICONTROL帧父项]</b> </p> <p>输入或映射以逗号分隔的父域URL列表，其中可能会找到返回的URL。 如果留空，则 [!DNL Adobe Acrobat Sign] 页面在iframe中不可见。</p> </li> 
     <li> <p><b>[!UICONTROL区域设置]</b> </p> <p>输入要在中创建视图的语言。 </p> </li> 
     <li> <p><b>[!UICONTROL无Chrome标记]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 以显示嵌入的页面，而不显示导航页眉或页脚。</p> </li> 
     <li> <p><b>[!UICONTROL发送视图配置]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 如果要配置[!UICONTROL Send]视图，请填写以下字段。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL协议名称]</b> </p> <p>在撰写页面上输入或映射库文档的协议名称。</p> </li> 
       <li> <p><b>[!UICONTROL可以编辑文件]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 如果希望通过添加或删除文件来编辑文件上传部分。 这不是访问控制机制。 默认值为[!UICONTROL Yes]。</p> </li> 
       <li> <p><b>[!UICONTROL本地文件]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 如果希望库文档链接可见。 默认值为[!UICONTROL Yes]。</p> </li> 
       <li> <p><b>[!UICONTROL Web连接器]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 如果希望显示用于附加来自web源的文档的链接。 默认值为[!UICONTROL Yes]。</p> </li> 
       <li> <p><b>已选中预览</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 将“撰写”页面设置为“创作”模式。</p> </li> 
      </ul> <p> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL用户视图信息]</td> 
   <td> <p>填写以下字段</p> 
    <ul> 
     <li> <p><b>[!UICONTROL名称]</b> </p> <p>选择请求的用户视图的名称。</p> </li> 
     <li> <p><b>[!UICONTROL自动登录用户]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 自动登录。 选择 <b>[!UICONTROL No]</b> 需要凭据。 默认值为[!UICONTROL No]。</p> </li> 
     <li> <p><b>[!UICONTROL帧父项]</b> </p> <p>输入或映射以逗号分隔的父域URL列表，其中可能会找到返回的URL。 如果留空，则 [!DNL Adobe Acrobat Sign] 页面在iframe中不可见。</p> </li> 
     <li> <p><b>无铬黄标记</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 以显示嵌入的页面，而不显示导航页眉或页脚。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL小组件相关字段]</td> 
   <td> <p>选择要创建的相关记录。</p> 
    <ul> 
     <li> <p>[!UICONTROL视图]</p> <p>填写以下字段。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL名称]</b> </p> <p>选择请求的Web窗体视图的名称</p> </li> 
       <li> <p><b>[!UICONTROL自动登录用户]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 自动登录。 选择 <b>[!UICONTROL No]</b> 需要凭据。 默认值为[!UICONTROL No]。</p> </li> 
       <li> <p><b>[!UICONTROL帧父项]</b> </p> <p>输入或映射以逗号分隔的父域URL列表，其中可能会找到返回的URL。 如果留空，则 [!DNL Adobe Acrobat Sign] 页面在iframe中不可见。</p> </li> 
       <li> <p><b>[!UICONTROL区域设置]</b> </p> <p>输入要在中创建视图的语言。 </p> </li> 
       <li> <p><b>[!UICONTROL无Chrome标记]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 以显示嵌入的页面，而不显示导航页眉或页脚。</p> </li> 
       <li> <p>[!UICONTROL个性化签名视图配置]</p> <p>如果要配置个性化的签名视图，请选择 <b>[!UICONTROL Yes]</b> 并填写以下字段：</p> 
        <ul> 
         <li> <p><b>[!UICONTROL电子邮件]</b> </p> <p>输入接收新创建的Web窗体的人员的电子邮件地址</p> </li> 
         <li> <p><b>[!UICONTROL注释]</b> </p> <p>输入描述API调用者如何建立签名者身份的注释。 此信息显示在 [!DNL Adobe Acrobat Sign] 审核跟踪。</p> </li> 
         <li> <p><b>[!UICONTROL过期]</b> </p> <p>输入此Web表单的个性化到期日期。 </p> <p>有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">在中键入强制 [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
         <li> <p><b>[!UICONTROL可重用]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 如果您希望目标签名者能够多次对表单签名。</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL成员共享]</b> </p> <p>对于要与其共享协议的每个成员，单击 <b>[!UICONTROL添加项目]</b> 并输入成员的电子邮件地址和发送给该成员的消息。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 自定义API调用]**
此模块允许您执行自定义API调用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Adobe Acrobat Sign] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>输入相对于 <code>https://api.[region].adobesign.com/api/rest/v6/</code></p> <p>注意：有关可用端点的列表，请参阅 [!DNL Adobe Sign] API引用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL方法]</p> </td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自动添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询字符串] </td> 
   <td> <p>输入请求查询字符串。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。</p> <p>注释:  <p>使用条件语句时，例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL上传临时文档]</td> 
   <td> <p>如果要上载临时文档，请输入要上载的文档的源文件。</p> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 列出记录]**

此操作模块列出了帐户有权访问的选定类型的所有记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Adobe Acrobat Sign] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自动添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择要为其检索相关记录的记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL区域设置]</td> 
   <td> <p>输入用户的区域设置。 这可确定UI的语言。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL External ID]</td> 
   <td>输入或映射外部ID(在 [!DNL Adobe Acrobat Sign])，以获取要返回的协议。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL组ID]</td> 
   <td>输入与要列出的记录关联的组ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL显示隐藏（记录）]</td> 
   <td>如果要在结果中包含隐藏记录，请启用此选项。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cursor] / [!UICONTROL Start index]</td> 
   <td> <p>输入模块应返回的第一个记录的编号。 </p> <p>注意：此字段与用于分页的[!UICONTROL返回记录的最大数]字段组合使用。 例如，如果[!UICONTROL返回事件的最大数]为100，而[!UICONTROL开始索引]为101，则模块会返回记录101-200，或结果的第二页。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回记录的最大数]</td> 
   <td> <p>在每个方案执行周期中，输入或映射希望模块[action]的最大记录数。</p> <p>注意：此字段与用于分页的[!UICONTROL Cursor]或[!UICONTROL Start Index]字段组合。 例如，如果[!UICONTROL返回事件的最大数]为100，而[!UICONTROL开始索引]为101，则模块会返回记录101-200，或结果的第二页。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL父域URL]</td> 
   <td> <p>输入或映射以逗号分隔的父域URL列表，其中可能会找到返回的URL。 如果留空，则 [!DNL Adobe Acrobat Sign] 页面在iframe中不可见。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 读取记录]**

此操作模块从单个记录中检索信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Adobe Acrobat Sign] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自动添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择要为其检索相关记录的记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录ID]</td> 
   <td>输入或映射要检索的记录的ID。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 读取相关记录]**

阅读与单个记录相关的其他信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Adobe Acrobat Sign] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自动添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择要为其检索相关记录的记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录ID](示例：[!UICONTROL帐户ID])</td> 
   <td>输入或映射要为其检索相关记录的记录的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL其他字段]</td> 
   <td>根据记录类型和相关字段在特定字段中输入信息。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 更新记录]**

此操作模块会更新 [!DNL Adobe Acrobat Sign].

>[!IMPORTANT]
>
>* 作为最佳实践，如果您预计协议会发生重大更改，我们建议创建新协议，而不是更新现有协议。
>* 某些更新包含必填字段。 在配置更新时，请确保填写所有必填字段。 必填字段以粗体显示 [!DNL Workfront Fusion] 模块。
>




<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Adobe Acrobat Sign] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自动添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录ID] </td> 
   <td>输入或映射要更新的记录的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择要更新的记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL其他字段]</td> 
   <td> <p>根据记录类型和相关字段在特定字段中输入信息。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL协议]</b> </p> <p>作为最佳实践，如果您预计协议会发生重大更改，我们建议创建新协议，而不是更新现有协议。</p> </li> 
     <li> <p><b>[!UICONTROL库文档]</b> </p> <p>选择要更新的字段，然后填写选定的字段：</p> 
      <ul> 
       <li> <p><b>[!UICONTROL状态]</b> </p> <p>为库文档选择新状态。</p> </li> 
       <li> <p><b>[!UICONTROL名称]</b> </p> <p>输入或映射库模板的名称</p> </li> 
       <li> <p><b>[!UICONTROL共享模式]</b> </p> <p>指定谁应有权访问库文档。</p> </li> 
       <li> <p><b>[!UICONTROL库模板类型]</b> </p> <p>对于要使用的每个库模板类型，单击 <b>[!UICONTROL添加项目]</b> ，然后选择模板类型。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL用户]</b> </p> <p>选择要更新的字段，然后填写选定的字段：</p> 
      <ul> 
       <li> <p><b>[!UICONTROL名字]</b> </p> <p>输入用户的名字。</p> </li> 
       <li> <p><b>[!UICONTROL姓氏]</b> </p> <p>输入用户的姓氏</p> </li> 
       <li> <p><b>[!UICONTROL公司]</b> </p> <p>输入用户的公司名称。</p> </li> 
       <li> <p><b>[!UICONTROL Phone]</b> </p> <p>输入用户的电话号码</p> </li> 
       <li> <p><b>[!UICONTROL主组ID]</b> </p> <p>输入新用户所在的群组。 如果未输入任何内容，则会将用户添加到帐户的默认组。</p> </li> 
       <li> <p><b>[!UICONTROL作业标题]</b> </p> <p>输入用户的作业标题。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Web窗体]（[!UICONTROL小组件]）</b> </p> <p>根据记录类型和相关字段在特定字段中输入信息。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 更新相关记录]**

此操作模块更新与特定对象相关的记录。

>[!IMPORTANT]
>
>* 作为最佳实践，如果您预计协议会发生重大更改，我们建议创建新协议，而不是更新现有协议。
>* 某些更新包含必填字段。 在配置更新时，请确保填写所有必填字段。 必填字段以粗体显示 [!DNL Workfront Fusion] 模块。
>




<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Adobe Acrobat Sign] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自动添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td>选择相关字段所关联的记录的记录类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agreement]/[!UICONTROL Library Document]/[!UICONTROL User]/[!UICONTROL Widget ID]</td> 
   <td>输入或映射要将创建的记录与其关联的对象的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL其他字段]</td> 
   <td> <p>根据记录类型和相关字段在特定字段中输入信息。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL协议]</b> </p> <p>作为最佳实践，如果您预计协议会发生重大更改，我们建议创建新协议，而不是更新现有协议。</p> </li> 
     <li> <p><b>[!UICONTROL库文档]</b> </p> <p>选择要更新的字段，然后填写选定的字段：</p> 
      <ul> 
       <li> <p><b>[!UICONTROL State]</b> </p> <p>为库文档选择新状态。</p> </li> 
       <li> <p><b>[!UICONTROL注意]</b> </p> <p>输入或映射注释的文本。</p> </li> 
       <li> <p><b>[!UICONTROL可见性]</b> </p> <p>选择是显示还是显示库文档。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL用户]</b> </p> <p>选择要更新的字段，然后填写选定的字段：</p> 
      <ul> 
       <li> <p><b>[!UICONTROL组信息列表]</b> </p> <p>填写以下字段</p> 
        <ul> 
         <li> <p><b>[!UICONTROL状态]</b> </p> <p>为用户选择新状态。</p> </li> 
         <li> <p><b>[!UICONTROL ID]</b> </p> <p>输入群组的唯一ID</p> </li> 
         <li> <p><b>[!UICONTROL是组管理员]</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 将此用户设为群组管理员。</p> </li> 
         <li> <p><b>是主组</b> </p> <p>选择 <b>[!UICONTROL Yes]</b> 将此组更新为用户的主组。</p> </li> 
         <li> <p><b>[!UICONTROL创建日期]</b> </p> <p>输入创建群组的日期。</p> <p>有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">在[!UICONTROL Adobe Workfront Fusion]中键入强制</a>.</p> </li> 
         <li> <p><b>[!UICONTROL名称]</b> </p> <p>输入或映射群组的名称。</p> </li> 
         <li> <p><b>[!UICONTROL库文档创建可见]</b> </p> <p>这些设置决定用户是否可以创建库文档</p> 
          <ul> 
           <li> <p>[!UICONTROL值]</p> <p>允许</p> </li> 
           <li> <p>[!UICONTROL Inherited]</p> <p>从组或帐户继承组设置</p> </li> 
          </ul> </li> 
         <li> <p><b>[!UICONTROL发送仅限工作流]</b> </p> <p>这些设置决定用户是否可以仅使用工作流创建协议。</p> 
          <ul> 
           <li> <p>[!UICONTROL值]</p> <p>允许</p> </li> 
           <li> <p>[!UICONTROL Inherited]</p> <p>从组或帐户继承组设置</p> </li> 
          </ul> </li> 
         <li> <p><b>[!UICONTROL用户可以发送]</b> </p> 
          <ul> 
           <li> <p>[!UICONTROL值]</p> <p>允许</p> </li> 
           <li> <p>[!UICONTROL Inherited]</p> <p>从组或帐户继承组设置</p> </li> 
          </ul> </li> 
        </ul> </li> 
      </ul> 
      <ul> 
       <li> <p><b>[!UICONTROL State]</b> </p> <p>为用户选择新状态，然后输入有关激活或停用用户的原因的评论。</p> </li> 
       <li> <p><b>[!UICONTROL区域设置]</b> </p> <p>输入用户的区域设置。 这可确定UI的语言。 </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Web窗体]（[!UICONTROL小组件]）</b> </p> <p>根据记录类型和相关字段在特定字段中输入信息。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 上载文档]**

上传临时文档。 临时文档在上传后7天内可用。

>[!NOTE]
>
>我们建议上传文档以作为临时文档进行签名，然后将其映射到创建协议模块中的“要发送的文件”字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Adobe Acrobat Sign] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自动添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录ID]</td> 
   <td>输入或映射要更新的记录的ID</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL MIME类型]</td> 
   <td>输入原始文件的mime类型。 多用途Internet邮件扩展(MIME)类型是允许软件识别在Internet上共享的不同类型数据的标签。 Web服务器和浏览器使用MIME类型来确定应对文件执行的操作。 例如，MIME类型为的文件 <code>text/html</code> 将在浏览器中以不同于MIME类型文件的方式处理 <code>image/jpeg</code>.</td> 
  </tr> 
 </tbody> 
</table>

**示例：** 在此工作流中，要签名的文档(以前从Workfront下载)将作为临时文档上传。

![](assets/sign-example-1-350x308.png)

的 [!UICONTROL 上载文档] 模块为文档提供 [!DNL Adobe Acrobat Sign] 可在以后的模块中引用的ID。 创建协议后，上传文档的ID将包含在 [!UICONTROL 要发送的文件] 字段。

![](assets/sign-example-2-350x356.png)

+++

### 搜索

+++ **[!UICONTROL 搜索协议]**

此搜索模块会根据您提供的条件搜索协议。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Adobe Acrobat Sign] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文本过滤器]</td> 
   <td> <p>在协议元数据中搜索文本。 </p> 
    <ul> 
     <li> <p><b>[!UICONTROL查找文本]</b> </p> <p>输入要在协议元数据中查找的文本。 每个单词都被视为单独的文本项。 </p> </li> 
     <li> <p><b>[!UICONTROL在中查找文本]</b> </p> <p>选择要在中查找文本的元数据字段。 如果未选择任何内容，则模块会搜索所有元数据。</p> </li> 
    </ul> <p>该模块会返回任何协议，其中包含任何选定字段中的任何输入文本。 示例：输入“spring campaign”并选择“标题”和“备注”选项，将返回在“标题”或“备注”中使用“Spring”或“Campaign”字样的任何协议。</p> <p>有关在 [!DNL Adobe Acrobat Sign]，请参阅 <a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">[!DNL Adobe Sign] 搜索 — 工作原理</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL创建日期]</td> 
   <td>选择日期。 模块仅返回创建日期与此条件匹配的记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL过期日期]</td> 
   <td>选择日期。 模块仅返回过期日期与此条件匹配的记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL修改日期]</p> </td> 
   <td>选择日期。 模块仅返回修改日期与此条件匹配的记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL External ID]</td> 
   <td> <p> 外部ID是由发件人分配的协议ID，可采用任何形式，但通常采用“&lt;groupid&gt;:&lt;id&gt;"</p> <p>对于要添加的每个外部ID，单击 <b>[!UICONTROL Add]</b> 并输入或映射外部ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL组ID]</td> 
   <td> <p>组ID是在创建组时分配的标识符。</p> <p>对于要添加的每个外部ID，单击 <b>[!UICONTROL Add]</b> 并输入或映射外部ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL资产ID]</td> 
   <td> <p>这是分配给特定协议的ID。 </p> <p>对于要添加的每个外部ID，单击 <b>[!UICONTROL Add]</b> 并输入或映射外部ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL父ID]</td> 
   <td> <p>这是分配给协议父对象的ID。 </p> <p>对于要添加的每个外部ID，单击 <b>[!UICONTROL Add]</b> 并输入或映射外部ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL参与者电子邮件]</td> 
   <td> <p>参与者的电子邮件地址。 </p> <p>对于要添加的每个外部ID，单击 <b>[!UICONTROL Add]</b> 并输入或映射外部ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL角色]</td> 
   <td>选择希望返回结果包含的角色。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL排序依据]</td> 
   <td>如果希望模块对结果进行排序，请选择要按结果排序的字段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL排序顺序]r</td> 
   <td>如果希望模块对结果进行排序，请选择是升序排序还是降序排序。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL状态]</td> 
   <td>选择您希望返回的结果包含的状态。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>选择您希望返回结果包含的协议类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL子类型]</td> 
   <td>选择您希望返回结果包含的协议子类型。 只有库模板协议具有子类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL用户ID]</td> 
   <td> <p>与协议共享的用户的用户ID。</p> <p>对于要添加的每个用户ID，单击 <b>[!UICONTROL Add]</b> 并输入或映射用户ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL可见性]</td> 
   <td>选择希望返回结果包含的可见性级别。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL开始索引]</td> 
   <td> <p>输入要返回的第一个结果的位置。 将它与[!UICONTROL maximum returned results]结合使用，以分页结果</p> <p>示例：如果一次返回100个结果，请输入100以返回结果100-200。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回结果的最大数]</td> 
   <td> <p>在每个方案执行周期中，输入或映射希望模块[action]的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++
