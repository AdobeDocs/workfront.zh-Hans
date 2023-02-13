---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Microsoft Office 365电子邮件
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用Microsoft Office 365电子邮件的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1838'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Email]

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!UICONTROL Microsoft Office 365电子邮件]，并将其连接到多个第三方应用程序和服务。

为了使用 [!UICONTROL Office 365电子邮件] with [!DNL Adobe Workfront Fusion]，则需要具有 [!UICONTROL Office 365帐户]. 您可以在www.office.com上创建一个。

有关连接 [!UICONTROL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 [创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

在您同意后，系统会将您重定向回 [!UICONTROL Workfront Fusion] 管理页面，您可以在该页面中继续创建方案。

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

使用 [!DNL Microsoft Office 365 Email] 模块，您必须 [!DNL Microsoft Office 365 Email] 帐户。

## [!DNL Microsoft Office 365 Email] 模块及其字段

配置 [!DNL Microsoft Office 365 Email] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Microsoft Office 365 Email] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [消息](#message)
* [草稿消息](#draft-message)
* [附件](#attachment)
* [其他](#other)

### 消息

* [[!UICONTROL 观看消息]](#watch-messages)
* [[!UICONTROL 搜索消息]](#search-messages)
* [[!UICONTROL 获取消息]](#get-a-message)
* [[!UICONTROL 创建和发送消息]](#create-and-send-a-message)
* [[!UICONTROL 移动消息]](#move-a-message)
* [[!UICONTROL 删除消息]](#delete-a-message)

#### [!UICONTROL 观看消息]

发送或接收新电子邮件时触发。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Watch Messages]</p> </td> 
   <td> <p>选择要观看的消息：</p> 
    <ul> 
     <li>[!UICONTROL仅未读]</li> 
     <li>[!UICONTROL只读]</li> 
     <li>[!UICONTROL All]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder]</td> 
   <td> <p>选择包含要监视的消息的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索]</td> 
   <td>输入搜索查询。 有关如何编写搜索查询的信息，请参阅 [!DNL Microsoft] 支持文章 <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">在中搜索邮件和人员 [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td> <p>输入消息的最大数量 [!DNL Workfront Fusion] 应在一个方案执行周期中返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索消息]

根据特定条件搜索消息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder]</td> 
   <td> <p>选择包含要搜索的消息的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索]</td> 
   <td>输入搜索查询。 有关如何编写搜索查询的信息，请参阅 [!DNL Microsoft] 支持文章 <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">在中搜索邮件和人员 [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td> <p>选择对结果排序的方式：</p> 
    <ul> 
     <li>[!UICONTROL主题（升序或降序）]</li> 
     <li>[!UICONTROL创建日期时间（升序或降序）]</li> 
     <li>[!UICONTROL上次修改日期时间（升序或降序）]</li> 
     <li>[!UICONTROL接收的日期时间（升序或降序）]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>输入消息的最大数量 [!DNL Workfront Fusion] 应在一个方案执行周期中返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取消息]

获取特定消息的元数据

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL消息ID]</td> 
   <td> <p> 选择或映射要为其检索元数据的消息的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL获取MIME内容]</td> 
   <td>启用此选项可检索有关消息MIME内容的数据。 [!UICONTROL MIME]内容可能包含图像、音频、视频或其他类型的文件。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建和发送消息]

创建并发送电子邮件消息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主题]</td> 
   <td> <p>输入或映射消息的主题行。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>选择消息的正文内容是HTML还是文本。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体内容]</td> 
   <td> <p>输入或映射电子邮件的邮件正文文本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL重要性]</td> 
   <td> <p>选择电子邮件的重要性</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL到收件人]</p> </td> 
   <td> <p>添加要将消息发送到的电子邮件地址：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[!UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC收件人]</p> </td> 
   <td> <p>添加要接收消息副本的收件人：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[!UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL密送收件人]</p> </td> 
   <td> <p>添加您要在邮件中复制的收件人，而不允许其他收件人查看其姓名或电子邮件地址：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[!UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL附件]</p> </td> 
   <td> <p>将附件添加到电子邮件：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL文件名]</strong> </p> <p>输入文件名。 示例: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL数据]</strong> </p> <p>在字段中输入文件数据或映射文件的源。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Internet消息标头]</td> 
   <td> <p>为电子邮件添加消息标头。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名称]</strong> </p> <p>输入标题的名称</p> </li> 
     <li> <p><strong>[!UICONTROL电子邮件地址]</strong> </p> <p>输入标题的值。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移动消息]

将电子邮件移至邮箱中的选定文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL消息ID]</td> 
   <td> <p> 选择或映射要移动到其他文件夹的消息的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder] </td> 
   <td> <p>选择或映射要移动消息的文件夹的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除消息]

删除现有电子邮件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL消息ID]</td> 
   <td> <p> 选择或映射要删除的消息的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 草稿消息

* [创建草稿消息](#create-a-draft-message)
* [发送草稿消息](#send-a-draft-message)
* [更新消息](#update-a-message)

#### [!UICONTROL 创建草稿消息]

创建新电子邮件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主题]</td> 
   <td> <p>输入消息的主题行。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>选择消息的正文内容是HTML还是文本。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体内容]</td> 
   <td> <p>输入电子邮件的邮件正文文本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL重要性]</td> 
   <td> <p>选择电子邮件的重要性</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL到收件人]</p> </td> 
   <td> <p>添加要将消息发送到的收件人：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[!UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC收件人]</p> </td> 
   <td> <p>添加收件人要接收消息副本：</p> 
    <ul> 
     <li> <p><strong>名称</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>电子邮件地址</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>密送收件人</p> </td> 
   <td> <p>添加您要在邮件中复制的收件人，而不允许其他收件人查看其姓名或电子邮件地址：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[!UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL附件]</p> </td> 
   <td> <p>将附件添加到电子邮件：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL文件名]</strong> </p> <p>输入文件名。 示例: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL数据]</strong> </p> <p>在字段中输入文件数据或映射文件的源。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 发送草稿消息]

发送当前处于草稿状态的电子邮件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL草稿消息ID]</td> 
   <td> <p> 选择或映射要发送的草稿的消息ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新消息]

更新现有消息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输入消息ID]</td> 
   <td> <p>选择要标识要更新消息的方式：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手动输入]</strong> </p> <p>输入或映射消息ID。</p> </li> 
     <li> <p><strong>[!UICONTROL从列表中选择]</strong> </p> <p>选择包含要更新的消息的文件夹，然后选择该消息</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主题]</td> 
   <td> <p>输入消息的主题行。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体内容]</td> 
   <td> <p>输入电子邮件的邮件正文文本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL重要性]</td> 
   <td> <p>选择电子邮件的重要性</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL到收件人]</p> </td> 
   <td> <p>添加要将消息发送到的电子邮件地址：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[!UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC收件人]</p> </td> 
   <td> <p>添加收件人要接收消息副本：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[!UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL密送收件人]</p> </td> 
   <td> <p>添加您要在邮件中复制的收件人，而不允许其他收件人查看其姓名或电子邮件地址：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[!UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL附件]</p> </td> 
   <td> <p>将附件添加到电子邮件：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL文件名]</strong> </p> <p>输入文件名。 示例: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL数据]</strong> </p> <p>在字段中输入文件数据或映射文件的源。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL将其标记为已读]</td> 
   <td>启用此选项可将更新的消息标记为已读。</td> 
  </tr> 
 </tbody> 
</table>

### 附件

* [[!UICONTROL 列出附件]](#list-attachments)
* [[!UICONTROL 下载附件]](#download-an-attachment)

#### [!UICONTROL 列出附件]

此模块检索属于指定消息的附件列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL消息ID]</td> 
   <td> <p> 选择或映射要从中检索附件的消息的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大附件数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下载附件]

此模块下载指定的附件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL消息ID]</td> 
   <td> <p> 选择或映射包含要下载的附件的消息的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL附件ID]</td> 
   <td> <p>输入或映射要下载的附件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

* [[!UICONTROL 进行API调用]](#make-an-api-call)
* [[!UICONTROL 添加附件]](#add-an-attachment)

#### [!UICONTROL 进行API调用]

此模块允许您执行自定义API调用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>输入相对于 <code>https://graph.microsoft.com</code>. 示例:<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL方法]</p> </td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。例如， <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询字符串]</td> 
   <td> <p> 以标准JSON对象的形式添加API调用的查询。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。</p> <p>注释:  <p>使用条件语句时，例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添加附件]

此模块会向消息添加大附件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Office 365] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL消息ID]</td> 
   <td> <p> 选择或映射要添加附件的消息的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择一个文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>
