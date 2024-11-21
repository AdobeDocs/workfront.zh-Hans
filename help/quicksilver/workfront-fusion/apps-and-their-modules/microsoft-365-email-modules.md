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
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2723'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Email]模块

在[!DNL Adobe Workfront Fusion]方案中，您可以自动使用[!UICONTROL Microsoft Office 365电子邮件]的工作流，并将其连接到多个第三方应用程序和服务。

若要将[!UICONTROL Office 365电子邮件]与[!DNL Adobe Workfront Fusion]一起使用，必须具有[!UICONTROL Office 365帐户]。 您可以在www.office.com创建一个。

有关将[!UICONTROL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅[创建与 [!DNL Adobe Workfront Fusion] 的连接 — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

授予同意后，您将被重定向回[!UICONTROL Workfront Fusion]管理页面，您可以在该页面继续创建场景。

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

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先决条件

要使用[!DNL Microsoft Office 365 Email]模块，您必须具有[!DNL Microsoft Office 365 Email]帐户。

## Microsoft Office 365电子邮件API信息

Microsoft Office 365电子邮件连接器使用以下内容：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基本URL</td> 
   <td> https://graph.microsoft.com/v1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API版本</td> 
   <td> v1.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API标记</td> 
   <td>v2.6.5</td> 
  </tr>
 </tbody> 
 </table>



## 正在将[!DNL Office 365 Email]服务连接到[!DNL Workfront Fusion]

有关将[!DNL Office 365 Email]帐户连接到[!UICONTROL Workfront Fusion]的说明，请参阅[创建与[!UICONTROL Adobe Workfront Fusion]的连接 — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>某些Microsoft应用程序使用相同的连接，该连接与单个用户权限相关联。 因此，在创建连接时，权限同意屏幕除了显示当前应用程序所需的任何新权限外，还会显示以前授予此用户连接的任何权限。
>
>例如，如果用户拥有通过Excel Connector授予的“读取表”权限，然后在Outlook Connector中创建连接以读取电子邮件，则权限同意屏幕将显示已授予的“读取表”权限和新要求的“写入电子邮件”权限。

## [!DNL Microsoft Office 365 Email]模块及其字段

配置[!DNL Microsoft Office 365 Email]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL Microsoft Office 365 Email]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)

* [消息](#message)
* [草稿消息](#draft-message)
* [附件](#attachment)
* [其他](#other)

### 消息

* [[!UICONTROL 创建并发送消息（旧版）]](#create-and-send-a-message)
* [[!UICONTROL 删除邮件]](#delete-a-message)
* [[!UICONTROL 获取消息]](#get-a-message)
* [[!UICONTROL 移动邮件]](#move-a-message)
* [[!UICONTROL 搜索邮件]](#search-messages)
* [[!UICONTROL 观看留言]](#watch-messages)



#### [!UICONTROL 创建并发送消息（旧版）]

创建并发送电子邮件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主题]</td> 
   <td> <p>输入或映射消息的主题行。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL正文内容类型]</td> 
   <td>选择消息正文内容是“HTML”还是“文本”。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL正文内容]</td> 
   <td> <p>输入或映射电子邮件的邮件正文文本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL重要性]</td> 
   <td> <p>选择电子邮件的重要性</p> 
    <ul> 
     <li>[！UICONTROL低]</li> 
     <li>[！UICONTROL正常]</li> 
     <li>[！UICONTROL高]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL到收件人]</p> </td> 
   <td> <p>添加要向其发送消息的电子邮件地址：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[！UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL CC收件人]</p> </td> 
   <td> <p>添加要接收邮件副本的收件人：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[！UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL密件抄送收件人]</p> </td> 
   <td> <p>在邮件中添加要复制的收件人，不允许其他收件人查看其姓名或电子邮件地址：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[！UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL附件]</p> </td> 
   <td> <p>将附件添加到电子邮件：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL文件名]</strong> </p> <p>输入文件名。 示例： <code>sample.doc</code></p> </li> 
     <li> <p><strong>[！UICONTROL数据]</strong> </p> <p>在字段中输入文件数据或映射文件的源。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Internet邮件头]</td> 
   <td> <p>添加电子邮件的邮件头。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名称]</strong> </p> <p>输入标题的名称</p> </li> 
     <li> <p><strong>[！UICONTROL电子邮件地址]</strong> </p> <p>输入题头值。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建并发送消息]

创建并发送电子邮件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主题]</td> 
   <td> <p>输入或映射消息的主题行。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL正文内容类型]</td> 
   <td>选择消息正文内容是“HTML”还是“文本”。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL正文内容]</td> 
   <td> <p>输入或映射电子邮件的邮件正文文本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL重要性]</td> 
   <td> <p>选择电子邮件的重要性</p> 
    <ul> 
     <li>[！UICONTROL低]</li> 
     <li>[！UICONTROL正常]</li> 
     <li>[！UICONTROL高]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL到收件人]</p> </td> 
   <td> <p>添加要向其发送消息的电子邮件地址：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[！UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL CC收件人]</p> </td> 
   <td> <p>添加要接收邮件副本的收件人：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[！UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL密件抄送收件人]</p> </td> 
   <td> <p>在邮件中添加要复制的收件人，不允许其他收件人查看其姓名或电子邮件地址：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[！UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL附件]</p> </td> 
   <td> <p>将附件添加到电子邮件：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL文件名]</strong> </p> <p>输入文件名。 示例： <code>sample.doc</code></p> </li> 
     <li> <p><strong>[！UICONTROL数据]</strong> </p> <p>在字段中输入文件数据或映射文件的源。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Internet邮件头]</td> 
   <td> <p>添加电子邮件的邮件头。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名称]</strong> </p> <p>输入标题的名称</p> </li> 
     <li> <p><strong>[！UICONTROL电子邮件地址]</strong> </p> <p>输入题头值。</p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 要使用共享的电子邮件地址，请在此处输入地址。 其凭据用于此模块的连接中的用户必须有权访问共享文件夹。<p>将此字段留空将使用连接所有者自己的电子邮件地址。</p></p> </td> 
  </tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除邮件]

删除现有电子邮件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 要使用共享的电子邮件地址，请在此处输入地址。 其凭据用于此模块的连接中的用户必须有权访问共享文件夹。<p>将此字段留空将使用连接所有者自己的电子邮件地址。</p></p> </td> 
  </tr> 
   <td role="rowheader">[！UICONTROL消息ID]</td> 
   <td> <p> 选择或映射要删除的消息的ID。</p> </td> 
  </tr> 
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
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 要使用共享的电子邮件地址，请在此处输入地址。 其凭据用于此模块的连接中的用户必须有权访问共享文件夹。<p>将此字段留空将使用连接所有者自己的电子邮件地址。</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL消息ID]</td> 
   <td> <p> 选择或映射要为其检索元数据的消息的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL获取MIME内容]</td> 
   <td>启用此选项以检索有关消息的MIME内容的数据。 [！UICONTROL MIME]内容可能包括图像、音频、视频或其他类型的文件。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移动邮件]

将电子邮件移至邮箱中的选定文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL消息ID]</td> 
   <td> <p> 选择或映射要移动到其他文件夹的邮件ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL邮件文件夹] </td> 
   <td> <p>选择或映射要将邮件移动到的文件夹的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索邮件]

根据特定条件搜索消息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 要使用共享的电子邮件地址，请在此处输入地址。 其凭据用于此模块的连接中的用户必须有权访问共享文件夹。<p>将此字段留空将使用连接所有者自己的电子邮件地址。</p></p> </td> 
  </tr> 
<tr> 
   <td role="rowheader">[！UICONTROL邮件文件夹]</td> 
   <td> <p>选择包含要搜索邮件的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜索]</td> 
   <td>输入您的搜索查询。 有关如何编写搜索查询的信息，请参阅[!DNL Microsoft]支持文章<a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">在[!DNL Outlook.com]</a>中搜索邮件和人员。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Order by]</td> 
   <td> <p>选择要对结果进行排序的方式：</p> 
    <ul> 
     <li>[！UICONTROL主题（升序或降序）]</li> 
     <li>[！UICONTROL创建日期时间（升序或降序）]</li> 
     <li>[！UICONTROL上次修改日期时间（升序或降序）]</li> 
     <li>[！UICONTROL收到日期时间（升序或降序）]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入在一个方案执行周期内应返回的最大邮件数[!DNL Workfront Fusion]。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看留言]

发送或接收新电子邮件时触发。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL监视消息]</p> </td> 
   <td> <p>选择要监视的消息：</p> 
    <ul> 
     <li>[！UICONTROL Only Unread]</li> 
     <li>[！UICONTROL只读read]</li> 
     <li>[！UICONTROL All]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL邮件文件夹]</td> 
   <td> <p>选择包含要监视的邮件的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜索]</td> 
   <td>输入您的搜索查询。 有关如何编写搜索查询的信息，请参阅[!DNL Microsoft]支持文章<a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">在[!DNL Outlook.com]</a>中搜索邮件和人员。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>输入在一个方案执行周期内应返回的最大邮件数[!DNL Workfront Fusion]。</p> </td> 
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
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主题]</td> 
   <td> <p>输入消息的主题行。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL正文内容类型]</td> 
   <td>选择消息正文内容是“HTML”还是“文本”。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL正文内容]</td> 
   <td> <p>输入电子邮件的邮件正文文本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL重要性]</td> 
   <td> <p>选择电子邮件的重要性</p> 
    <ul> 
     <li>[！UICONTROL低]</li> 
     <li>[！UICONTROL正常]</li> 
     <li>[！UICONTROL高]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL到收件人]</p> </td> 
   <td> <p>添加要向其发送消息的收件人：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[！UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL CC收件人]</p> </td> 
   <td> <p>添加收件人您希望接收邮件的副本：</p> 
    <ul> 
     <li> <p><strong>名称</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>电子邮件地址</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>密件抄送收件人</p> </td> 
   <td> <p>在邮件中添加要复制的收件人，不允许其他收件人查看其姓名或电子邮件地址：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[！UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL附件]</p> </td> 
   <td> <p>将附件添加到电子邮件：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL文件名]</strong> </p> <p>输入文件名。 示例： <code>sample.doc</code></p> </li> 
     <li> <p><strong>[！UICONTROL数据]</strong> </p> <p>在字段中输入文件数据或映射文件的源。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 要使用共享的电子邮件地址，请在此处输入地址。 其凭据用于此模块的连接中的用户必须有权访问共享文件夹。<p>将此字段留空将使用连接所有者自己的电子邮件地址。</p></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 发送草稿邮件]

发送当前处于草稿状态的电子邮件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 要使用共享的电子邮件地址，请在此处输入地址。 其凭据用于此模块的连接中的用户必须有权访问共享文件夹。<p>将此字段留空将使用连接所有者自己的电子邮件地址。</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL草稿消息ID]</td> 
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
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 要使用共享的电子邮件地址，请在此处输入地址。 其凭据用于此模块的连接中的用户必须有权访问共享文件夹。<p>将此字段留空将使用连接所有者自己的电子邮件地址。</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入消息ID]</td> 
   <td> <p>选择要如何标识要更新的消息：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手动输入]</strong> </p> <p>输入或映射消息ID。</p> </li> 
     <li> <p><strong>[！UICONTROL从列表中选择]</strong> </p> <p>选择包含要更新的邮件的文件夹，然后选择邮件</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主题]</td> 
   <td> <p>输入消息的主题行。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL正文内容]</td> 
   <td> <p>输入电子邮件的邮件正文文本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL重要性]</td> 
   <td> <p>选择电子邮件的重要性</p> 
    <ul> 
     <li>[！UICONTROL低]</li> 
     <li>[！UICONTROL正常]</li> 
     <li>[！UICONTROL高]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL到收件人]</p> </td> 
   <td> <p>添加要向其发送消息的电子邮件地址：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[！UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL CC收件人]</p> </td> 
   <td> <p>添加收件人您希望接收邮件的副本：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[！UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL密件抄送收件人]</p> </td> 
   <td> <p>在邮件中添加要复制的收件人，不允许其他收件人查看其姓名或电子邮件地址：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名称]</strong> </p> <p>输入联系人的姓名</p> </li> 
     <li> <p><strong>[！UICONTROL电子邮件地址]</strong> </p> <p>输入联系人的电子邮件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL附件]</p> </td> 
   <td> <p>将附件添加到电子邮件：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL文件名]</strong> </p> <p>输入文件名。 示例： <code>sample.doc</code></p> </li> 
     <li> <p><strong>[！UICONTROL数据]</strong> </p> <p>在字段中输入文件数据或映射文件的源。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL将其标记为已读]</td> 
   <td>启用此选项可将更新的邮件标记为已读。</td> 
  </tr> 
 </tbody> 
</table>

### 附件

* [[!UICONTROL 下载附件]](#download-an-attachment)
* [[!UICONTROL 列出附件]](#list-attachments)

#### [!UICONTROL 下载附件]

此模块下载指定的附件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 要使用共享的电子邮件地址，请在此处输入地址。 其凭据用于此模块的连接中的用户必须有权访问共享文件夹。<p>将此字段留空将使用连接所有者自己的电子邮件地址。</p></p> </td> 
  </tr> 
   <td role="rowheader">[！UICONTROL消息ID]</td> 
   <td> <p> 选择或映射包含要下载附件的邮件的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL附件ID]</td> 
   <td> <p>输入或映射要下载的附件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出附件]

此模块检索属于指定邮件的附件列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 要使用共享的电子邮件地址，请在此处输入地址。 其凭据用于此模块的连接中的用户必须有权访问共享文件夹。<p>将此字段留空将使用连接所有者自己的电子邮件地址。</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL消息ID]</td> 
   <td> <p> 选择或映射要从中检索附件的邮件的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射每个方案执行周期中您希望模块返回的最大附件数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

* [[!UICONTROL 添加附件]](#add-an-attachment)
  <!--Create and send a message-->
* [[!UICONTROL 进行API调用]](#make-an-api-call)

#### [!UICONTROL 添加附件]

此模块向邮件添加大型附件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 要使用共享的电子邮件地址，请在此处输入地址。 其凭据用于此模块的连接中的用户必须有权访问共享文件夹。<p>将此字段留空将使用连接所有者自己的电子邮件地址。</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL消息ID]</td> 
   <td> <p> 选择或映射要添加附件的邮件的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source file]</td> 
   <td> <p>从上一个模块中选择一个文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 进行API调用]

此模块允许您执行自定义API调用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Office 365]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>输入相对于<code>https://graph.microsoft.com</code>的路径。 示例：<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP请求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。例如，<code>{"Content-type":"application/json"}</code>。 [!DNL Workfront Fusion]为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p> 以标准JSON对象的形式添加API调用的查询。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：  <p>在JSON中使用条件语句（如<code>if</code>）时，请将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
