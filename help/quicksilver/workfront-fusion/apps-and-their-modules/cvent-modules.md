---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: 事件模块
description: 在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用Cvent的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 1%

---

# [!DNL Cvent] 模块

在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL Cvent]，并将其连接到多个第三方应用程序和服务。

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

使用 [!DNL Cvent] 模块，您必须具有 [!DNL Cvent] 帐户。

## Connect [!DNL Cvent] 到 [!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>此 [!DNL Cvent] 模块通过 [!UICONTROL SOAP] API。 要创建与的连接 [!DNL Cvent]，您必须确保以下各项：
>
>* 您有 [!UICONTROL SOAP] 访问 [!DNL Cvent] API。
>* 此 [!DNL Workfront Fusion] IP地址已添加到贵组织的允许列表。
>
>  对于列表 [!DNL Workfront Fusion] IP地址，请参见 [用于访问的IP地址 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


您可以创建与 [!DNL Cvent] 直接从 [!DNL Cvent] 模块。

1. 在任意 [!DNL Cvent] 模块，单击 **[!UICONTROL 添加]** 旁边的 [!UICONTROL 连接] 字段。
1. 选择要连接的区域。

   * [!UICONTROL 北美洲]
   * [!UICONTROL 欧洲]
   * [!UICONTROL 沙盒]

1. 单击 **[!UICONTROL 继续]** 以创建连接并返回模块。

## [!DNL Cvent] 模块及其字段

配置时 [!DNL Cvent] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Cvent] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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

通过此操作模块，您可以对 [!DNL Cvent] API。 这样，您就可以创建一个其他人无法实现的数据流自动化 [!DNL Cvent] 模块。

配置此模块时，会显示以下字段。

模块会返回状态代码，以及API调用的标头和正文。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Cvent] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">操作</td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">正文(XML)</td> 
   <td> <p>输入或映射API调用的正文。 必须只包含XML。 模块将自动包含身份验证标头。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 读取记录]

该操作模块读取有关特定记录的信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Cvent] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL记录类型]</p> </td> 
   <td>选择要读取的记录的项目类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL联系人] / [！UICONTROL事件] / [！UICONTROL被邀请者ID]</td> 
   <td> <p>输入或映射要读取的项目的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td> <p>选择要包含在模块输出中的字段。 根据您选择的物料类型，字段可用。</p> </td> 
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
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Cvent] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>被邀请者ID</p> </td> 
   <td> <p>输入或映射要注册事件的被邀请者的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">事件ID</td> 
   <td> <p>输入或映射要为其注册被邀请者的事件ID。</p> </td> 
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
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Cvent] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</p> </td> 
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
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Cvent] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</p> </td> 
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
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Cvent] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</p> </td> 
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
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Cvent] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</p> </td> 
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
   <td> <p>选择要为其输入信息的事件请求字段，然后为这些字段填写所需的值。</p> </td> 
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
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Cvent] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] 到 [!DNL Adobe Workfront Fusion]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL记录类型]</p> </td> 
   <td> <p>选择要列出的记录类型。</p> 
    <ul> 
     <li> <p>来自您的的所有活动 [!DNL Cvent] 帐户</p> </li> 
     <li> <p>事件的所有会话</p> </li> 
     <li> <p>活动的所有被邀请者</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件ID]</td> 
   <td> <p>如果您要列出被邀请人或会话，请输入或映射与这些被邀请人或会话关联的事件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>
