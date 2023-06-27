---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Gmail模块
description: 在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用Gmail的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1833'
ht-degree: 0%

---

# [!DNL Gmail] 模块

在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL Gmail]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). 有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用 [!DNL Gmail] 模块，您必须具有 [!DNL Gmail] 帐户。

## Connect [!DNL Gmail] 到 [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [Connect [!DNL Gmail] 到 [!DNL Workfront Fusion] 使用[！DNL G Suite]](#connect-gmail-to-workfront-fusion-usingg-suite)
* [Connect [!DNL Gmail] 到 [!DNL Workfront Fusion] 使用 [!DNL gmail.com] 或 [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### Connect [!DNL Gmail] 到 [!DNL Workfront Fusion] 使用[!DNL  G Suite] {#connect-gmail-to-workfront-fusion-using-g-suite}

有关连接 [!DNL G Suite] 目标帐户 [!UICONTROL Workfront Fusion]，请参见 [将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) 在文章中 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Connect [!DNL Gmail] 到 [!DNL Workfront Fusion] 使用 [!DNL gmail.com] 或 [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

如果您是 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 您必须在以下位置创建OAuth客户端的用户 [此 [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 为了获得 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密码].

有关如何创建OAuth客户端并获取 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密码]，请参见 [使用自定义OAuth客户端将Adobe Workfront Fusion连接到Google Services](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## [!DNL Gmail] 模块及其字段

配置时 [!DNL Gmail] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Gmail] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [迭代器](#iterators)

### 触发器

#### [!UICONTROL 观看电子邮件]

此触发器模块在收到要处理的新电子邮件时执行场景。

该模块返回与一个或多个记录关联的所有标准字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] 到[！UICONTROL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择要监视的电子邮件文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL筛选器类型] </td> 
   <td> <p>选择要用于观看电子邮件的过滤器类型</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL简单筛选器]</strong> </p> <p>填写[！UICONTROL标准]、[！UICONTROL发件人电子邮件地址]、[！UICONTROL主题]和[！UICONTROL搜索短语]字段</p> </li> 
     <li> <p> <strong>[！UICONTROL Gmail筛选器]</strong> </p> <p>在[！UICONTROL Query]字段中，输入要用于筛选电子邮件的查询。</p> <p>有关的详细信息 [!DNL Gmail] 过滤器，请参阅 <a href="https://support.google.com/mail/answer/7190">搜索运算符</a> 在 [!DNL Gmail] 文档。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL标准]</td> 
   <td>选择是要观看[！UICONTROL所有电子邮件]、[！UICONTROL仅读取电子邮件]还是[！UICONTROL仅读取未读]电子邮件。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL发件人电子邮件地址]</td> 
   <td> <p> 输入电子邮件地址，以便仅观看从该地址发送的电子邮件。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL主题]</td> 
   <td>输入文本字符串以仅观看主题中带有该文本字符串的电子邮件。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜索短语]</td> 
   <td>输入一个文本字符串，以仅观看电子邮件中任何位置包含该文本字符串的电子邮件。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL在获取时将电子邮件标记为已读]</td> 
   <td> <p> 启用此选项可将检索到的电子邮件标记为已读。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最大结果数]</td> 
   <td> <p> 设置满足以下条件的最大结果数 [!DNL Workfront Fusion] 在一个周期内使用。</p> </td> 
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
* [[!UICONTROL 修改电子邮件标签]](#modify-email-labels)

#### [!UICONTROL 发送电子邮件]

该操作模块会发送一封新电子邮件。

您可以指定电子邮件的收件人。

该模块会返回电子邮件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] 到 [!DNL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL From]</td> 
   <td> <p>输入或映射发件人电子邮件地址。</p> <p>注意：如果输入的电子邮件地址不正确，则在发送邮件时可能会发生错误，因为您的帐户可能无权从不同于您自己的地址发送电子邮件。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL至] </td> 
   <td> <p>单击 <strong>[！UICONTROL添加]</strong>，然后输入或映射每个收件人的电子邮件地址。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL主题] </td> 
   <td> <p>输入或映射电子邮件主题。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL内容] </td> 
   <td> <p>输入或映射电子邮件内容（邮件正文）。 允许使用HTML标记。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL附件] </td> 
   <td> <p>单击 <strong>[！UICONTROL添加]</strong> 以添加附件。 您可以从以前的模块映射文件。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL复制收件人]</td> 
   <td> <p> 单击 <strong>[！UICONTROL添加]</strong>，然后输入或映射每个副本收件人的电子邮件地址。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL密件副本收件人]</td> 
   <td> <p> 单击 <strong>[！UICONTROL添加]</strong>，然后输入或映射每个密件副本收件人的电子邮件地址。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建草稿]

此操作模块会创建新的电子邮件草稿，并将其添加到您指定的文件夹中。

指定要在其中创建草稿的文件夹。

该模块会返回电子邮件草稿的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] 到[！UICONTROL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择 [!DNL Gmail] 要在其中创建草绘的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL至] </td> 
   <td> <p>单击 <strong>[！UICONTROL添加]</strong>，然后输入或映射每个收件人的电子邮件地址。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL主题] </td> 
   <td> <p>输入或映射电子邮件主题。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL内容] </td> 
   <td> <p>输入或映射电子邮件内容（邮件正文）。 允许使用HTML标记。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL附件] </td> 
   <td> <p>单击 <strong>[！UICONTROL添加]</strong> 以添加附件。 您可以从以前的模块映射文件。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL复制收件人]</td> 
   <td> <p> 单击 <strong>[！UICONTROL添加]</strong>，然后输入或映射每个副本收件人的电子邮件地址。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL密件副本收件人]</td> 
   <td> <p> 单击 <strong>[！UICONTROL添加]</strong>，然后输入或映射每个密件副本收件人的电子邮件地址。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将电子邮件标记为已读]

此操作模块将电子邮件标记为已读。

您可以指定电子邮件及其文件夹的ID。

该模块会返回电子邮件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] 到[！UICONTROL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择 [!DNL Gmail] 包含电子邮件的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL电子邮件ID (UID)]</td> 
   <td> <p> 输入或映射电子邮件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将电子邮件标记为未读]

此操作模块将电子邮件或电子邮件草稿标记为未读。

您可以指定电子邮件及其文件夹的ID。

该模块会返回电子邮件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] 到[！UICONTROL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择 [!DNL Gmail] 包含电子邮件的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL电子邮件ID (UID)] </td> 
   <td> <p>输入或映射要标记为未读的电子邮件的电子邮件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移动电子邮件]

此操作模块会将电子邮件或电子邮件草稿移动到您指定的文件夹。

您可以指定文件夹、目标文件夹和电子邮件的ID。

该模块会返回电子邮件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] 到[！UICONTROL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择 [!DNL Gmail] 包含要移动的电子邮件的源文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目标文件夹]</td> 
   <td> <p> 选择 [!DNL Gmail] 要将电子邮件移动到的目标文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL电子邮件ID (UID)]</td> 
   <td> <p> 输入或映射要移动的电子邮件的电子邮件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 复制电子邮件]

此操作模块会将电子邮件或电子邮件草稿复制到您指定的文件夹中。

您可以指定文件夹、目标文件夹和电子邮件的ID。

该模块会返回电子邮件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] 到[！UICONTROL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择 [!DNL Gmail] 包含要复制的电子邮件的源文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目标文件夹]</td> 
   <td> <p>选择 [!DNL Gmail] 要将电子邮件复制到的目标文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL电子邮件ID (UID)]</td> 
   <td> <p>输入或映射要复制的电子邮件的电子邮件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除电子邮件]

此操作模块会从您指定的文件夹中删除电子邮件或电子邮件草稿。

该模块会返回电子邮件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] 到[！UICONTROL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL [!DNL Gmail] 消息ID</p> </td> 
   <td> <p>输入或映射要删除的电子邮件的电子邮件ID。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL永久] </td> 
   <td> <p>启用此选项可允许模块永久删除电子邮件，而不是将其移至垃圾桶文件夹。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 修改电子邮件标签]

此操作模块可修改您指定的电子邮件上的标签。

该模块会返回电子邮件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] 到[！UICONTROL Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL [!DNL Gmail] 消息ID</td> 
   <td> <p> 输入或映射要删除的电子邮件的电子邮件ID。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>要添加的[！UICONTROL标签]</p> </td> 
   <td> <p>选择或映射您要添加到所选电子邮件的标签。</p> </td> 
  </tr> 
  <tr> 
   <td>要移除的[！UICONTROL标签]</td> 
   <td> <p> 选择或映射要从所选电子邮件中删除的标签。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>[!UICONTROL 添加标签] 和 [!UICONTROL 要移除的标签] 字段仅加载用户创建的标签。

### 迭代器

#### [!UICONTROL 迭代附件]

您可以迭代电子邮件附件。 每个附件都是模块输出中的一个单独捆绑包。 有关更多信息，请参阅 [Adobe Workfront Fusion中的迭代器模块](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL源模块] </td> 
   <td> <p>选择要从中迭代处理附件的模块。 </p> </td> 
  </tr> 
 </tbody> 
</table>
