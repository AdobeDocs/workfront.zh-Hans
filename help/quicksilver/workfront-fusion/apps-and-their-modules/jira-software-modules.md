---
title: Jira软件模块
description: 在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL Jira] 软件，并将其连接到多个第三方应用程序和服务。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2085'
ht-degree: 1%

---

# [!DNL Jira Software] 模块

在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL Jira Software]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

<!-- Bob Fix this compared to original -->

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

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 先决条件

使用 [!DNL Jira] 模块必须具有 [!DNL Jira] 帐户。

## Connect [!DNL Jira Software] 到 [!DNL Workfront Fusion]

您的连接方法基于您是否使用 [!DNL Jira Cloud] 或 [!DNL Jira Server].

* [Connect [!DNL Jira Cloud] 到Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [Connect [!DNL Jira Server] 到 [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### Connect [!DNL Jira Cloud] 到 [!DNL Workfront Fusion]

Connect [!DNL Jira Cloud] 到 [!DNL Workfront Fusion]

连接 [!DNL Jira Software] 到 [!DNL Workfront Fusion]，您必须创建一个API令牌，并将其与服务URL和用户名一起插入到 [!UICONTROL 创建连接] 中的字段 [!DNL Workfront Fusion].

#### 在中创建API令牌 [!DNL Jira]

1. 转到 [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) 并登录。
1. 单击 **[!UICONTROL 创建API令牌]**.
1. 键入令牌的名称，例如 *Workfront Fusion*.
1. 使用复制标记 **[!UICONTROL 复制到剪贴板]** 按钮。

   >[!IMPORTANT]
   >
   >关闭此对话框后，无法再次查看令牌。
1. 将生成的令牌存储在安全位置。
1. 继续使用 [配置 [!DNL Jira] 中的API标记 [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### 配置 [!DNL Jira] 中的API标记 [!DNL Workfront Fusion]

1. In [!DNL Workfront Fusion]，添加 [!DNL Jira] 模块到场景以打开 **[!UICONTROL 创建连接]** 盒子。
1. 指定以下信息：

   * **[!UICONTROL 服务URL]**
   * **[!UICONTROL 用户名]**
   * **[!UICONTROL api令牌]：** 这是您在中创建的API令牌 [在中创建API令牌 [!DNL Jira]](#create-an-api-token-in-jira) 章节。

1. 单击 [!UICONTROL 继续] 以创建连接并返回到模块。

### Connect [!DNL Jira Server] 到 [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

授权以下对象之间的连接： [!DNL Workfront Fusion] 和 [!DNL Jira Server]，您需要消费者密钥、私钥和服务URL。 您可能需要联系 [!DNL Jira] 管理员获取此信息。

* [为您的生成公钥和私钥 [!DNL Jira] 连接](#generate-public-and-private-keys-for-your-jira-connection)
* [将客户端应用程序配置为中的消费者 [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [创建连接 [!DNL Jira] 服务器或Jira数据中心 [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### 为您的生成公钥和私钥 [!DNL Jira] 连接

获取您的私钥 [!DNL Workfront Fusion Jira] 连接，您需要生成公钥和私钥。

1. 在终端中，运行以下命令 `openssl` 命令。

   * `openssl genrsa -out jira_privatekey.pem 1024`

     此命令生成1024位私钥。

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

     此命令创建X509证书。

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

     此命令将私钥（PKCS8格式）提取到 `jira_privatekey.pcks8`
文件。

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

     此命令将公钥从证书提取到 `jira_publickey.pem` 文件。

     >[!NOTE]
     >
     >如果您使用的是Windows，您可能需要将公钥保存到 `jira_publickey.pem` 手动文件：
     >
     >1. 在终端中，运行以下命令：
     >   
     >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
     >   
     >1. 复制终端输出(包括 `-------BEGIN PUBLIC KEY--------` 和 `-------END PUBLIC KEY--------`
     >   
     >1. 将终端输出粘贴到名为的文件中 `jira_publickey.pem`.


1. 继续访问 [将客户端应用程序配置为中的消费者 [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)

#### 将客户端应用程序配置为中的消费者 [!DNL Jira]

1. 登录 [!DNL Jira] 实例。
1. 在左侧导航面板中，单击 **[!UICONTROL [!DNL Jira]设置]** ![](assets/jira-settings-icon.png) > **[!UICONTROL 应用程序]**> **[!UICONTROL 应用程序链接]**.
1. 在 **[!UICONTROL 输入要链接的应用程序的URL]** 字段，输入

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. 单击 **[!UICONTROL 创建新链接]**. 忽略“没有从您输入的URL收到响应”错误消息。
1. 在 **[!UICONTROL 链接应用程序]** 窗口中，输入值 **[!UICONTROL 使用者密钥]** 和 **[!UICONTROL 共享密钥]** 字段。

   您可以选择这些字段的值。

1. 复制 **[!UICONTROL 使用者密钥]** 和 **[!UICONTROL 共享密钥]** 字段到安全位置。

   稍后在配置过程中您将需要这些值。

1. 按如下方式填写URL字段：

   | 字段 | 描述 |
   |---|---|
   | [!UICONTROL 请求令牌URL] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL 授权URL] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL 访问令牌URL] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. 选择 **[!UICONTROL 创建传入链接]** 复选框。
1. 单击 **[!UICONTROL 继续]**.
1. 在 **[!UICONTROL 链接应用程序]** 窗口中，填写以下字段：

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL使用者密钥]</p> </td> 
      <td> 粘贴您复制到安全位置的使用者密钥。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者名称]</td> 
      <td>输入您选择的名称。 此名称供您参考。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL公钥]</td> 
      <td>从您的网站粘贴公钥 <code>[!DNL jira_publickey.pem]</code> 文件。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 继续]**.
1. 继续访问 [创建连接 [!DNL Jira Server] 或 [!DNL Jira Data Center] 在 [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### 创建连接 [!DNL Jira Server] 或 [!DNL Jira Data Center] 在 [!DNL Workfront Fusion]

>[!NOTE]
>
>使用 [!DNL Jira Server] 要连接的应用程序 [!DNL Jira Server] 或 [!DNL Jira Data Center].
1. 在任意 [!DNL Jira Server] 中的模块 [!DNL Workfront Fusion]，单击 **[!UICONTROL 添加]** 旁边的 [!UICONTROL 连接] 字段。
1. 在 [!UICONTROL 创建连接] 面板中，填写以下字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL连接名称]</p> </td> 
      <td> <p>输入连接的名称</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者密钥]</td> 
      <td>粘贴您复制到中安全位置的使用者密钥 <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">将客户端应用程序配置为中的消费者 [!DNL Jira]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>从粘贴私钥 <code>[!DNL jira_privatekey.pcks8]</code> 您在中创建的文件 <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">为您的生成公钥和私钥 [!DNL Jira] 连接</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>输入您的 [!DNL Jira] 实例URL </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 继续]** 以创建连接并返回模块。

## [!DNL Jira Software] 模块及其字段

配置时 [!DNL Jira Software] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Jira Software] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

#### [!UICONTROL 留意记录]

此触发器模块在添加、更新或删除记录时启动方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook]</td> 
   <td> <p>选择要用于监视记录的webhook。 </p> <p>要添加新的webhook，请执行以下操作：</p> 
    <ol> 
     <li value="1">单击 <strong>[！UICONTROL添加]</strong></li> 
     <li value="2">输入webhook的名称。</li> 
     <li value="3"> <p>选择要用于webhook的连接。 </p> <p>有关连接 [!DNL Jira Software] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </li> 
     <li value="4"> <p>选择要软件监视的记录类型：</p> 
      <ul> 
       <li>[！UICONTROL注释] </li> 
       <li>[！UICONTROL问题]</li> 
       <li>[！UICONTROL项目] </li> 
       <li>[！UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 将问题添加到冲刺(sprint)]](#add-issue-to-sprint)
* [[!UICONTROL 自定义API调用]](#custom-api-call)
* [[!UICONTROL 创建记录]](#create-a-record)
* [[!UICONTROL 删除记录]](#delete-a-record)
* [[!UICONTROL 下载附件]](#download-an-attachment)
* [[!UICONTROL 读取记录]](#read-a-record)
* [[!UICONTROL 更新记录]](#update-a-record)

#### [!UICONTROL 将问题添加到冲刺(sprint)]

此操作模块向冲刺添加一个或多个问题。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Jira Software] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Sprint ID]</td> 
   <td>输入或映射要添加问题的冲刺(sprint)的Sprint ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL问题ID或密钥]</td> 
   <td>为要添加到冲刺的每个问题添加问题ID或密钥。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建记录]

此操作模块在Jira中创建新记录。

该模块返回与记录关联的任何标准字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Jira Software] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择您希望模块创建的记录类型。 当您选择记录类型时，特定于该记录类型的其他字段会显示在模块中。</p> 
    <ul> 
     <li>[！UICONTROL附件]</li> 
     <li>[！UICONTROL注释]</li> 
     <li>[！UICONTROL问题]</li> 
     <li>[！UICONTROL项目]</li> 
     <li>[！UICONTROL Sprint] </li> 
     <li>[！UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 自定义API调用]

通过此操作模块，您可以对 [!DNL Jira Software] API。 这样，您就可以创建一个其他人无法实现的数据流自动化 [!DNL Jira Software] 模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Jira Software] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>输入相对路径<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注释:  <p>使用条件语句(例如 <code>if</code> 在JSON中，将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除记录]

此操作模块删除特定记录。

您指定记录的ID。

该模块返回记录的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Jira Software] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择要模块删除的记录类型。 </p> 
    <ul> 
     <li>[！UICONTROL附件]</li> 
     <li>[！UICONTROL注释]</li> 
     <li>[！UICONTROL问题]</li> 
     <li>[！UICONTROL项目]</li> 
     <li>[！UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID或密钥]</td> 
   <td>输入或映射要删除的记录的ID或键。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下载附件]

此操作模块下载特定附件。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Jira Software] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>输入或映射要下载的附件的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 读取记录]

该操作模块从中的单个记录读取数据 [!DNL Jira Software].

您指定记录的ID。

该模块返回与记录关联的任何标准字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Jira Software] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择类型 [!DNL Jira] 您希望模块读取的记录。</p> 
    <ul> 
     <li>[！UICONTROL附件]</li> 
     <li>[！UICONTROL问题]</li> 
     <li>[！UICONTROL项目]</li> 
     <li>[！UICONTROL Sprint] </li> 
     <li>[！UICONTROL用户]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td>选择要接收的输出。 根据“[！UICONTROL记录类型]”字段中选择的记录类型，输出选项可用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td> <p>输入或映射唯一值 [!DNL Jira Software] 您希望模块读取的记录的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新记录]

此操作模块更新现有记录，例如问题或项目。

您指定记录的ID。

该模块返回记录的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Jira Software] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择您希望模块更新的记录类型。 当您选择记录类型时，特定于该记录类型的其他字段会显示在模块中。</p> 
    <ul> 
     <li>[！UICONTROL注释]</li> 
     <li>[！UICONTROL问题]</li> 
     <li>[！UICONTROL项目]</li> 
     <li>[！UICONTROL Sprint] </li> 
     <li>[！UICONTROL过渡问题]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID或密钥]</td> 
   <td>输入或映射要更新的记录的ID或键。</td> 
  </tr> 
 </tbody> 
</table>

### 搜索

* [[!UICONTROL 列出记录]](#list-records)
* [[!UICONTROL 搜索记录]](#search-for-records)

#### [!UICONTROL 列出记录]

此搜索模块可检索与您的搜索查询匹配的特定类型的所有项目

您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Jira Software] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择您希望模块列出的记录类型。 当您选择记录类型时，特定于该记录类型的其他字段会显示在模块中。</p> 
    <ul> 
     <li>[！UICONTROL注释]</li> 
     <li>[！UICONTROL问题]</li> 
     <li>[！UICONTROL项目]</li> 
     <li>[！UICONTROL Sprint问题]</li> 
     <li>[！UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL最大结果]</p> </td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期中检索的最大记录数。</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL 搜索记录]

此搜索模块查找对象中的记录 [!DNL Jira Software] 与指定的搜索查询匹配的用户名称。

您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Jira Software] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择要模块搜索的记录类型。 当您选择记录类型时，特定于该记录类型的其他字段会显示在模块中。</p> 
    <ul> 
     <li>[！UICONTROL问题]</li> 
     <li> <p>[！UICONTROL Issues by JQL （Jira查询语言）] </p> <p>有关JQL的更多信息，请参阅 <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> 在Atlassian帮助站点。 </p> </li> 
     <li>[！UICONTROL项目]</li> 
     <li>[！UICONTROL项目（按问题）]</li> 
     <li>[！UICONTROL用户]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
