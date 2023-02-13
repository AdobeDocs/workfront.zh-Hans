---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: 电子邮件模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以将电子邮件帐户连接到多个第三方应用程序和服务。这允许您通过IMAP下载电子邮件、通过SMTP发送电子邮件、创建新草稿、将电子邮件从一个文件夹移动并复制到另一个文件夹、将电子邮件标记为已读或未读，以及删除电子邮件。
author: Becky
feature: Workfront Fusion
exl-id: 384ba60a-d79e-4126-a247-6d67b5154ede
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2613'
ht-degree: 0%

---

# 电子邮件模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以将电子邮件帐户连接到多个第三方应用程序和服务。这允许您通过IMAP下载电子邮件、通过SMTP发送电子邮件、创建新草稿、将电子邮件从一个文件夹移动并复制到另一个文件夹、将电子邮件标记为已读或未读，以及删除电子邮件。

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

## 将电子邮件连接到Workfront Fusion {#connect-your-email-to-workfront-fusion}

* [连接到Google](#connect-to-google)
* [连接到其他电子邮件服务(SMAP)](#connect-to-other-email-services-smap)

### 连接到 [!DNL Google]

使用此选项，可创建包含电子邮件模块且需要与 [!DNL Google] 帐户。 这是一个有受限范围的帐户。

您可以创建与 [!DNL Google] 帐户。

1. 在任意电子邮件模块中，单击 **[!UICONTROL 添加]** 旁边 [!UICONTROL 连接] 字段。
1. 选择 **[!DNL Google]** 作为连接类型。
1. 输入连接的名称。
1. （可选）输入 [!UICONTROL [!DNL Google] 客户端ID] 和 [!UICONTROL 客户端密钥].
1. 单击 **[!UICONTROL 继续]** 创建连接，然后返回到模块。

### 连接到其他电子邮件服务(SMAP)

SMAP连接允许您远程访问邮箱，并读取或处理邮箱中的邮件。 大多数电子邮件模块都使用SMAP连接。

1. 在任意电子邮件模块中，单击 **[!UICONTROL 添加]** 旁边 [!UICONTROL 连接] 字段。
1. 选择 **[!UICONTROL 其他(SMTP)]** 作为连接类型。
1. 输入 **[!UICONTROL 名称]** 的URL。
1. 选择 **[!UICONTROL 电子邮件提供商]** 列表。 如果您的电子邮件提供商不在列表中，请选择其他。
1. 输入 **[!UICONTROL 电子邮件地址]**, **[!UICONTROL 您的全名]**，您的 **[!UICONTROL 用户名]**&#x200B;和 **[!UICONTROL 密码]**.
1. （视情况而定）如果您的提供商不在列表中，请输入 **[!UICONTROL SMTP服务器]** 和 **[!UICONTROL 端口]**，并指定是否 **[!UICONTROL 使用安全连接(TLS)]**. 要查找此信息，请查看 [!UICONTROL 帮助] 的区域。 如果您没有此信息可用，请联系您的电子邮件服务提供商。
1. 单击 **[!UICONTROL 继续]** 创建连接，然后返回到模块。

## [!UICONTROL 电子邮件] 模块及其字段

配置 [!UICONTROL 电子邮件] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 此外，还可能显示其他字段，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

某些电子邮件字段可能已包含数据，因为您在方案的其他模块中使用了它们。 如果您需要有关电子邮件帮助的信息，请参阅电子邮件帮助文档。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>唯一电子邮件ID，称为“[!UICONTROL 电子邮件ID(UID)]&#39;是电子邮件的标识符。 电子邮件ID是特定于每个电子邮件文件夹的。

* [触发器](#triggers)
* [操作](#actions)
* [迭代器](#iterators)

### 触发器

#### [!UICONTROL 观看电子邮件]

收到新电子邮件以根据指定的条件进行处理时触发。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关将您的电子邮件帐户连接到[!UICONTROL Workfront Fusion]的说明，请参阅 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">将您的电子邮件连接到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件夹] </td> 
   <td> <p>选择包含要监视的电子邮件的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL标准]</p> </td> 
   <td> <p>选择您要通过哪个标准来观看电子邮件：</p> 
    <ul> 
     <li>[!UICONTROL所有电子邮件]</li> 
     <li>[!UICONTROL仅读电子邮件]</li> 
     <li>[!UICONTROL仅未读电子邮件]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL发件人电子邮件地址] </td> 
   <td> <p>输入要监视其电子邮件的发件人的电子邮件地址。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL收件人电子邮件地址]</td> 
   <td> <p> 输入要观看其电子邮件的收件人的电子邮件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主题] </td> 
   <td> <p>输入您要观看的电子邮件的主题。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL短语] </td> 
   <td> <p>输入任何关键词，以仅观看包含特定短语的电子邮件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL将消息标记为读取时]</td> 
   <td> <p>启用此选项，可在检索详细信息后将未读电子邮件标记为已读。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL最大结果数]</td> 
   <td> <p> 电子邮件的最大数量 [!DNL Workfront Fusion] 应在一个方案执行周期中返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 发送电子邮件]](#send-an-email)
* [[!UICONTROL 创建草稿]](#create-a-draft)
* [[!UICONTROL 将电子邮件标记为已读]](#mark-an-email-as-read)
* [[!UICONTROL 将电子邮件标记为未读]](#mark-an-email-as-unread)
* [[!UICONTROL 移动电子邮件]](#move-an-email)
* [[!UICONTROL 复制电子邮件]](#copy-an-email)
* [[!UICONTROL 删除电子邮件]](#delete-an-email)
* [[!UICONTROL 获取电子邮件]](#get-emails)
* [[!UICONTROL 给我发送电子邮件]](#send-me-an-email)

#### [!UICONTROL 发送电子邮件]

发送新电子邮件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关将您的电子邮件帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">将您的电子邮件连接到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL发送后保存消息]</td> 
   <td>发送电子邮件后，该邮件将保存在您的邮箱中。 如果要保存使用 [!DNL Workfront Fusion] 到 <i>[!UICONTROL已发送邮件]</i> 文件夹或邮箱中的其他文件夹。 一些电子邮件服务，例如 [!DNL Gmail]，自动保存已发送的消息。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL至] </td> 
   <td> <p>添加要将电子邮件发送到的电子邮件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主题] </td> 
   <td> <p>输入或映射电子邮件的主题行。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL内容类型]</p> </td> 
   <td> <p>为电子邮件选择[!UICONTROL content]类型：</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Plaintext]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL内容] </td> 
   <td> <p>使用HTML标记或纯文本以HTML格式输入或映射电子邮件内容，具体取决于您在[!UICONTROL内容类型]字段中选择的内容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL附件]</p> </td> 
   <td> <p>添加附件：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL文件名]</strong> </p> <p>输入文件名。 例如，sample.doc。</p> </li> 
     <li> <p><strong>[!UICONTROL数据]</strong> </p> <p>输入上传附件的文件夹路径。</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>输入[!UICONTROL内容ID]以在内容中插入附件（图像）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy Recipient] </td> 
   <td> <p>输入或映射要向其发送此电子邮件副本的一个或多个电子邮件地址。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Blind Copy收件人]</td> 
   <td> <p> 输入或映射一个或多个要向其发送此电子邮件副本的电子邮件地址，而不会在电子邮件中显示此电子邮件地址。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL From] </td> 
   <td> <p>输入或映射电子邮件[!UICONTROL From]字段中显示的电子邮件地址(和名称（如果需要）)。 </p> <p>重要信息：使用正确的语法： <code>name@email.com</code> 或 <code>"Name" name@email.com</code>.</p> <p>注意：通常， [!DNL Workfront Fusion] 使用您在创建连接时输入的电子邮件地址作为发件人地址。 如果您输入任何其他电子邮件地址，则在发送消息时可能会出错，因为您的帐户可能没有从您自己的地址以外的其他地址发送电子邮件的权限。 例如 <code>test@mail.com</code> 或"<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>输入或映射电子邮件中[!UICONTROL Sender]字段中显示的电子邮件地址。</p> <p>提示：如果不确定是使用此字段还是“发件人”字段，我们建议选择“发件人”字段。</p> <p>重要信息：使用正确的语法： <code>name@email.com</code> 或 <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reply-To]</td> 
   <td> <p> 如果您希望将此电子邮件的回复发送到与“发件人”地址不同的地址，请输入您希望回复此电子邮件的电子邮件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL In-Reply-To]</td> 
   <td> <p> 如果您回复的是特定电子邮件，请输入或映射您回复的电子邮件的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL引用] </td> 
   <td> <p>输入线程中所有回复的消息ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL优先级]</p> </td> 
   <td> <p>选择电子邮件的优先级：</p> 
    <ul> 
     <li>[!UICONTROL High]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Low]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL标头]</p> </td> 
   <td> <p>添加标头：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL密钥]</strong> </p> <p>添加密钥。 例如，[!UICONTROL Sender]、[!UICONTROL Date]、[!UICONTROL To]等。</p> </li> 
     <li> <p><strong>[!UICONTROL值]</strong> </p> <p>输入键值。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建草稿]

创建新草稿并将其添加到选定文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关将您的电子邮件帐户连接到[!UICONTROL Workfront Fusion]的说明，请参阅 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">将您的电子邮件连接到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件夹]</td> 
   <td>选择要在其中创建草稿电子邮件的文件夹。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL至] </td> 
   <td> <p>输入或映射要将电子邮件发送到的电子邮件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主题] </td> 
   <td> <p>输入或映射电子邮件的主题行。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL内容类型]</p> </td> 
   <td> <p>为电子邮件选择内容类型：</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL纯文本]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL内容] </td> 
   <td> <p>使用HTML标记或纯文本以HTML格式输入或映射电子邮件内容，具体取决于您在[!UICONTROL内容类型]字段中选择的内容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL附件]</p> </td> 
   <td> <p>添加附件：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL文件名]</strong> </p> <p>输入文件名。 例如，sample.doc。</p> </li> 
     <li> <p><strong>[!UICONTROL数据]</strong> </p> <p>输入上传附件的文件夹路径。</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>输入内容ID以在内容中插入附件（图像）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy Recipient] </td> 
   <td> <p>输入或映射要向其发送此电子邮件副本的一个或多个电子邮件地址。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Blind Copy收件人]</td> 
   <td> <p> 输入或映射一个或多个要向其发送此电子邮件副本的电子邮件地址，而不会在电子邮件中显示此电子邮件地址。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL From] </td> 
   <td> <p>输入或映射电子邮件[!UICONTROL From]字段中显示的电子邮件地址(和名称（如果需要）)。 </p> <p>重要信息：使用正确的语法： <code>name@email.com</code> 或 <code>"Name" name@email.com</code>.</p> <p>注意：通常， [!DNL Workfront Fusion] 使用您在创建连接时输入的电子邮件地址作为发件人地址。 如果您输入任何其他电子邮件地址，则在发送消息时可能会出错，因为您的帐户可能没有从您自己的地址以外的其他地址发送电子邮件的权限。 例如 <code>test@mail.com</code> 或"<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>输入或映射电子邮件中[!UICONTROL Sender]字段中显示的电子邮件地址。</p> <p>提示：如果不确定是使用此字段还是“发件人”字段，我们建议选择“发件人”字段。</p> <p>重要信息：使用正确的语法： <code>name@email.com</code> 或 <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Reply-To]</td> 
   <td> <p> 如果您希望将此电子邮件的回复发送到与“[!UICONTROL from]”地址不同的地址，请输入要在其中回复此电子邮件的电子邮件地址。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL In-Reply-To]</td> 
   <td> <p> 如果您回复的是特定电子邮件，请输入或映射您回复的电子邮件的ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL引用] </td> 
   <td> <p>输入线程中所有回复的消息ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL优先级]</p> </td> 
   <td> <p>选择电子邮件的优先级：</p> 
    <ul> 
     <li>[!UICONTROL High]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Low]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL标头]</p> </td> 
   <td> <p>添加标头：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL密钥]</strong> </p> <p>添加密钥。 例如，“发件人”、“日期”、“收件人”等。</p> </li> 
     <li> <p><strong>[!UICONTROL值]</strong> </p> <p>输入键值。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将电子邮件标记为已读]

通过将 [!UICONTROL 读取] 标记。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关将您的电子邮件帐户连接到[!UICONTROL Workfront Fusion]的说明，请参阅 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">将您的电子邮件连接到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件夹]</td> 
   <td>选择要标记为已读的电子邮件的文件夹。 示例：主要。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL电子邮件ID(UID)]</p> </td> 
   <td> <p>输入要标记为已读的电子邮件的电子邮件UID。</p> <p>您可以使用[!UICONTROL Email] &gt;[!UICONTROL Watch Email]模块或[!UICONTROL Search Email]模块获取电子邮件的UID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将电子邮件标记为未读]

通过设置“未读”标记，将选定文件夹中的电子邮件或草稿标记为未读。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关将您的电子邮件帐户连接到[!UICONTROL Workfront Fusion]的说明，请参阅 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">将您的电子邮件连接到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件夹]</td> 
   <td>选择要标记为未读的电子邮件的文件夹。 示例：主要。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL电子邮件ID(UID)]</p> </td> 
   <td> <p>输入要标记为未读的电子邮件的电子邮件UID。</p> <p>您可以使用[!UICONTROL Email] &gt;[!UICONTROL Watch Email]模块或[!UICONTROL Search Email]模块获取电子邮件的UID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移动电子邮件]

将选定的电子邮件或草稿移动到选定的文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关将您的电子邮件帐户连接到[!UICONTROL Workfront Fusion]的说明，请参阅 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">将您的电子邮件连接到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件夹]</td> 
   <td>选择包含要从中移动电子邮件的电子邮件的文件夹。 示例：主要。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL目标文件夹]</td> 
   <td> <p> 选择要将电子邮件添加到的文件夹。 示例：工作。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL电子邮件ID(UID)]</p> </td> 
   <td> <p>输入要移动到目标文件夹的电子邮件的电子邮件UID。</p> <p>您可以使用[!UICONTROL Email] &gt;[!UICONTROL Watch Email]模块或[!UICONTROL Search Email]模块获取电子邮件的UID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 复制电子邮件]

将电子邮件或草稿复制到选定的文件夹中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关将您的电子邮件帐户连接到[!UICONTROL Workfront Fusion]的说明，请参阅 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">将您的电子邮件连接到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件夹]</td> 
   <td>选择要从中复制电子邮件的文件夹。 示例：主要。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL目标文件夹]</td> 
   <td> <p> 选择要将电子邮件复制到的文件夹。 示例：工作。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL电子邮件ID(UID)]</p> </td> 
   <td> <p>输入要复制到目标文件夹的电子邮件的电子邮件UID。</p> <p>您可以使用[!UICONTROL Email] &gt;[!UICONTROL Watch Email]模块或[!UICONTROL Search Email]模块获取电子邮件的UID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除电子邮件]

从选定文件夹中删除电子邮件或草稿。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关将您的电子邮件帐户连接到[!UICONTROL Workfront Fusion]的说明，请参阅 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">将您的电子邮件连接到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件夹]</td> 
   <td>选择要删除的电子邮件的文件夹。 示例：主要。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL电子邮件ID(UID)]</p> </td> 
   <td> <p>输入要删除的电子邮件的电子邮件UID。</p> <p>您可以使用[!UICONTROL Email] &gt;[!UICONTROL Watch Email]模块或[!UICONTROL Search Email]模块获取电子邮件的UID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL扩展]</td> 
   <td> <p>启用此选项，以允许模块永久删除当前打开的邮箱中标记为[!UICONTROL Deleted]的所有邮件。</p> <p>注意：在 [!DNL Gmail]，此行为由[!UICONTROL设置] &gt;[!UICONTROL转发POP/IMAP（在IMAP访问中）部分中的设置驱动。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取电子邮件]

返回与指定条件匹配的电子邮件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关将您的电子邮件帐户连接到[!UICONTROL Workfront Fusion]的说明，请参阅 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">将您的电子邮件连接到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件夹] </td> 
   <td> <p>选择包含要检索的电子邮件的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL将消息标记为读取时] </td> 
   <td> <p>如果要在检索详细信息后将未读电子邮件标记为已读，请启用此选项。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL标准]</p> </td> 
   <td> <p>选择要检索的电子邮件的标准：</p> 
    <ul> 
     <li>[!UICONTROL所有电子邮件]</li> 
     <li>[!UICONTROL仅读电子邮件]</li> 
     <li>[!UICONTROL仅未读电子邮件]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL发件人电子邮件地址] </td> 
   <td> <p>输入或映射要检索其电子邮件的发件人的电子邮件地址。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL收件人电子邮件地址]</td> 
   <td> <p> 输入或映射要检索其电子邮件的收件人的电子邮件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL开始日期] </td> 
   <td> <p>输入或映射日期以检索在指定日期或之后处理的电子邮件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Before date]</td> 
   <td> <p> 输入或映射日期以检索在指定日期或之前处理的电子邮件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主题] </td> 
   <td> <p>输入或映射要检索的电子邮件的主题。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL短语] </td> 
   <td> <p>输入或映射任何关键词以仅检索包含特定短语的电子邮件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL电子邮件ID(UID)]</td> 
   <td> <p> 输入要检索其详细信息的电子邮件的电子邮件ID(UID)。</p> <p>您可以使用 [!DNL Workfront Fusion]“s[!UICONTROL Watch Email]”模块或“[!UICONTROL Search Email]”模块。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL最大结果数]</td> 
   <td> <p> 电子邮件的最大数量 [!DNL Workfront Fusion] 应在一个方案执行周期中返回。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL即使模块未返回任何结果，仍继续执行路由]</td> 
   <td> <p> 选择是否要继续运行模块，即使没有返回任何结果。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 给我发送电子邮件]

向您的电子邮件地址发送新电子邮件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL主题] </td> 
   <td> <p>输入或映射电子邮件的主题行。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL内容] </td> 
   <td> <p>输入电子邮件的正文。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 迭代器

#### [!UICONTROL 迭代附件]

迭代会逐个接收附件。

电子邮件迭代器模块允许您单独管理电子邮件附件。 例如，您可以设置为观看电子邮件，以循环访问带有附件的电子邮件并接收警报。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源模块]</td> 
   <td> <p>选择输出包含要迭代的附件的电子邮件的模块。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关迭代器的更多信息，请参阅 [中的迭代器模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
