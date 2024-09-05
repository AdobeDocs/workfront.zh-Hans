---
title: Jira软件模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Jira] 软件的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 3abfa92e6ad33243a1cdd19de25bbe04a8e81425
workflow-type: tm+mt
source-wordcount: '2087'
ht-degree: 1%

---

# [!DNL Jira Software]模块

在[!DNL Adobe Workfront Fusion]方案中，您可以自动使用[!DNL Jira Software]的工作流，并将其连接到多个第三方应用程序和服务。

如果需要有关创建方案的说明，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中创建方案。

有关模块的信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模块。

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
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 先决条件

要使用[!DNL Jira]模块，您必须具有[!DNL Jira]帐户。

## 将[!DNL Jira Software]连接到[!DNL Workfront Fusion]

您的连接方法基于您使用的是[!DNL Jira Cloud]还是[!DNL Jira Server]。

* [连接 [!DNL Jira Cloud] 到Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [连接 [!DNL Jira Server] 到 [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### 将[!DNL Jira Cloud]连接到[!DNL Workfront Fusion]

将[!DNL Jira Cloud]连接到[!DNL Workfront Fusion]

要将[!DNL Jira Software]连接到[!DNL Workfront Fusion]，您必须创建一个API令牌，并将其与您的服务URL和用户名一起插入到[!DNL Workfront Fusion]中的[!UICONTROL 创建连接]字段。

#### 在[!DNL Jira]中创建API令牌

1. 转到[https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens)并登录。
1. 单击&#x200B;**[!UICONTROL 创建API令牌]**。
1. 键入令牌的名称，如&#x200B;*Workfront Fusion*。
1. 使用&#x200B;**[!UICONTROL 复制到剪贴板]**&#x200B;按钮复制令牌。

   >[!IMPORTANT]
   >
   >关闭此对话框后，无法再次查看令牌。
1. 将生成的令牌存储在安全位置。
1. 继续[在 [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion)中配置 [!DNL Jira] API令牌。

#### 在[!DNL Workfront Fusion]中配置[!DNL Jira] API令牌

1. 在[!DNL Workfront Fusion]中，将[!DNL Jira]模块添加到方案以打开&#x200B;**[!UICONTROL 创建连接]**&#x200B;框。
1. 指定以下信息：

   * **[!UICONTROL 服务URL]：**&#x200B;这是用于访问Jira帐户的基本URL。 示例： `yourorganization.atlassian.net`
   * **[!UICONTROL 用户名]**
   * **[!UICONTROL API令牌]：**&#x200B;这是您在[在此文章的 [!DNL Jira]](#create-an-api-token-in-jira)部分中创建API令牌的API令牌。

1. 单击[!UICONTROL 继续]以创建连接并返回模块。

### 将[!DNL Jira Server]连接到[!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

要授权[!DNL Workfront Fusion]与[!DNL Jira Server]之间的连接，您需要消费者密钥、私钥和服务URL。 您可能需要联系[!DNL Jira]管理员以获取此信息。

* [为 [!DNL Jira] 连接生成公钥和私钥](#generate-public-and-private-keys-for-your-jira-connection)
* [将客户端应用程序配置为 [!DNL Jira]中的消费者](#configure-the-client-app-as-a-consumer-in-jira)
* [创建与 [!DNL Workfront Fusion]中的 [!DNL Jira] 服务器或Jira数据中心的连接](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### 为您的[!DNL Jira]连接生成公钥和私钥

要获取[!DNL Workfront Fusion Jira]连接的私钥，您需要生成公钥和私钥。

1. 在终端中，运行以下`openssl`命令。

   * `openssl genrsa -out jira_privatekey.pem 1024`

     此命令生成1024位私钥。

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

     此命令创建X509证书。

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

     此命令将私钥（PKCS8格式）提取到`jira_privatekey.pcks8`
文件。

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

     此命令将公钥从证书提取到`jira_publickey.pem`文件。

     >[!NOTE]
     >
     >如果您使用的是Windows，您可能需要手动将公钥保存到`jira_publickey.pem`文件：
     >
     >1. 在终端中，运行以下命令：
     >   
     >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
     >   
     >1. 复制终端输出（包括`-------BEGIN PUBLIC KEY--------`和`-------END PUBLIC KEY--------`）
     >   
     >1. 将终端输出粘贴到名为`jira_publickey.pem`的文件中。


1. 继续[将客户端应用程序配置为 [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)中的消费者

#### 在[!DNL Jira]中将客户端应用配置为消费者

1. 登录到您的[!DNL Jira]实例。
1. 在左侧导航面板中，单击&#x200B;**[!UICONTROL [!DNL Jira]设置]** ![](assets/jira-settings-icon.png) > **[!UICONTROL 应用程序]**> **[!UICONTROL 应用程序链接]**。
1. 在&#x200B;**[!UICONTROL 输入要链接的应用程序的URL]**&#x200B;字段中，输入

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. 单击&#x200B;**[!UICONTROL 新建链接]**。 忽略“No received from the URL you entered（从输入的URL未收到任何响应）”错误消息。
1. 在&#x200B;**[!UICONTROL 链接应用程序]**&#x200B;窗口中，在&#x200B;**[!UICONTROL 使用者密钥]**&#x200B;和&#x200B;**[!UICONTROL 共享密钥]**&#x200B;字段中输入值。

   您可以选择这些字段的值。

1. 将&#x200B;**[!UICONTROL 使用者密钥]**&#x200B;和&#x200B;**[!UICONTROL 共享密钥]**&#x200B;字段的值复制到安全位置。

   在配置过程的后续步骤中，您将需要这些值。

1. 按如下方式填写URL字段：

   | 字段 | 描述 |
   |---|---|
   | [!UICONTROL 请求令牌URL] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL 授权URL] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL 访问令牌URL] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. 选中&#x200B;**[!UICONTROL 创建传入链接]**&#x200B;复选框。
1. 单击&#x200B;**[!UICONTROL 继续]**。
1. 在&#x200B;**[!UICONTROL 链接应用程序]**&#x200B;窗口中，填写以下字段：

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL使用者密钥]</p> </td> 
      <td> 将您复制的使用者密钥粘贴到安全位置。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者名称]</td> 
      <td>输入您选择的名称。 此名称供您参考。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL公钥]</td> 
      <td>从<code>[!DNL jira_publickey.pem]</code>文件中粘贴公钥。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**[!UICONTROL 继续]**。
1. 继续[在 [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)中创建与 [!DNL Jira Server] 或 [!DNL Jira Data Center] 的连接

#### 在[!DNL Workfront Fusion]中创建与[!DNL Jira Server]或[!DNL Jira Data Center]的连接

>[!NOTE]
>
>使用[!DNL Jira Server]应用连接到[!DNL Jira Server]或[!DNL Jira Data Center]。
1. 在[!DNL Workfront Fusion]中的任何[!DNL Jira Server]模块中，单击[!UICONTROL 连接]字段旁边的&#x200B;**[!UICONTROL 添加]**。
1. 在[!UICONTROL 创建连接]面板中，填写以下字段：

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
      <td>将您复制的使用者密钥粘贴到<a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">中的安全位置在[!DNL Jira]</a>中将客户端应用程序配置为使用者</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>粘贴您在<a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">中为[!DNL Jira]连接</a>生成公钥和私钥的<code>[!DNL jira_privatekey.pcks8]</code>文件中的私钥。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>输入您的[!DNL Jira]实例URL。 示例： <code>yourorganization.atlassian.net</code></td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**[!UICONTROL 继续]**&#x200B;以创建连接并返回模块。

## [!DNL Jira Software]模块及其字段

配置[!DNL Jira Software]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL Jira Software]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

#### [!UICONTROL 观看记录]

此触发器模块在添加、更新或删除记录时启动方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook]</td> 
   <td> <p>选择要用于监视记录的webhook。 </p> <p>要添加新的webhook，请执行以下操作：</p> 
    <ol> 
     <li value="1">单击<strong>[！UICONTROL添加]</strong></li> 
     <li value="2">输入webhook的名称。</li> 
     <li value="3"> <p>选择要用于webhook的连接。 </p> <p>有关将[!DNL Jira Software]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">将[!DNL Jira Software]连接到[!DNL Workfront Fusion]</a>。</p> </li> 
     <li value="4"> <p>选择要软件监视的记录类型：</p> 
      <ul> 
       <li>[！UICONTROL Comment] </li> 
       <li>[！UICONTROL问题]</li> 
       <li>[！UICONTROL项目] </li> 
       <li>[！UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 将问题添加到冲刺]](#add-issue-to-sprint)
* [[!UICONTROL 创建记录]](#create-a-record)
* [[!UICONTROL 自定义API调用]](#custom-api-call)
* [[!UICONTROL 删除记录]](#delete-a-record)
* [[!UICONTROL 下载附件]](#download-an-attachment)
* [[!UICONTROL 读取记录]](#read-a-record)
* [[!UICONTROL 更新记录]](#update-a-record)

#### [!UICONTROL 将问题添加到冲刺]

此操作模块向冲刺添加一个或多个问题。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Jira Software]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">将[!DNL Jira Software]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
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

该模块会返回与记录关联的任何标准字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Jira Software]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">将[!DNL Jira Software]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择要模块创建的记录类型。 选择记录类型后，该记录类型特有的其他字段将显示在模块中。</p> 
    <ul> 
     <li>[！UICONTROL附件]</li> 
     <li>[！UICONTROL Comment]</li> 
     <li>[！UICONTROL问题]</li> 
     <li>[！UICONTROL项目]</li> 
     <li>[！UICONTROL Sprint] </li> 
     <li>[！UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 自定义API调用]

此操作模块允许您对[!DNL Jira Software] API进行经过身份验证的自定义调用。 这样，您可以创建其他[!DNL Jira Software]模块无法实现的数据流自动化。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Jira Software]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">将[!DNL Jira Software]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>输入相对路径<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP请求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：  <p>在JSON中使用条件语句（如<code>if</code>）时，请将引号放在条件语句之外。</p> 
     <img src="assets/quotes-in-json-350x120.png">  </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除记录]

此操作模块删除特定记录。

您指定记录的ID。

该模块返回记录ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Jira Software]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">将[!DNL Jira Software]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择要模块删除的记录类型。 </p> 
    <ul> 
     <li>[！UICONTROL附件]</li> 
     <li>[！UICONTROL Comment]</li> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Jira Software]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">将[!DNL Jira Software]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>输入或映射要下载的附件的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 读取记录]

此操作模块从[!DNL Jira Software]中的单个记录读取数据。

您指定记录的ID。

该模块会返回与记录关联的任何标准字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Jira Software]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">将[!DNL Jira Software]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择要模块读取的[!DNL Jira]记录的类型。</p> 
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
   <td> <p>输入或映射您希望模块读取的记录的唯一[!DNL Jira Software] ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新记录]

此操作模块更新现有记录，如问题或项目。

您指定记录的ID。

该模块返回记录ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Jira Software]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">将[!DNL Jira Software]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择您希望模块更新的记录类型。 选择记录类型后，该记录类型特有的其他字段将显示在模块中。</p> 
    <ul> 
     <li>[！UICONTROL Comment]</li> 
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

您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Jira Software]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">将[!DNL Jira Software]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择您希望模块列出的记录类型。 选择记录类型后，该记录类型特有的其他字段将显示在模块中。</p> 
    <ul> 
     <li>[！UICONTROL Comment]</li> 
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

此搜索模块在[!DNL Jira Software]中查找与您指定的搜索查询匹配的对象中的记录。

您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Jira Software]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">将[!DNL Jira Software]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择要模块搜索的记录类型。 选择记录类型后，该记录类型特有的其他字段将显示在模块中。</p> 
    <ul> 
     <li>[！UICONTROL Issues]</li> 
     <li> <p>[！UICONTROL Issues by JQL （Jira查询语言）] </p> <p>有关JQL的详细信息，请参阅Atlassian帮助网站上的<a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a>。 </p> </li> 
     <li>[！UICONTROL项目]</li> 
     <li>[！UICONTROL项目（按问题）</li> 
     <li>[！UICONTROL用户]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
