---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: 事件模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用Cvent的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 1%

---

# [!DNL Cvent] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Cvent]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用 [!DNL Cvent] 模块，您必须 [!DNL Cvent] 帐户。

## 连接 [!DNL Cvent] to [!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>的 [!DNL Cvent] 模块通过 [!UICONTROL SOAP] API。 创建连接 [!DNL Cvent]，您必须确保：
>
>* 您拥有 [!UICONTROL SOAP] 对 [!DNL Cvent] API。
>* 的 [!DNL Workfront Fusion] 已将IP地址添加到您组织的允许列表中。
>
>  要获取 [!DNL Workfront Fusion] IP地址，请参阅 [用于访问的IP地址 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


您可以创建与 [!DNL Cvent] 直接从内部帐户 [!DNL Cvent] 模块。

1. 在任意 [!DNL Cvent] 模块，单击 **[!UICONTROL 添加]** 旁边 [!UICONTROL 连接] 字段。
1. 选择要连接的区域。

   * [!UICONTROL 北美洲]
   * [!UICONTROL 欧洲]
   * [!UICONTROL Sandbox]

1. 单击 **[!UICONTROL 继续]** 创建连接，然后返回到模块。

## [!DNL Cvent] 模块及其字段

配置 [!DNL Cvent] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Cvent] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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

通过此操作模块，您可以对 [!DNL Cvent] API。 这样，您就可以创建数据流自动化，而另一个数据流无法实现 [!DNL Cvent] 模块。

配置此模块时，将显示以下字段。

模块会返回状态代码，以及API调用的标头和正文。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Cvent] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">连接 [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">操作</td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">正文(XML)</td> 
   <td> <p>输入或映射API调用的正文。 这必须仅包含XML。 模块将自动包含身份验证标头。 </p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Cvent] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">连接 [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL记录类型]</p> </td> 
   <td>选择要读取的记录的项目类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL联系人] / [!UICONTROL事件] / [!UICONTROL被邀请者ID]</td> 
   <td> <p>输入或映射要读取的项目的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出]</td> 
   <td> <p>选择要包含在模块输出中的字段。 根据您选择的项目类型提供相应的字段。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 注册被邀请者]

此操作模块为事件注册一个被邀请者。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Cvent] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">连接 [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>被邀请者ID</p> </td> 
   <td> <p>输入或映射要为事件注册的被邀请者的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">事件ID</td> 
   <td> <p>输入或映射要为其注册被邀请者的事件的ID。</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Cvent] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">连接 [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL联系人ID]</p> </td> 
   <td> <p>输入或映射要添加到事件的联系人的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL事件ID]</td> 
   <td> <p>输入或映射要将联系人添加到的事件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除联系人]

此操作模块会删除Cvent中的单个联系人。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Cvent] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">连接 [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL联系人ID]</td> 
   <td> <p>输入或映射要删除的联系人的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新联系人]

此操作模块会使用其ID更新现有联系人。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Cvent] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">连接 [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL联系人ID]</p> </td> 
   <td> <p>输入或映射要更新的联系人的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL字段]</td> 
   <td> <p>选择要输入信息的字段，然后为这些字段填写所需的值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL自定义字段]</td> 
   <td> <p>选择要输入信息的字段，然后为这些字段填写所需的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建会议请求]

此操作模块会向您的帐户添加会议请求。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Cvent] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">连接 [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL表单ID]</p> </td> 
   <td> <p>输入或映射用于创建新会议请求的表单的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL会议请求字段]</td> 
   <td> <p>选择要为其输入信息的会议请求字段，然后为这些字段填写所需的值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL事件请求字段]</td> 
   <td> <p>选择要为其输入信息的事件请求字段，然后为这些字段填写所需的值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL RFP请求字段]</td> 
   <td> <p>选择要为其输入信息的建议书字段的请求，然后为这些字段填写所需的值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜索

#### [!UICONTROL 列出记录]

此搜索模块检索有关特定类型的所有记录的信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>有关连接 [!DNL Cvent] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">连接 [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL记录类型]</p> </td> 
   <td> <p>选择要列出的记录类型。</p> 
    <ul> 
     <li> <p>您的 [!DNL Cvent] 帐户</p> </li> 
     <li> <p>事件的所有会话</p> </li> 
     <li> <p>活动的所有被邀请者</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL事件ID]</td> 
   <td> <p>如果列出被邀请者或会话，请输入或映射被邀请者或会话所关联的事件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>
