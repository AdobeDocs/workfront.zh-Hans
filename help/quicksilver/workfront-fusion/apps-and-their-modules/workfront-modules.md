---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Adobe Workfront模块
description: 您可以使用Adobe Workfront Fusion Adobe Workfront连接器在Workfront中自动执行流程。 如果您拥有Workfront Fusion for Work Automation and Integration许可证，则还可以使用它连接到第三方应用程序和服务。
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: b84d2d41-a983-4ea3-b331-0302bfcf8a2b
source-git-commit: 2682c027b2cd248b2674cebe8f0a0b8d1006257b
workflow-type: tm+mt
source-wordcount: '6797'
ht-degree: 2%

---

# [!DNL Adobe Workfront]模块

您可以使用[!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront]连接器自动执行[!DNL Workfront]中的流程。 如果您拥有[!UICONTROL [!DNL Workfront Fusion]工作自动化和集成]许可证，则还可以使用它连接到第三方应用程序和服务。

[!DNL Workfront]连接器不计入您的组织可用的活动应用程序数量。 所有方案，即使它们仅使用[!DNL Workfront]应用程序，也会计入贵组织的方案总数。

有关您组织的可用应用和方案的详细信息，请参阅[[!DNL Adobe Workfront Fusion] 组织和团队](../../workfront-fusion/organizations/organizations-and-teams.md)中的[组织](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2)。

如果需要有关创建方案的说明，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中创建方案。 有关模块的信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模块。

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
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## 将[!DNL Workfront]连接到[!DNL Workfront Fusion]

[!DNL Workfront]连接器使用OAuth 2.0连接到[!DNL Workfront]。

您可以在[!DNL Workfront Fusion]模块内直接创建与[!DNL Workfront]帐户的连接。

1. 在任意Adobe Workfront模块中，单击连接字段旁边的&#x200B;**添加**。
1. 填写以下字段：

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[！UICONTROL连接名称]</td>
        <td>
          <p>输入新连接的名称。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL环境]</td>
        <td>
          <p>选择是连接到生产环境还是非生产环境。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL连接类型]</td>
        <td>
          <p>选择您是要连接到服务帐户还是个人帐户。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL客户端ID]</td>
        <td>输入您的[!DNL Workfront]客户端ID。 您可以在Workfront中“设置”区域的“OAuth2应用程序”区域找到此代码。 打开要连接的特定应用程序以查看客户端ID。</td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL客户端密钥]</td>
        <td>输入您的[!DNL Workfront]客户端ID。 您可以在Workfront中“设置”区域的“OAuth2应用程序”区域找到此代码。 打开要连接的特定应用程序以查看客户端ID。</td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL身份验证URL]</td>
        <td>此值可保留为默认值，也可以输入Workfront实例的URL，后跟<code>/integrations/oauth2</code>。 <p>示例： <code>https://mydomain.my.workfront.com/integrations/oauth2</code></p></td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL主机前缀]</td>
        <td>在大多数情况下，此值应为<code>origin</code>。
      </tr>
    </tbody>
    </table>

1. 单击&#x200B;**[!UICONTROL 继续]**&#x200B;保存连接并返回模块。




<!--1. Enter the name of your instance into the URL. Example: `https://<your instance>.my.workfront.com`.
1. Click **[!UICONTROL Next]**.
1. Click **[!UICONTROL SAML log in]** to create the connection and go back to the module.

   Or

   Enter your Username and Password, then click **[!UICONTROL Log in]** to create the connection and go back to the module.-->

>[!NOTE]
>
>* 如果您没有看到SAML登录按钮，则表明贵组织未启用单点登录(SSO)。 您可以使用用户名和密码登录。
>   
>   有关SSO的详细信息，请参阅[单点登录概述 [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
>   
>* 到[!DNL Workfront] API的OAuth 2.0连接不再依赖API密钥。
>* 要创建与Workfront沙盒环境的连接，您必须在该环境中创建一个OAuth2应用程序，然后在您的连接中使用由该应用程序生成的客户端ID和客户端密钥。
>
>   有关在Workfront中创建OAuth2应用程序的说明，请参阅为Workfront集成创建OAuth2应用程序一文中的[使用用户凭据创建OAuth2应用程序（授权代码流）](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow)。

## [!DNL Workfront]模块及其字段

配置[!DNL Workfront]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL Workfront]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。


![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>* 如果您在Workfront模块中未看到最新字段，这可能是因为缓存问题。 等待一小时，然后重试。
>* 来自Adobe Workfront的HTTP 429状态代码不应导致停用，而是会在场景中触发短暂的执行暂停。

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

<!--
* [Watch Events](#watch-events) 
* [Watch Record](#watch-record) 
* [Watch Field](#watch-field)
-->

+++ **[!UICONTROL 观看活动]**

在Workfront中添加、更新或删除特定类型的对象时，此触发器模块会实时执行场景

该模块会返回与记录关联的任何标准字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

1. 单击&#x200B;**Webhook**&#x200B;框右侧的&#x200B;**[!UICONTROL 添加]**。

1. 在显示的&#x200B;**[!UICONTROL 添加挂接]**&#x200B;框中配置webhook。

   配置此模块时，会显示以下字段。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[！UICONTROL Webhook名称]</td> 
      <td>（可选）为webhook键入新名称</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL Connection]</td> 
      <td> <p>有关将[!DNL Workfront]应用连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">将[!DNL Workfront]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL记录类型]</td> 
      <td>选择要模块监视的[!DNL Workfront]记录的类型。</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL状态]</td> 
      <td>选择您要观察旧状态还是新状态。<ul><li><p><b>[！UICONTROL新状态]</b></p><p>当记录将<b>更改为</b>给定值时触发方案。</p><p>例如，如果状态设置为[！UICONTROL New State]，而过滤器设置为[！UICONTROL Status] [！UICONTROL Equals] [！UICONTROL In Progress]，则webhook会在[！UICONTROL Status]更改为[！UICONTROL In Progress]时触发场景，而不管状态之前是什么。 </p></li><li><p><b>[！UICONTROL旧状态]</b></p><p>当记录从</b>更改<b>给定值时触发方案。</p><p>例如，如果状态设置为[！UICONTROL Old State]，而过滤器设置为[！UICONTROL Status] [！UICONTROL Equals] [！UICONTROL In Progress]，则当[！UICONTROL Status]当前为[！UICONTROL In Progress]的状态更改为其他状态时，webhook会触发一个场景。 </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[！UICONTROL事件过滤器]</p> </td> 
      <td> <p>您可以设置过滤器，以仅监视符合您选择标准的记录。</p> <p>对于每个筛选器，输入希望筛选器计算的字段、运算符以及希望筛选器允许的值。 通过添加AND规则，您可以使用多个过滤器。</p> <p>注意：您无法编辑现有[!DNL Workfront] Webhook中的筛选器。 要为[!DNL Workfront]事件订阅设置不同的筛选器，请删除当前webhook并创建一个新筛选器。</p> <p>有关事件过滤器的详细信息，请参阅本文中[!DNL Workfront] &gt; [！UICONTROL监视事件]模块中的<a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">事件订阅过滤器</a>。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>排除由此连接产生的事件</td> 
      <td>启用此选项可排除使用此触发器模块使用的同一连接器创建或更新的事件。 这可以防止场景触发自身，导致其在无休止循环中重复的情况。<p><b>注意</b>工作分配记录类型不包括此选项。</p></td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL记录源]</td> 
      <td> <p>选择您希望方案仅观看<strong>[！UICONTROL新记录]</strong>、<strong>[！UICONTROL仅更新记录]</strong>、<strong>[！UICONTROL新记录和更新记录]</strong>还是<strong>[!DNL Deleted Records Only]</strong>。</p> <p>注意：如果您选择<strong>[！UICONTROL新建和更新的记录]</strong>，webhook创建将创建2个事件订阅（针对同一webhook地址）。</p> </td> 
     </tr> 
    </tbody> 
   </table>

创建webhook后，您可以查看事件所发往的端点地址。

有关详细信息，请参阅[!DNL Workfront]帮助文章[事件订阅API](../../wf-api/general/event-subs-api.md)中的[事件负载示例](../../wf-api/general/event-subs-api.md#examples-of-event-payloads)部分。

查看可在每个 [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 对象类型中使用此模块的[!DNL Workfront]对象类型列表。

+++

+++ **[!UICONTROL 监视字段]**

当您指定的字段更新时，此触发器模块会执行场景。 模块会返回您指定的字段的旧值和新值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Workfront]应用连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">将[!DNL Workfront]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL记录类型]</td> 
   <td> <p>选择要模块监视的[!DNL Workfront]记录的类型。</p> <p>例如，如果希望每次更新任务中的记录字段时都开始执行方案，请选择[！UICONTROL Task]。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL字段]</td> 
   <td>选择您希望模块关注更新的字段。 这些字段反映了[!DNL Workfront]管理员为跟踪而设置的字段。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL输出]</td> 
   <td>选择要包含在此模块的输出捆绑包中的信息。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

查看可在每个 [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 对象类型中使用此模块的[!DNL Workfront]对象类型列表。

+++

+++ **[!UICONTROL 观看记录]**

此触发器模块执行特定类型的对象添加、更新或同时添加和更新的方案。 该模块返回与一个或多个记录关联的所有标准字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。 在输出中，模块指示每个记录是新的还是更新的。

在给定时间段内添加和更新的记录将作为新记录返回。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Workfront]应用连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">将[!DNL Workfront]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL筛选器]</td> 
   <td> <p>选择您希望方案仅观看<strong>[！UICONTROL新记录]</strong>、<strong>[！UICONTROL仅更新记录]</strong>还是<strong>[！UICONTROL新记录和更新记录]</strong>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>（在选择<strong>筛选器</strong>后显示。）选择您希望模块监视的[!DNL Workfront]记录类型。</p> <p>例如，如果您要在每次创建新项目时启动方案，请选择[！UICONTROL项目]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块的输出捆绑包中的信息。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL可选过滤器]</td> 
   <td> <p>（高级）键入API代码字符串以定义任何其他将细化标准的参数或代码。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

查看可在每个 [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 对象类型中使用此模块的[!DNL Workfront]对象类型列表。

+++


### 操作

<!--
* [Convert object](#convert-object) 
* [Create a record (attaching custom forms)](#create-a-record-attaching-custom-forms) 
* [Create a record](#create-a-record) 
* [Custom API Call](#custom-api-call) 
* [Delete Record](#delete-record) 
* [Download Document](#download-document) 
* [Misc Action](#misc-action) 
* [Read a Record](#read-a-record) 
* [Update Record](#update-record) 
* [Upload Document](#upload-document)
-->

+++ **[!UICONTROL 转换对象]**

此操作模块进行以下转换之一：

* 将问题转化为项目
* 将问题转化为任务
* 将任务转换为项目

>[!NOTE]
>
>自2024年7月起，转化对象时可包含自定义表单。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Workfront]应用连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">将[!DNL Workfront]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL对象类型]</td> 
   <td> <p>选择要转换的对象类型。 这是转换之前对象的类型。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL转换为]</td> 
   <td>选择要将其转换为的对象。 这是转换后对象的类型。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL &lt;对象&gt; ID]</td> 
   <td> <p>输入对象的ID。 </p> <p>注意：输入对象的ID时，可以开始键入对象的名称，然后从列表中选择该对象。 然后，模块在字段中输入相应的ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL模板ID]</td> 
   <td> <p>如果要转换为项目，请选择要用于项目的模板ID。</p> <p>注意：输入对象的ID时，可以开始键入对象的名称，然后从列表中选择该对象。 然后，模块在字段中输入相应的ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL自定义表单]</td> 
   <td>选择要添加到新转换的对象中的任何自定义表单，然后输入自定义表单字段的值。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL Options]</td> 
   <td> <p>在转换对象时启用所需的任意选项。 选项是否可用取决于您要转换到的对象或从哪个对象转换。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL复制本机字段]</td> 
   <td> <p>启用此选项可将任何本地字段从原始对象复制到新对象。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL复制自定义表单]</td> 
   <td> <p>启用此选项可将任何本地字段从原始对象复制到新对象。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 创建记录（附加自定义表单）]**

此操作模块在[!DNL Workfront]中创建对象，如项目、任务或问题，并允许您向新对象添加自定义表单。 利用模块，可选择模块中可用的对象字段。

您指定记录的ID。

该模块返回记录ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

例如，当客户端在需要完成的任务的[!DNL Google Sheets]列表中添加新行时，可以使用此模块在[!DNL Workfront]中创建任务。

配置此模块时，会显示以下字段。

确保提供最小数量的输入字段。 例如，如果您要创建问题，则需要在“项目ID”字段中提供有效的父项目ID，以指示问题应存在于Workfront中的位置。 您可以使用映射面板从场景中的其他模块映射此信息，也可以通过键入名称，然后从列表中选择该名称来手动输入该信息。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Workfront]应用连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">将[!DNL Workfront]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL记录类型]</td> 
   <td> <p>选择要模块创建的[!DNL Workfront]记录的类型。</p> <p>例如，如果要创建项目，请从下拉列表中选择[！UICONTROL项目]，并确保您有权访问将填充该项目的数据（来自场景中以前的模块）。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL选择要映射的字段]</td> 
   <td> <p>选择可用于数据输入的字段。 这样，您就无需滚动浏览不需要的字段即可使用这些字段。</p> <p>对于自定义表单中的字段，请使用<b>[！UICONTROL附加自定义表单]</b>字段。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL附加自定义表单]</td> 
   <td>选择要添加到新对象的任何自定义表单，然后输入这些字段的值。</td> 
  </tr> 
 </tbody> 
</table>

查看可在每个 [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 对象类型中使用此模块的[!DNL Workfront]对象类型列表。

>[!NOTE]
>
>* 输入对象的ID时，可以开始键入对象的名称，然后从列表中选择该对象。 然后，模块在字段中输入相应的ID。
>* 为自定义字段或[!UICONTROL 注释]对象（注释或回复）输入文本时，您可以使用[!UICONTROL 注释文本]字段中的HTML标记来创建富文本，如粗体或斜体文本。
>
>  有关更新中富文本的详细信息，请参阅[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)中的[将更新添加到工作项](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add)。
>

+++

+++ **[!UICONTROL 创建记录]**

此操作模块可在Workfront中创建对象，如项目、任务或问题。 利用模块，可选择模块中可用的对象字段。

您指定记录的ID。

该模块返回记录ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

例如，当客户端在Google工作表中添加新行时，您可以使用此模块在[!DNL Workfront]中创建一项任务，该列表包含需要完成的任务。

配置此模块时，会显示以下字段。

确保提供最小数量的输入字段。 例如，如果您要创建问题，则需要在“项目ID”字段中提供有效的父项目ID，以指示问题应存在于Workfront中的位置。 您可以使用映射面板从场景中的其他模块映射此信息，也可以通过键入名称，然后从列表中选择该名称来手动输入该信息。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Workfront]应用连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">将[!DNL Workfront]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL记录类型]</td> 
   <td> <p>选择要模块创建的[!DNL Workfront]记录的类型。</p> <p>例如，如果要创建项目，请从下拉列表中选择[！UICONTROL项目]，并确保您有权访问将填充该项目的数据（来自场景中以前的模块）。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL选择要映射的字段]</td> 
   <td>选择可用于数据输入的字段。 这样，您就无需滚动浏览不需要的字段即可使用这些字段。</td> 
  </tr> 
 </tbody> 
</table>

查看可在每个 [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 对象类型中使用此模块的[!DNL Workfront]对象类型列表。

>[!NOTE]
>
>* 输入对象的ID时，可以开始键入对象的名称，然后从列表中选择该对象。 然后，模块在字段中输入相应的ID。
>* 为自定义字段或[!UICONTROL 注释]对象（注释或回复）输入文本时，您可以使用[!UICONTROL 注释文本]字段中的HTML标记来创建富文本，如粗体或斜体文本。
>
>  有关更新中富文本的详细信息，请参阅[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)中的[将更新添加到工作项](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add)。
>

+++

+++ **[!UICONTROL 自定义API调用]**

此操作模块允许您对[!DNL Workfront] API进行经过身份验证的自定义调用。 这样，您可以创建其他[!DNL Workfront]模块无法实现的数据流自动化。

模块返回以下信息：

* **[!UICONTROL 状态代码]** （数字）：这表示HTTP请求是成功还是失败。 这些是标准代码，您可以在互联网上查找。
* **[!UICONTROL 标头]** （对象）：与输出正文无关的响应/状态代码的更详细的上下文。 并非响应标头中显示的所有标头都是响应标头，因此某些标头可能对您没什么用。

  响应标头取决于您在配置模块时选择的HTTP请求。

* **[!UICONTROL Body]**（对象）：根据您在配置模块时选择的HTTP请求，您可能会收到一些返回的数据。 该数据(例如来自GET请求的数据)包含在此对象中。

您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Workfront]应用连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">将[!DNL Workfront]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>输入相对于<code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>的路径。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL API版本]</td> 
   <td>选择您希望模块使用的[!DNL Workfront] API的版本。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP请求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。 这会确定请求的内容类型。</p> <p>例如，<code> {"Content-type":"application/json"}</code></p> <p>注意：如果您收到错误并且难以确定其来源，请考虑根据[!DNL Workfront]文档修改标头。 如果自定义API调用返回422 HTTP请求错误，请尝试使用<code>"Content-Type":"text/plain"</code>标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> <p>提示：我们建议您通过JSON正文而不是查询参数发送信息。</p> </td> 
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

查看可在每个 [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 对象类型中使用此模块的[!DNL Workfront]对象类型列表。

+++

+++ **[!UICONTROL 删除记录]**

此操作模块可删除对象，如Workfront中的项目、任务或问题。

您指定记录的ID。

该模块返回记录ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Workfront]应用连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">将[!DNL Workfront]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL强制删除]</td> 
   <td>启用此选项以确保删除记录，即使[!DNL Workfront] UI会请求确认删除。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>输入您希望模块删除的记录的唯一[!DNL Workfront] ID。</p> <p>要获取ID，请在浏览器中打开[!DNL Workfront]对象，并在“ID=”之后复制URL末尾的文本。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL记录类型]</td> 
   <td>选择要模块删除的[!DNL Workfront]记录的类型。</td> 
  </tr> 
 </tbody> 
</table>

查看可在每个 [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 对象类型中使用此模块的[!DNL Workfront]对象类型列表。

>[!NOTE]
>
>我们建议采用以下方案配置，以避免因异步操作而无法删除记录。
>
>1. 同步删除记录。
>1. 将错误处理添加到删除记录模块以忽略由40秒超时导致的错误。


+++

+++ **[!UICONTROL 下载文档]**

此操作模块可从Workfront下载文档。

您指定记录的ID。

该模块返回文档的内容、文件名、文件扩展名和文件大小。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Workfront]应用连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">将[!DNL Workfront]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文档ID]</td> 
   <td> <p>映射或手动输入您希望模块下载的文档的唯一[!DNL Workfront] ID。</p> <p>要获取ID，请在浏览器中打开[!DNL Workfront]对象，并在“ID=”之后复制URL末尾的文本。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

查看可在每个 [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 对象类型中使用此模块的[!DNL Workfront]对象类型列表。

+++

+++ **[!UICONTROL 其他操作]**

通过此操作模块，您可以对API执行操作。

>[!NOTE]
>
>自2024年7月起，`convertToProject`操作包括字段`copyCategories`。 当设置为`TRUE`时，所有自定义表单都将包含在问题所转换到的项目中。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Workfront]应用连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">将[!DNL Workfront]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL记录类型]</td> 
   <td> <p>选择您希望模块与之交互的[!DNL Workfront]记录的类型。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL操作]</td> 
   <td> <p>选择要模块执行的操作。</p> <p>根据您选择的[！UICONTROL记录类型]和[！UICONTROL操作]，您可能需要填写其他字段。 这两个设置的某些组合可能只需要记录ID，而其他设置（如<strong>[！UICONTROL记录类型的Project]</strong>和<strong>[！UICONTROL操作]</strong>的[！UICONTROL附加模板]）需要其他信息（如对象ID和模板ID）。</p><p>有关某些操作可用的选项，请参阅本文中的<a href="#misc-action-options" class="MCXref xref">其他操作选项</a>。</p> <p>有关各个字段的详细信息，请参阅<a href="http://developer.workfront.com/">Workfront开发人员文档</a>。 <p><strong>注意</strong>：开发人员文档网站仅包含通过API版本14传递的信息，但仍包含可供API调用使用的有用信息。 </p> 
    <ol> 
     <li value="1"> <p>从[!DNL Workfront]开发人员文档页面的左侧导航中选择记录类型。 以下类型有自己的页面：</p> 
      <ul> 
       <li> <p>[！UICONTROL项目]</p> </li> 
       <li> <p>[！UICONTROL任务]</p> </li> 
       <li> <p>[！UICONTROL Issues]</p> </li> 
       <li> <p>[！UICONTROL用户]</p> </li> 
       <li> <p>[！UICONTROL文档]</p> </li> 
      </ul> <p>对于所有其他记录类型，请选择<b>[！UICONTROL Other objects and endpoints]</b>，然后在按字母顺序排序的页面上查找该记录类型。</p> </li> 
     <li value="2"> <p>在相应记录类型的页面上，搜索操作（Ctrl-F或Cmd-F）。</p> </li> 
     <li value="3"> <p>查看所选操作下可用字段的描述。</p> </li> 
    </ol> <p>注意：  <p>通过[!DNL Workfront] [！UICONTROL杂项操作]模块创建验证时，最佳实践是创建不包含任何高级选项的验证，然后使用[!DNL Workfront Proof] SOAP API更新验证。</p> <p>有关使用[!DNL Workfront] API（此模块使用）创建验证的更多信息，请参阅<a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">通过[!DNL Adobe Workfront] API创建验证时添加高级验证选项</a></p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL ID]</td> 
   <td>输入或映射您希望模块与之交互的记录的唯一[!DNL Workfront] ID。<p>要获取ID，请在浏览器中打开[!DNL Workfront]对象，并在“ID=”之后复制URL末尾的文本。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

查看可在每个 [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 对象类型中使用此模块的[!DNL Workfront]对象类型列表。

#### 其他操作选项

##### 任务

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <th>操作</th> 
   <th>选项</th> 
  </tr> 
  <tr> 
   <td>复制</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignations</li>
   <li>clearConstraints</li>
   <li>clearCustomData</li>
   <li>clearDocuments</li>
   <li>clearExpenses</li>
   <li>clearFinancials<p>清除财务数据</p></li>
   <li>clearpermissions</li>
   <li>clearPredecessors</li>
   <li>clearProgress</li>
   <li>clearTimedNotifications<p>清除提醒通知</p></li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>移动</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignations</li>
   <li>clearDocuments</li>
   <li>clearConstraints</li>
   <li>clearExpenses</li>
   <li>clearFinancials<p>清除财务数据</p></li>
   <li>clearpermissions</li>
   <li>clearPredecessors</li>
   <li>clearProgress</li>
   <li>clearTimedNotifications<p>清除提醒通知</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

##### 问题

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <th>操作</th> 
   <th>选项</th> 
  </tr> 
  <tr> 
   <td>复制</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignations</li>
   <li>clearCustomData</li>
   <li>clearDocuments</li>
   <li>clearpermissions</li>
   <li>clearProgress</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>转换为任务</td> 
   <td>
   <ul>
   <li>preserveIssue<p>保留原来的问题，并将其解决方案与此任务绑定</p></li>
   <li>preservePrimaryContact<p>允许问题的主要联系人访问此任务</p></li>
   <li>preserveCompletionDate<p>保留问题的计划完成日期</p></li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>转换至项目</td> 
   <td>
   <ul>
   <li>preserveIssue<p>保留原来的问题，并将其解决方案与此任务绑定</p></li>
   <li>preservePrimaryContact<p>允许问题的主要联系人访问此任务</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>



##### 项目

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <th>操作</th> 
   <th>选项</th> 
  </tr> 
  <tr> 
   <td>复制</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignations</li>
   <li>clearCustomData</li>
   <li>clearDocuments</li>
   <li>clearExpenses</li>
   <li>clearFinancials<p>清除财务数据</p></li>
   <li>clearpermissions</li>
   <li>clearPredecessors</li>
   <li>clearProgress</li>
   <li>clearTimedNotifications<p>清除提醒通知</p></li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>附加模板/另存为模板</td> 
   <td>
   <ul>
   <li>clearApprovers</li>
   <li>clearAssignations</li>
   <li>clearBillingRates</li>
   <li>clearConstraints</li>
   <li>clearDeliverable<p>清除目标</p></li>
   <li>clearDocuments</li>
   <li>clearExpenses</li>
   <li>clearFinancials<p>清除财务数据</p></li>
   <li>clearHourTypes</li>
   <li>Clearisssetup<p>清除队列属性和问题设置</p></li>
   <li>clearPredecessors</li>
   <li>clearrisks</li>
   <li>clearSharingOptions</li>
   <li>clearTimedNotifications<p>清除提醒通知</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>



+++

+++ **[!UICONTROL 读取记录]**

此操作模块从单个记录中检索数据。

您指定记录的ID。 您还可以指定希望模块读取哪些相关记录。

例如，如果模块正在读取的记录是项目，则可以指定希望读取项目的任务。

模块从指定输出的标准字段中返回一个数据数组。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[！UICONTROL Connection]</td>
    <td> <p>有关将[!DNL Workfront]应用连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">将[!DNL Workfront]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL记录类型]</td>
     <td>选择您希望模块读取的[!DNL Workfront]对象类型。</td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL输出]</td>
     <td> <p>选择要包含在此模块的输出捆绑包中的信息。</p> </td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL引用]</td>
   <td>选择要包含在输出中的任何引用字段。</td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL收藏集]</td>
   <td>选择要包含在输出中的任何引用字段。</td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL ID]</td>
   <td> <p>输入您希望模块读取的记录的唯一[!DNL Workfront] ID。</p> <p>要获取ID，请在浏览器中打开[!DNL Workfront]对象，并在“ID=”之后复制URL末尾的文本。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

查看可在每个 [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 对象类型中使用此模块的[!DNL Workfront]对象类型列表。

+++

+++ **[!UICONTROL 更新记录]**

此操作模块可更新对象，如项目、任务或问题。 利用模块，可选择模块中可用的对象字段。

您指定记录的ID。

模块会返回对象的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Workfront]应用连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">将[!DNL Workfront]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL ID]</td> 
   <td> <p>输入您希望模块更新的记录的唯一[!DNL Workfront] ID。</p> <p>要获取ID，请在浏览器中打开[!DNL Workfront]对象，并在“ID=”之后复制URL末尾的文本。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>选择要更新模块的[!DNL Workfront]记录的类型。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>选择可用于数据输入的字段。 这样，您就无需滚动浏览不需要的字段即可使用这些字段。</td> 
  </tr> 
 </tbody> 
</table>

查看可在每个 [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 对象类型中使用此模块的[!DNL Workfront]对象类型列表。

>[!NOTE]
>
>* 输入对象的ID时，可以开始键入对象的名称，然后从列表中选择该对象。 然后，模块在字段中输入相应的ID。
>* 为自定义字段或[!UICONTROL 注释]对象（注释或回复）输入文本时，您可以使用[!UICONTROL 注释文本]字段中的HTML标记来创建富文本，如粗体或斜体文本。
>
>  有关更新中富文本的详细信息，请参阅[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)中的[将更新添加到工作项](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add)。
>

+++

+++ **[!UICONTROL 上载文档]**

此操作模块将文档上传到[!DNL Workfront]对象，如项目、任务或问题。 此模块会以块形式上传文档，从而使Workfront的上传过程更加顺畅。

您可以指定文档的位置、要上传的文件以及文件的新名称（可选）。

模块会返回文档的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Workfront]应用连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">将[!DNL Workfront]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL相关记录ID]</td> 
   <td>输入要上载文档的记录的唯一[!DNL Workfront] ID。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL相关记录类型]</td> 
   <td>选择您希望模块上传文档的[!DNL Workfront]记录类型。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹ID]</td> 
   <td>根据相关记录的类型，您可能需要输入或映射文件夹ID。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Source file]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

查看可在每个 [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 对象类型中使用此模块的[!DNL Workfront]对象类型列表。

+++

+++ **[!UICONTROL 上载文档（旧版）]**

此操作模块将文档上传到[!DNL Workfront]对象，如项目、任务或问题。 它一次上载整个文档。

您可以指定文档的位置、要上传的文件以及文件的新名称（可选）。

模块会返回文档的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Workfront]应用连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">将[!DNL Workfront]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL相关记录ID]</td> 
   <td>输入要上载文档的记录的唯一[!DNL Workfront] ID。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL相关记录类型]</td> 
   <td>选择您希望模块上传文档的[!DNL Workfront]记录类型。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹ID]</td> 
   <td>根据相关记录的类型，您可能需要输入或映射文件夹ID。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Source file]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

查看可在每个 [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 对象类型中使用此模块的[!DNL Workfront]对象类型列表。

+++

### 搜索

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL 读取相关记录]**

此搜索模块读取与指定的搜索查询相匹配的记录（在特定父对象中）。

您可以指定要包含在输出中的字段。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Workfront]应用连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">将[!DNL Workfront]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL记录类型]</td> 
   <td> <p>选择要读取其关联记录的父记录(Workfront对象)的类型。</p> <p>查看[!DNL Workfront]对象类型的列表，您可以在此文章中每个[!DNL Workfront]模块</a>可用的<a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront]对象类型中使用此模块。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL父记录ID]</td> 
   <td> <p>输入或映射要读取其关联记录的父记录的ID。</p> <p>要获取ID，请在浏览器中打开[!DNL Workfront]对象，并在“ID=”之后复制URL末尾的文本。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL收藏集]</td> 
   <td>选择或映射您希望模块读取的子记录类型。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块的输出捆绑包中的信息。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 搜索]**

此搜索模块在[!DNL Workfront]中查找与您指定的搜索查询匹配的对象中的记录。

您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Workfront]应用连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">将[!DNL Workfront]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL记录类型]</td> 
   <td> <p>选择要模块搜索的[!DNL Workfront]记录的类型。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL结果集]</td> 
   <td>选择一个选项，以指定您希望模块获得符合您的搜索条件的第一个结果还是所有符合该条件的结果。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最大]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜索条件字段]</td> 
   <td> <p>选择要用于搜索条件的字段。 随后，这些字段将显示在搜索条件下拉列表中。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜索条件]</td> 
   <td> <p>输入搜索依据的字段、要在查询中使用的运算符以及要在字段中搜索的值。</p> <p>注意：请勿在您的搜索条件中使用<code>username </code>。 在对[!DNL Workfront]的API查询中包含<code>username </code>会将用户记录到Workfront中，搜索将不会成功。</p> <p>注意： <code>In</code>和<code>NotIn</code>使用数组。 输入的格式应为数组。</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块输出中的字段。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL引用]</td> 
   <td>选择要包含在搜索中的任何引用字段。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL收藏集]</td> 
   <td>选择要添加到搜索的任何收藏集。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 搜索（旧版）]**

此搜索模块在[!DNL Workfront]中查找与您指定的搜索查询匹配的对象中的记录。

您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Workfront]应用连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">将[!DNL Workfront]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL记录类型]</td> 
   <td> <p>选择要模块搜索的[!DNL Workfront]记录的类型。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL结果集]</td> 
   <td>选择一个选项，以指定您希望模块获得符合您的搜索条件的第一个结果还是所有符合该条件的结果。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最大]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜索条件]</td> 
   <td> <p>输入搜索依据的字段、要在查询中使用的运算符以及要在字段中搜索的值。</p> <p>注意：请勿在您的搜索条件中使用<code>username </code>。 在对[!DNL Workfront]的API查询中包含<code>username </code>会将用户记录到Workfront中，搜索将不会成功。</p> <p>注意： <code>In</code>和<code>NotIn</code>使用数组。 输入的格式应为数组。</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块输出中的字段。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL引用]</td> 
   <td>选择要包含在搜索中的任何引用字段。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL收藏集]</td> 
   <td>选择要添加到搜索的任何收藏集。</td> 
  </tr> 
 </tbody> 
</table>

查看可在每个 [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 对象类型中使用此模块的[!DNL Workfront]对象类型列表。

+++

## 每个[!DNL Workfront]模块都有[!DNL Workfront]对象类型可用

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++每个[!DNL Workfront]触发器模块都有&#x200B;**可用的对象类型**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[！UICONTROL监视记录]</th> 
   <th>[！UICONTROL监视字段]</th> 
   <th>[！UICONTROL监视活动]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>审批流程</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任务分配</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>基线</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 账单记录 </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>记帐费率</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>仪表板</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>文档</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>文档文件夹</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>文档请求</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>文档版本</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>费用</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>费用类型</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>组</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>小时</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>小时数类型</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>问题</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>迭代</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>工作角色</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>日志条目</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑路径</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>注释</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>注释标签</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>项目组合</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>项目群</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>项目用户</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>校样审批</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>保留时间* </td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>报告</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>风险</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>风险类型</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>步骤审批者</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任务</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>团队</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>模板</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>模板任务</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>时间表</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>更新</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++每个[!DNL Workfront]操作模块都有&#x200B;**可用的对象类型**

>[!NOTE]
>
>[!UICONTROL 下载文档]模块未包含在此表中，因为[!DNL Workfront]对象类型不是其配置的一部分。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[！UICONTROL创建记录]</th> 
   <th>[！UICONTROL更新记录]</th> 
   <th>[！UICONTROL删除记录]</th> 
   <th>[！UICONTROL上传文档]</th> 
   <th>[！UICONTROL读取记录]</th> 
   <th>[！UICONTROL自定义API调用]</th> 
   <th>[！UICONTROL杂项操作]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>审批流程</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>任务分配</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>基线</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
   <tr> 
   <td>账单记录</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>记帐费率</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>文档</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>文档文件夹</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>文档版本</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>汇率</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>费用</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>费用类型</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>外部文档</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>组</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>小时</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>小时数类型</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>问题</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>迭代</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>工作角色</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>日志条目</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>里程碑</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑路径</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>注释</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>注释标签</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>项目组合</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>项目群</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>项目用户</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>保留时间* </td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>风险</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>风险类型</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>步骤审批者</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任务</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>团队</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>模板</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>模板任务</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>时间表</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>更新</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++每个[!DNL Workfront]搜索模块都有&#x200B;**可用的对象类型**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[！UICONTROL搜索]</th> 
   <th>[！UICONTROL读取相关记录]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>审批流程</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>任务分配</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>账单记录</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>记帐费率</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>文档</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>文档文件夹</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>文档版本</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>费用</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>费用类型</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>组</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>小时</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>小时数类型</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>问题</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>迭代</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>工作角色</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>日志条目</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑路径</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>注释</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>注释标签</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>项目组合</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>项目群</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>项目用户</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>保留时间* </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>风险</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>风险类型</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>步骤审批者</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任务</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>团队</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>模板</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>模板任务</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>时间表</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>用户委托</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

我们建议您仔细检查，以确保它按您预期的方式运行。

+++

## [!DNL Workfront] > [!UICONTROL 观看活动]模块中的活动订阅筛选器

>[!NOTE]
>
>我们强烈建议在您的[!UICONTROL 观看活动]模块中使用活动订阅过滤器。

[!DNL Workfront] [!UICONTROL 监视事件]模块根据webhook触发在[!DNL Workfront] API中创建事件订阅的场景。 事件订阅是一组数据，用于确定哪些事件发送到webhook。 例如，如果您设置了[!UICONTROL 监视事件]模块来监视问题，则事件订阅仅发送与问题相关的事件。

通过使用事件订阅过滤器，Fusion用户可以创建更适合其用例的事件订阅。 例如，您可以在[!DNL Workfront] API中设置事件订阅，以便仅将特定项目中的问题发送到webhook，从而确保[!UICONTROL Watch Events]模块将仅触发该项目中的问题。 创建更窄触发器的功能通过减少无关触发器的数量而改进了方案设计。

这与在[!DNL Workfront Fusion]方案中设置过滤器不同。 如果没有事件订阅过滤器，您的webhook将接收与您选择的对象类型相关的所有事件。 这些事件中的大多数与方案无关，必须先将其过滤掉，方案才能继续。

在Workfront >关注事件过滤器中可以使用以下运算符：

* 等于
* 不等于
* 大于
* 小于
* 大于或等于
* 小于或等于
* 包含
* 已存在
   * 此运算符不需要值，并且值字段不存在。
* 不存在
   * 此运算符不需要值，并且值字段不存在。
* 已更改
   * 此运算符不需要值，并且值字段不存在。
   * 此运算符忽略状态字段。
   * 使用`Changed`时，在&#x200B;**记录来源**&#x200B;字段中选择&#x200B;**仅更新事件**。

>[!IMPORTANT]
>
>无法在现有[!DNL Workfront] Webhook中编辑筛选器。 要为[!DNL Workfront]事件订阅设置不同的筛选器，请删除当前webhook并创建一个新筛选器。

>[!INFO]
>
>**示例：**&#x200B;考虑处理分配给特定用户Ana的新问题的方案。
>
>### 使用事件订阅过滤器过滤事件（推荐）
>
>使用事件过滤器，您可以设置webhook以在创建问题时将问题分配给Ana时触发场景。 Ana具有userID b378489d8f7cd3cee0539260720a84b7。
>
>![](assets/event-filter-watch-events-350x277.png)
>
>如果一天内创建100个问题，但只有两个问题分配给Ana，则该场景将执行两次。
>
>### 筛选场景中的事件（不推荐）
>
>要筛选事件以便仅处理分配给Ana的问题，您可以在[!UICONTROL 关注事件]模块之后创建筛选器。
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>如果一天内创建100个问题，但只有两个问题分配给Ana，则该场景将执行100次。 98个执行将在过滤器处停止，但触发器模块仍在使用数据并对所有执行执行执行操作。

有关活动订阅的详细信息，请参阅[常见问题解答 — 活动订阅](../../wf-api/general/event-subs-faq.md)。

有关Webhook的详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)中的[即时触发器(Webhook)

有关场景中过滤器的更多信息，请参阅[将过滤器添加到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md)中的场景。

