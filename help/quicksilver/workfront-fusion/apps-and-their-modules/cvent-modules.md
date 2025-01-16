---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Cvent模块
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1111'
ht-degree: 1%

---

# [!DNL Cvent]模块

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [Cvent模块](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/cvent-modules.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

在[!DNL Adobe Workfront Fusion]方案中，您可以自动使用[!DNL Cvent]的工作流，并将其连接到多个第三方应用程序和服务。

如果需要有关创建方案的说明，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中创建方案。

有关模块的信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模块。

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

要使用[!DNL Cvent]模块，您必须具有[!DNL Cvent]帐户。

## Cvent API信息

Cvent连接器使用以下功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API版本</td> 
   <td> V200611.ASMX </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API标记</td> 
   <td>v1.7.14</td> 
  </tr>
 </tbody> 
 </table>

## 将[!DNL Cvent]连接到[!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>[!DNL Cvent]模块通过[!UICONTROL SOAP] API工作。 要创建与[!DNL Cvent]的连接，您必须确保以下各项：
>
>* 您有[!UICONTROL SOAP]访问[!DNL Cvent] API的权限。
>* 列入允许列表 [!DNL Workfront Fusion] IP地址已添加到组织的。
>
>  有关[!DNL Workfront Fusion] IP地址的列表，请参阅[用于访问的IP地址 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


您可以在[!DNL Cvent]模块内直接创建与[!DNL Cvent]帐户的连接。

1. 在任意[!DNL Cvent]模块中，单击[!UICONTROL 连接]字段旁边的&#x200B;**[!UICONTROL 添加]**。
1. 选择要连接的区域。

   * [!UICONTROL 北美]
   * [!UICONTROL 欧洲]
   * [!UICONTROL 沙盒]

1. 单击&#x200B;**[!UICONTROL 继续]**&#x200B;以创建连接并返回模块。

## [!DNL Cvent]模块及其字段

配置[!DNL Cvent]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL Cvent]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)

* [操作](#actions)
* [搜索](#searches)

### 操作

* [[!UICONTROL 自定义API调用]](#create-meeting-request)
* [[!UICONTROL 读取记录]](#read-a-record)
* [[!UICONTROL 注册被邀请者]](#register-invitee)
* [[!UICONTROL 添加被邀请者]](#add-invitee)
* [[!UICONTROL 删除联系人]](#delete-contact)
* [[!UICONTROL 更新联系人]](#update-contact)
* [[!UICONTROL 创建会议请求]](#create-meeting-request)

#### [!UICONTROL 自定义API调用]

此操作模块允许您对[!DNL Cvent] API进行经过身份验证的自定义调用。 这样，您可以创建其他[!DNL Cvent]模块无法实现的数据流自动化。

配置此模块时，会显示以下字段。

模块返回a状态代码，以及API调用的标头和正文。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Cvent]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">将[!DNL Cvent]连接到[!DNL Adobe Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">操作</td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP请求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">正文(XML)</td> 
   <td> <p>输入或映射API调用的正文。 必须只包含XML。 模块将自动包含身份验证标头。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 读取记录]

此操作模块读取有关特定记录的信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Cvent]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">将[!DNL Cvent]连接到[!DNL Adobe Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL记录类型]</p> </td> 
   <td>选择要读取的记录的项目类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL联系人] / [！UICONTROL事件] / [！UICONTROL邀请者ID]</td> 
   <td> <p>输入或映射要读取的项目的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td> <p>选择要包含在模块输出中的字段。 根据您选择的项目类型，字段可用。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 注册被邀请者]

此操作模块为事件注册被邀请者。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Cvent]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">将[!DNL Cvent]连接到[!DNL Adobe Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>被邀请者ID</p> </td> 
   <td> <p>输入或映射要注册事件的被邀请者的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">事件ID</td> 
   <td> <p>输入或映射要为其注册被邀请人的事件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添加被邀请者]

此操作模块邀请联系人参加活动。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Cvent]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">将[!DNL Cvent]连接到[!DNL Adobe Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL联系人ID]</p> </td> 
   <td> <p>输入或映射要添加到事件的联系人ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件ID]</td> 
   <td> <p>输入或映射您要将联系人添加到的事件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除联系人]

此操作模块删除Cvent中的单个联系人。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Cvent]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">将[!DNL Cvent]连接到[!DNL Adobe Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL联系人ID]</td> 
   <td> <p>输入或映射要删除的联系人的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新联系人]

此操作模块使用其ID更新现有联系人。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Cvent]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">将[!DNL Cvent]连接到[!DNL Adobe Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL联系人ID]</p> </td> 
   <td> <p>输入或映射要更新的联系人ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL字段]</td> 
   <td> <p>选择要为其输入信息的字段，然后为这些字段填写所需的值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL自定义字段]</td> 
   <td> <p>选择要为其输入信息的字段，然后为这些字段填写所需的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建会议请求]

此操作模块会将会议请求添加到您的帐户。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Cvent]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">将[!DNL Cvent]连接到[!DNL Adobe Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL表单ID]</p> </td> 
   <td> <p>输入或映射要用于创建新会议请求的表单ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL会议请求字段]</td> 
   <td> <p>选择要为其输入信息的会议请求字段，然后填写这些字段的所需值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件请求字段]</td> 
   <td> <p>选择您要为其输入信息的事件请求字段，然后填写这些字段的所需值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL RFP请求字段]</td> 
   <td> <p>选择要为其输入信息的建议请求字段，然后填写这些字段的所需值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜索

#### [!UICONTROL 列出记录]

此搜索模块可检索有关特定类型的所有记录的信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>有关将[!DNL Cvent]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">将[!DNL Cvent]连接到[!DNL Adobe Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL记录类型]</p> </td> 
   <td> <p>选择要列出的记录类型。</p> 
    <ul> 
     <li> <p>[!DNL Cvent]帐户中的所有事件</p> </li> 
     <li> <p>事件的所有会话</p> </li> 
     <li> <p>某个活动的所有被邀请者</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件ID]</td> 
   <td> <p>如果您要列出被邀请者或会话，请输入或映射与这些被邀请者或会话关联的事件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>
