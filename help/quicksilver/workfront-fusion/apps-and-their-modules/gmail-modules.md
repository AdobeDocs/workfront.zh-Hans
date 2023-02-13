---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Gmail模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用Gmail的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1785'
ht-degree: 0%

---

# [!DNL Gmail] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Gmail]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). 有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用 [!DNL Gmail] 模块，您必须 [!DNL Gmail] 帐户。

## 连接 [!DNL Gmail] to [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [连接 [!DNL Gmail] to [!DNL Workfront Fusion] 使用[!DNL G Suite]](#connect-gmail-to-workfront-fusion-usingg-suite)
* [连接 [!DNL Gmail] to [!DNL Workfront Fusion] 使用 [!DNL gmail.com] 或 [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### 连接 [!DNL Gmail] to [!DNL Workfront Fusion] 使用[!DNL  G Suite] {#connect-gmail-to-workfront-fusion-using-g-suite}

有关连接 [!DNL G Suite] 帐户 [!UICONTROL Workfront Fusion]，请参阅 [将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) 在文章中 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### 连接 [!DNL Gmail] to [!DNL Workfront Fusion] 使用 [!DNL gmail.com] 或 [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

如果您 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 用户，必须在 [the [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 为了获得 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密钥].

有关如何创建OAuth客户端并获取 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密钥]，请参阅 [使用自定义OAuth客户端将Adobe Workfront Fusion连接到Google Services](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## [!DNL Gmail] 模块及其字段

配置 [!DNL Gmail] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Gmail] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [迭代器](#iterators)

### 触发器

#### [!UICONTROL 观看电子邮件]

此触发器模块会在收到要处理的新电子邮件时执行方案。

模块会返回与记录或记录关联的所有标准字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">连接 [!DNL Gmail] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>选择要监视的电子邮件文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL过滤器类型] </td> 
   <td> <p>选择要用于观看电子邮件的过滤器类型</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Simple Filter]</strong> </p> <p>填写[!UICONTROL标准]、[!UICONTROL发件人电子邮件地址]、[!UICONTROL主题]和[!UICONTROL搜索短语]字段</p> </li> 
     <li> <p> <strong>[!UICONTROL Gmail过滤器]</strong> </p> <p>在[!UICONTROL查询]字段中，输入要用于筛选电子邮件的查询。</p> <p>有关 [!DNL Gmail] 过滤器，请参阅 <a href="https://support.google.com/mail/answer/7190">搜索运算符</a> 在 [!DNL Gmail] 文档。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL标准]</td> 
   <td>选择您是要观看[!UICONTROL all email]、[!UICONTROL only read emails]还是[!UICONTROL only unread]电子邮件。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL发件人电子邮件地址]</td> 
   <td> <p> 输入电子邮件地址以仅观看从该地址发送的电子邮件。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL主题]</td> 
   <td>输入文本字符串，以仅观看在主题中包含该文本字符串的电子邮件。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL搜索短语]</td> 
   <td>输入文本字符串，以仅观看在电子邮件中任意位置具有该文本字符串的电子邮件。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL将电子邮件标记为已读，获取时]</td> 
   <td> <p> 启用此选项可将检索到的电子邮件标记为已读。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL最大结果数]</td> 
   <td> <p> 设置 [!DNL Workfront Fusion] 可在一个周期内使用。</p> </td> 
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

此操作模块会发送一封新电子邮件。

您可以指定电子邮件的收件人。

模块会返回电子邮件和任何关联字段的ID，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">连接 [!DNL Gmail] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL From]</td> 
   <td> <p>输入或映射发件人电子邮件地址。</p> <p>注意：如果您输入的电子邮件地址不正确，则在发送消息时可能会出错，因为您的帐户可能没有从您自己的地址以外的地址发送电子邮件的权限。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL至] </td> 
   <td> <p>单击 <strong>[!UICONTROL Add]</strong>，然后输入或映射每个收件人的电子邮件地址。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL主题] </td> 
   <td> <p>输入或映射电子邮件主题。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL内容] </td> 
   <td> <p>输入或映射电子邮件内容（消息正文）。 允许使用HTML标记。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL附件] </td> 
   <td> <p>单击 <strong>[!UICONTROL Add]</strong> 添加附件。 您可以映射来自先前模块的文件。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL复制收件人]</td> 
   <td> <p> 单击 <strong>[!UICONTROL Add]</strong>，然后输入或映射每个复制收件人的电子邮件地址。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL盲文收件人]</td> 
   <td> <p> 单击 <strong>[!UICONTROL Add]</strong>，然后输入或映射每个盲副本收件人的电子邮件地址。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建草稿]

此操作模块会创建新的电子邮件草稿，并将其添加到您指定的文件夹。

您可以指定要创建草稿的文件夹。

模块会返回电子邮件草稿和任何关联字段的ID，以及连接访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">连接 [!DNL Gmail] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>选择 [!DNL Gmail] 要在中创建草稿的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL至] </td> 
   <td> <p>单击 <strong>[!UICONTROL Add]</strong>，然后输入或映射每个收件人的电子邮件地址。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL主题] </td> 
   <td> <p>输入或映射电子邮件主题。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL内容] </td> 
   <td> <p>输入或映射电子邮件内容（消息正文）。 允许使用HTML标记。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL附件] </td> 
   <td> <p>单击 <strong>[!UICONTROL Add]</strong> 添加附件。 您可以映射来自先前模块的文件。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL复制收件人]</td> 
   <td> <p> 单击 <strong>[!UICONTROL Add]</strong>，然后输入或映射每个复制收件人的电子邮件地址。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL盲文收件人]</td> 
   <td> <p> 单击 <strong>[!UICONTROL Add]</strong>，然后输入或映射每个盲副本收件人的电子邮件地址。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将电子邮件标记为已读]

此操作模块将电子邮件标记为已读。

您可以指定电子邮件及其文件夹的ID。

模块会返回电子邮件和任何关联字段的ID，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">连接 [!DNL Gmail] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>选择 [!DNL Gmail] 包含电子邮件的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL电子邮件ID(UID)]</td> 
   <td> <p> 输入或映射电子邮件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将电子邮件标记为未读]

此操作模块将电子邮件或电子邮件草稿标记为未读。

您可以指定电子邮件及其文件夹的ID。

模块会返回电子邮件和任何关联字段的ID，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">连接 [!DNL Gmail] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>选择 [!DNL Gmail] 包含电子邮件的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL电子邮件ID(UID)] </td> 
   <td> <p>输入或映射要标记为未读的电子邮件的电子邮件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移动电子邮件]

此操作模块会将电子邮件或电子邮件草稿移至您指定的文件夹。

您可以指定文件夹、目标文件夹和电子邮件的ID。

模块会返回电子邮件和任何关联字段的ID，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">连接 [!DNL Gmail] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>选择 [!DNL Gmail] 包含要移动的电子邮件的源文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL目标文件夹]</td> 
   <td> <p> 选择 [!DNL Gmail] 目标文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL电子邮件ID(UID)]</td> 
   <td> <p> 输入或映射要移动的电子邮件的电子邮件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 复制电子邮件]

此操作模块将电子邮件或电子邮件草稿复制到您指定的文件夹中。

您可以指定文件夹、目标文件夹和电子邮件的ID。

模块会返回电子邮件和任何关联字段的ID，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">连接 [!DNL Gmail] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>选择 [!DNL Gmail] 包含要复制的电子邮件的源文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL目标文件夹]</td> 
   <td> <p>选择 [!DNL Gmail] 目标文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL电子邮件ID(UID)]</td> 
   <td> <p>输入或映射要复制的电子邮件的电子邮件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除电子邮件]

此操作模块会从您指定的文件夹中删除电子邮件或电子邮件草稿。

模块会返回电子邮件和任何关联字段的ID，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">连接 [!DNL Gmail] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL [!DNL Gmail] 消息ID]</p> </td> 
   <td> <p>输入或映射您要删除的电子邮件的电子邮件ID。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permently] </td> 
   <td> <p>启用此选项，以允许模块永久删除电子邮件，而不是将其移动到垃圾桶文件夹。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 修改电子邮件标签]

此操作模块修改您指定的电子邮件上的标签。

模块会返回电子邮件和任何关联字段的ID，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Gmail] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">连接 [!DNL Gmail] 到[!UICONTROL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Gmail] 消息ID]</td> 
   <td> <p> 输入或映射您要删除的电子邮件的电子邮件ID。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！要添加的UICONTROL标签]</p> </td> 
   <td> <p>选择或映射要添加到选定电子邮件的标签。</p> </td> 
  </tr> 
  <tr> 
   <td>[！要删除的UICONTROL标签]</td> 
   <td> <p> 选择或映射要从选定电子邮件中删除的标签。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>[!UICONTROL 要添加的标签] 和 [!UICONTROL 要删除的标签] 字段仅加载用户创建的标签。

### 迭代器

#### [!UICONTROL 迭代附件]

您可以迭代电子邮件附件。 每个附件是模块输出中的一个单独捆绑包。 有关更多信息，请参阅 [Adobe Workfront Fusion中的迭代器模块](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL源模块] </td> 
   <td> <p>选择要从中迭代附件的模块。 </p> </td> 
  </tr> 
 </tbody> 
</table>
