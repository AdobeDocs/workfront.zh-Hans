---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Adobe Workfront模块
description: 您可以使用Adobe Workfront Fusion Adobe Workfront连接器在Workfront中自动执行您的流程。 如果您拥有Workfront Fusion for Work Automation和集成许可证，则还可以使用它连接到第三方应用程序和服务。
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: b84d2d41-a983-4ea3-b331-0302bfcf8a2b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '5276'
ht-degree: 3%

---

# [!DNL Adobe Workfront] 模块

您可以使用 [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] 连接器可在 [!DNL Workfront]. 如果您有 [!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成）] 许可证，您还可以使用它连接到第三方应用程序和服务。

的 [!DNL Workfront] 连接器不计入贵组织可用的活动应用程序数。 所有方案，即使它们仅使用 [!DNL Workfront] 应用程序时，请根据贵组织的总方案计数计算。

有关贵组织可用应用程序和方案的更多信息，请参阅 [组织](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) in [[!DNL Adobe Workfront Fusion] 组织和团队](../../workfront-fusion/organizations/organizations-and-teams.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p>  <p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化）</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>


要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 连接 [!DNL Workfront] to [!DNL Workfront Fusion]

的 [!DNL Workfront] 连接器使用OAuth 2.0连接到 [!DNL Workfront].

您可以创建与 [!DNL Workfront] 直接从内部帐户 [!DNL Workfront Fusion] 模块。

1. 在任意 [!DNL Workfront] 应用程序模块，单击 **[!UICONTROL 添加]** 旁边 [!UICONTROL 连接] 框中。
1. 在URL中输入实例的名称。 示例: `https://<your instance>.my.workfront.com`.
1. 单击 **[!UICONTROL 下一个]**.
1. 单击 **[!UICONTROL SAML登录]** 创建连接，然后返回到模块。

   或

   输入您的用户名和密码，然后单击 **[!UICONTROL 登录]** 创建连接，然后返回到模块。

   >[!NOTE]
   >
   >* 如果看不到SAML登录按钮，则表示贵组织未启用单点登录(SSO)。 您可以使用您的用户名和密码登录。
      >   
      >   有关单点登录(SSO)的详细信息，请参阅 [单点登录概述 [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
   >   
   >* 与 [!DNL Workfront] API不再依赖API密钥。


## [!DNL Workfront] 模块及其字段

配置 [!DNL Workfront] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Workfront] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

<!--
* [Watch Events](#watch-events) 
* [Watch Record](#watch-record) 
* [Watch Field](#watch-field)
-->

+++ **[!UICONTROL 观看事件]**

当在Workfront中添加、更新或删除特定类型的对象时，此触发器模块会实时执行一个方案

模块会返回与记录关联的任何标准字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

1. 单击 **[!UICONTROL 添加]** 权利 **网钩** 框中。

1. 在 **[!UICONTROL 添加挂接]** 框中。

   配置此模块时，将显示以下字段。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Webhook name]</td> 
      <td>（可选）为网页挂接键入新名称</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL连接]</td> 
      <td> <p>有关连接 [!DNL Workfront] 应用程序 [!DNL Workfront Fusion]，请参阅 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">连接 [!DNL Workfront] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL记录类型]</td> 
      <td>选择 [!DNL Workfront] 记录您希望模块监视的内容。</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL State]</td> 
      <td>选择您要观看旧状态还是新状态。<ul><li><p><b>[!UICONTROL New state]</b></p><p>记录更改时会触发方案 <b>to</b> 给定值。</p><p>例如，如果状态设置为[!UICONTROL New State] ，而过滤器设置为[!UICONTROL Status] [!UICONTROL Equals] [!UICONTROL In Progress] ，则当[!UICONTROL Status]更改为[!UICONTROL In Progress]时，Webhook将触发一个方案，而无论之前的状态如何。 </p></li><li><p><b>[!UICONTROL旧状态]</b></p><p>记录更改时会触发方案 <b>从</b> 给定值。</p><p>例如，如果状态设置为[!UICONTROL Old State] ，而过滤器设置为[!UICONTROL Status] [!UICONTROL Equals] [!UICONTROL In Progress] ，则当当前为[!UICONTROL Status]的[!UICONTROL In Progress]的[!UICONTROL Status]变为其他状态时，Webhook将触发一个方案。 </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL事件过滤器]</p> </td> 
      <td> <p>您可以设置过滤器，以便仅监视符合您选择的标准的记录。</p> <p>对于每个过滤器，输入您希望过滤器评估的字段、运算符以及您希望过滤器允许的值。 您可以通过添加AND规则来使用多个过滤器。</p> <p>注意：无法编辑现有 [!DNL Workfront] 网络挂钩。 为 [!DNL Workfront] 事件订阅，删除当前webhook并创建新webhook。</p> <p>有关事件过滤器的更多信息，请参阅 <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">中的事件订阅过滤器 [!DNL Workfront] &gt; [!UICONTROL Watch Events]模块</a> 在本文中。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>排除此连接所发生的事件</td> 
      <td>启用此选项可排除使用此触发器模块所使用的相同连接器创建或更新的事件。 这可以防止情景可能触发自身的情况，导致其在无休止循环中重复。</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL记录来源]</td> 
      <td> <p>选择是否希望方案监视 <strong>[!UICONTROL仅新记录]</strong>, <strong>[!UICONTROL仅更新记录]</strong>, <strong>[!UICONTROL新记录和更新记录]</strong>或 <strong>[!DNL Deleted Records Only]</strong>.</p> <p>注意：如果您选择 <strong>[!UICONTROL新记录和更新记录]</strong>，则创建webhook会创建2个事件订阅（对于同一webhook地址）。</p> </td> 
     </tr> 
    </tbody> 
   </table>

创建Webhook后，您可以查看事件发送到的端点的地址。

有关更多信息，请参阅 [事件负载示例](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) 在 [!DNL Workfront] 帮助文章 [事件订阅API](../../wf-api/general/event-subs-api.md).

查看 [!DNL Workfront] 可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 监视字段]**

此触发器模块会在您指定的字段更新时执行方案。 模块会返回您指定字段的旧值和新值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Workfront] 应用程序 [!DNL Workfront Fusion]，请参阅 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">连接 [!DNL Workfront] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL记录类型]</td> 
   <td> <p>选择 [!DNL Workfront] 记录您希望模块监视的内容。</p> <p>例如，如果希望在每次更新任务中的记录字段时都开始执行方案，请选择[!UICONTROL Task]。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL字段]</td> 
   <td>选择您希望模块监视的字段以进行更新。 这些字段反映了 [!DNL Workfront] 管理员已设置进行跟踪。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL输出]</td> 
   <td>选择要包含在此模块的输出包中的信息。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 观看记录]**

当添加、更新或同时添加特定类型的对象时，此触发器模块会执行一个方案。 模块会返回与记录或记录关联的所有标准字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。 在输出中，模块指示每个记录是新记录还是更新记录。

在给定时间段内添加和更新的记录将作为新记录返回。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Workfront] 应用程序 [!DNL Workfront Fusion]，请参阅 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">连接 [!DNL Workfront] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL过滤器]</td> 
   <td> <p>选择是否希望方案监视 <strong>[!UICONTROL仅新记录]</strong>, <strong>[!UICONTROL仅更新记录]</strong>或 <strong>[!UICONTROL新记录和更新记录]</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL记录类型]</td> 
   <td> <p>(在您选择 <strong>过滤器</strong>.) 选择 [!DNL Workfront] 记录您希望模块监视的内容。</p> <p>例如，如果您想在每次创建新项目时启动方案，请选择[!UICONTROL Project]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块的输出包中的信息。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL可选过滤器]</td> 
   <td> <p>（高级）键入一个API代码字符串，以定义将优化您的标准的任何其他参数或代码。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module).

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

此操作模块进行了以下转化之一：

* 将问题转换为项目
* 将问题转换为任务
* 将任务转换为项目

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Workfront] 应用程序 [!DNL Workfront Fusion]，请参阅 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">连接 [!DNL Workfront] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL对象类型]</td> 
   <td> <p>选择要转换的对象类型。 这是对象在转换之前具有的类型。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL转换为]</td> 
   <td>选择要将其转换为的对象。 这是对象在转换后具有的类型。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL &lt;object&gt; ID]</td> 
   <td> <p>输入对象的ID。 </p> <p>注意：输入对象的ID时，您可以开始键入对象的名称，然后从列表中选择该对象。 然后，模块在字段中输入相应的ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL模板ID]</td> 
   <td> <p>如果要转换为项目，请选择要用于项目的模板ID。</p> <p>注意：输入对象的ID时，您可以开始键入对象的名称，然后从列表中选择该对象。 然后，模块在字段中输入相应的ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL自定义表单]</td> 
   <td>选择要添加到新转换对象的任何自定义表单，然后为自定义表单的字段输入值。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL选项]</td> 
   <td> <p>在转换对象时，启用所需的任何选项。 选项可用，具体取决于您要转换到的对象或从中转换的对象。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 创建记录（附加自定义表单）]**

此操作模块会创建一个对象，如中的项目、任务或问题 [!DNL Workfront]，以及用于向新对象添加自定义表单。 利用模块，可选择模块中可用对象的哪些字段。

您指定记录的ID。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

例如，您可以使用此模块在 [!DNL Workfront] 当客户端在 [!DNL Google Sheets] 需要完成的任务列表。

配置此模块时，将显示以下字段。

确保提供最少的输入字段数。 例如，如果要创建问题，您需要在项目ID字段中提供有效的父项目ID，以指示该问题在Workfront中的位置。 您可以使用映射面板来映射方案中其他模块中的此信息，也可以通过键入名称并从列表中选择该名称来手动输入此信息。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Workfront] 应用程序 [!DNL Workfront Fusion]，请参阅 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">连接 [!DNL Workfront] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL记录类型]</td> 
   <td> <p>选择 [!DNL Workfront] 记录您希望模块创建的内容。</p> <p>例如，如果要创建项目，请从下拉列表中选择[!UICONTROL项目]，然后确保您有权访问将填充项目的数据（来自方案中的前几个模块）。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL选择要映射的字段]</td> 
   <td> <p>选择要用于数据输入的字段。 这样，您就无需滚动浏览您不需要的字段即可使用这些字段。</p> <p>对于自定义表单中的字段，请使用 <b>[!UICONTROL附加自定义表单]</b> 字段。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL附加自定义表单]</td> 
   <td>选择要添加到新对象的任何自定义表单，然后为这些字段输入值。</td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* 输入对象的ID时，您可以开始键入对象的名称，然后从列表中选择该对象。 然后，模块在字段中输入相应的ID。
>* 输入自定义字段或 [!UICONTROL 注意] 对象（注释或回复），您可以在 [!UICONTROL 注释文本] 字段来创建富文本，如粗体或斜体文本。
>
>  有关更新中富文本的更多信息，请参阅 [向工作项添加更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

+++

+++ **[!UICONTROL 创建记录]**

此操作模块会创建一个对象，如Workfront中的项目、任务或问题。 利用模块，可选择模块中可用对象的哪些字段。

您指定记录的ID。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

例如，您可以使用此模块在 [!DNL Workfront] 当客户端在Google工作表中添加新行时，需要完成的任务列表。

配置此模块时，将显示以下字段。

确保提供最少的输入字段数。 例如，如果要创建问题，您需要在项目ID字段中提供有效的父项目ID，以指示该问题在Workfront中的位置。 您可以使用映射面板来映射方案中其他模块中的此信息，也可以通过键入名称并从列表中选择该名称来手动输入此信息。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Workfront] 应用程序 [!DNL Workfront Fusion]，请参阅 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">连接 [!DNL Workfront] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL记录类型]</td> 
   <td> <p>选择 [!DNL Workfront] 记录您希望模块创建的内容。</p> <p>例如，如果要创建项目，请从下拉列表中选择[!UICONTROL项目]，然后确保您有权访问将填充项目的数据（来自方案中的前几个模块）。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL选择要映射的字段]</td> 
   <td>选择要用于数据输入的字段。 这样，您就无需滚动浏览您不需要的字段即可使用这些字段。</td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* 输入对象的ID时，您可以开始键入对象的名称，然后从列表中选择该对象。 然后，模块在字段中输入相应的ID。
>* 输入自定义字段或 [!UICONTROL 注意] 对象（注释或回复），您可以在 [!UICONTROL 注释文本] 字段来创建富文本，如粗体或斜体文本。
>
>  有关更新中富文本的更多信息，请参阅 [向工作项添加更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

+++

+++ **[!UICONTROL 自定义API调用]**

通过此操作模块，您可以对 [!DNL Workfront] API。 这样，您就可以创建数据流自动化，而另一个数据流无法实现 [!DNL Workfront] 模块。

该模块返回以下信息：

* **[!UICONTROL 状态代码]** （数字）：这表示HTTP请求的成功或失败。 这些是可在互联网上查找的标准代码。
* **[!UICONTROL 标题]** （对象）：与输出正文无关的响应/状态代码的更详细上下文。 响应标头中显示的并非所有标头都是响应标头，因此某些标头可能对您没有用处。

   响应标头取决于您在配置模块时选择的HTTP请求。

* **[!UICONTROL 正文]** （对象）：根据您在配置模块时选择的HTTP请求，您可能会收到一些数据。 该数据(如GET请求中的数据)包含在此对象中。

您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Workfront] 应用程序 [!DNL Workfront Fusion]，请参阅 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">连接 [!DNL Workfront] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>输入相对于<code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API版本]</td> 
   <td>选择 [!DNL Workfront] 您希望模块使用的API。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。 这可确定请求的内容类型。</p> <p>例如，<code> {"Content-type":"application/json"}</code></p> <p>注意：如果您收到错误，且很难确定其来源，请考虑根据 [!DNL Workfront] 文档。 如果您的自定义API调用返回422 HTTP请求错误，请尝试使用 <code>"Content-Type":"text/plain"</code> 标题。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> <p>提示：我们建议您通过JSON正文发送信息，而不是作为查询参数发送信息。</p> </td> 
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

查看 [!DNL Workfront] 可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 删除记录]**

此操作模块会删除对象，如Workfront中的项目、任务或问题。

您指定记录的ID。

模块会返回记录的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Workfront] 应用程序 [!DNL Workfront Fusion]，请参阅 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">连接 [!DNL Workfront] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL强制删除]</td> 
   <td>启用此选项可确保删除记录，即使 [!DNL Workfront] UI将请求确认删除。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>输入唯一 [!DNL Workfront] 您希望模块删除的记录的ID。</p> <p>要获取ID，请打开 [!DNL Workfront] 对象，并复制URL末尾的“ID=”后的文本。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL记录类型]</td> 
   <td>选择 [!DNL Workfront] 记录您希望删除模块。</td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 下载文档]**

此操作模块从Workfront下载文档。

您指定记录的ID。

模块返回文档的内容、文件名、文件扩展名和文件大小。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Workfront] 应用程序 [!DNL Workfront Fusion]，请参阅 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">连接 [!DNL Workfront] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文档ID]</td> 
   <td> <p>映射或手动输入唯一 [!DNL Workfront] 要下载模块的文档的ID。</p> <p>要获取ID，请打开 [!DNL Workfront] 对象，并复制URL末尾的“ID=”后的文本。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 杂项操作]**

此操作模块允许您对API执行操作。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Workfront] 应用程序 [!DNL Workfront Fusion]，请参阅 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">连接 [!DNL Workfront] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL记录类型]</td> 
   <td> <p>选择 [!DNL Workfront] 记录您希望模块与之交互。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Action]</td> 
   <td> <p>选择您希望模块执行的操作。</p> <p>您可能需要填写其他字段，具体取决于您选择的[!UICONTROL记录类型]和[!UICONTROL操作]。 这两个设置的某些组合可能只需要一个记录ID，而其他设置(例如 <strong>[!UICONTROL记录类型]</strong> 和[!UICONTROL附加模板] <strong>[!UICONTROL Action]</strong>)需要其他信息（例如对象ID和模板ID）。</p> <p>有关各个字段的详细信息，请参阅 <a href="http://developer.workfront.com/">Workfront开发人员文档</a>. </p> 
    <ol> 
     <li value="1"> <p>从 [!DNL Workfront] 开发人员文档页面。 以下类型有其自己的页面：</p> 
      <ul> 
       <li> <p>[!UICONTROL项目]</p> </li> 
       <li> <p>[!UICONTROL任务]</p> </li> 
       <li> <p>[!UICONTROL问题]</p> </li> 
       <li> <p>[!UICONTROL用户]</p> </li> 
       <li> <p>[!UICONTROL文档]</p> </li> 
      </ul> <p>对于所有其他记录类型，请选择 <b>[!UICONTROL其他对象和端点]</b>，并在按字母顺序排序的页面上找到记录类型。</p> </li> 
     <li value="2"> <p>在相应记录类型的页面上，搜索（Ctrl-F或Cmd-F）操作。</p> </li> 
     <li value="3"> <p>查看所选操作下可用字段的描述。</p> </li> 
    </ol> <p>注释:  <p>通过 [!DNL Workfront] [!UICONTROL Misc Action]模块，最佳做法是创建没有任何高级选项的校样，然后使用 [!DNL Workfront Proof] SOAP API。</p> <p>有关使用创建校样的更多信息 [!DNL Workfront] API（此模块使用的API），请参阅 <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">通过创建校样时，添加高级校样选项 [!DNL Adobe Workfront] API</a></p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>输入或映射唯一 [!DNL Workfront] 您希望模块与之交互的记录的ID。<p>要获取ID，请打开 [!DNL Workfront] 对象，并复制URL末尾的“ID=”后的文本。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 读取记录]**

此操作模块从单个记录中检索数据。

您指定记录的ID。 您还可以指定希望模块读取的相关记录。

例如，如果模块正在读取的记录是项目，则可以指定要读取项目的任务。

模块会从您指定输出的标准字段中返回一个数据数组。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL连接]</td>

<td> <p>有关连接 [!DNL Workfront] 应用程序 [!DNL Workfront Fusion]，请参阅 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">连接 [!DNL Workfront] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL记录类型]</td>

<td>选择 [!DNL Workfront] 您希望模块读取的对象类型。</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL输出]</td>

<td> <p>选择要包含在此模块的输出包中的信息。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL引用]</td>
   <td>选择要包含在输出中的任何引用字段。</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL收藏集]</td>
   <td>选择要包含在输出中的任何引用字段。</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL ID]</td>
   <td> <p>输入唯一 [!DNL Workfront] 您希望模块读取的记录的ID。</p> <p>要获取ID，请打开 [!DNL Workfront] 对象，并复制URL末尾的“ID=”后的文本。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 更新记录]**

此操作模块会更新对象，如项目、任务或问题。 利用模块，可选择模块中可用对象的哪些字段。

您指定记录的ID。

模块会返回对象的ID和任何关联的字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Workfront] 应用程序 [!DNL Workfront Fusion]，请参阅 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">连接 [!DNL Workfront] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>输入唯一 [!DNL Workfront] 要更新模块的记录的ID。</p> <p>要获取ID，请打开 [!DNL Workfront] 对象，并复制URL末尾的“ID=”后的文本。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>选择 [!DNL Workfront] 记录您希望模块更新。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>选择要用于数据输入的字段。 这样，您就无需滚动浏览您不需要的字段即可使用这些字段。</td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* 输入对象的ID时，您可以开始键入对象的名称，然后从列表中选择该对象。 然后，模块在字段中输入相应的ID。
>* 输入自定义字段或 [!UICONTROL 注意] 对象（注释或回复），您可以在 [!UICONTROL 注释文本] 字段来创建富文本，如粗体或斜体文本。
>
>  有关更新中富文本的更多信息，请参阅 [向工作项添加更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

+++

+++ **[!UICONTROL 上载文档]**

此操作模块将文档上传到 [!DNL Workfront] 对象，如项目、任务或问题。

指定文档的位置、要上传的文件，以及文件的可选新名称。

模块会返回文档的ID和任何关联字段，以及连接所访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Workfront] 应用程序 [!DNL Workfront Fusion]，请参阅 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">连接 [!DNL Workfront] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL相关记录ID]</td> 
   <td>输入唯一 [!DNL Workfront] 要将文档上传到的记录的ID。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL相关记录类型]</td> 
   <td>选择 [!DNL Workfront] 记录您希望模块上传文档的位置。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module).

+++

### 搜索

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL 读取相关记录]**

此搜索模块读取与您在特定父对象中指定的搜索查询匹配的记录。

您可以指定要在输出中包含哪些字段。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Workfront] 应用程序 [!DNL Workfront Fusion]，请参阅 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">连接 [!DNL Workfront] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL记录类型]</td> 
   <td> <p>选择要读取其关联记录的父记录(Workfront对象)的类型。</p> <p>查看 [!DNL Workfront] 可以在 <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] 每个 [!DNL Workfront] 模块</a> 在本文中。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL父记录ID]</td> 
   <td> <p>输入或映射要读取其关联记录的父记录的ID。</p> <p>要获取ID，请打开 [!DNL Workfront] 对象，并复制URL末尾的“ID=”后的文本。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL收藏集]</td> 
   <td>选择或映射希望模块读取的子记录类型。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块的输出包中的信息。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 搜索]**

此搜索模块在 [!DNL Workfront] 与您指定的搜索查询匹配。

您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Workfront] 应用程序 [!DNL Workfront Fusion]，请参阅 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">连接 [!DNL Workfront] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL记录类型]</td> 
   <td> <p>选择 [!DNL Workfront] 记录您希望模块搜索的内容。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL结果集]</td> 
   <td>选择一个选项，以指定您希望模块获得与您的搜索条件匹配的第一个结果还是与之匹配的所有结果。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal]</td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL搜索标准]</td> 
   <td> <p>输入要搜索的字段、要在查询中使用的运算符，以及要在字段中搜索的值。</p> <p>注意：请勿使用 <code>username </code>中。 包括 <code>username </code>在API查询中 [!DNL Workfront] 将用户记录到Workfront，则搜索将失败。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL输出]</td> 
   <td> <p>选择要包含在此模块输出中的字段。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL引用]</td> 
   <td>选择要包含在搜索中的任何引用字段。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL收藏集]</td> 
   <td>选择要添加到搜索的任何收藏集。</td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模块](#workfront-object-types-available-for-each-workfront-module).

+++

## [!DNL Workfront] 每个 [!DNL Workfront] 模块

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**每个对象可用的对象类型 [!DNL Workfront] 触发模块**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL监视记录]</th> 
   <th>[!UICONTROL监视字段]</th> 
   <th>[!UICONTROL Watch Events]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>批准流程</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>分配</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>基线</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 开票记录 </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>记帐费率</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>仪表板</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文档</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文件文件夹</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>文档请求</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>文档版本</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>费用</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>费用类型</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>组</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>小时</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>小时数类型</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>问题</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>迭代</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>工作角色</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>日志条目</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑路径</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>注释</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>注释标签</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>项目组合</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>项目群</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>项目用户</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>保留时间* </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>报告</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
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
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任务</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>团队</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>模板</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>模板任务</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>时间表</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
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

+++**每个对象可用的对象类型 [!DNL Workfront] 操作模块**

>[!NOTE]
>
>的 [!UICONTROL 下载文档] 此表中未包含模块，因为 [!DNL Workfront] 对象类型未包含在其配置中。

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
   <th>[!UICONTROL创建记录]</th> 
   <th>[!UICONTROL更新记录]</th> 
   <th>[!UICONTROL删除记录]</th> 
   <th>[!UICONTROL上传文档]</th> 
   <th>[!UICONTROL读取记录]</th> 
   <th>[!UICONTROL自定义API调用]</th> 
   <th>[!UICONTROL杂项操作]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>批准流程</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>分配</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>开票记录</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>记帐费率</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文档</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文件文件夹</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文档版本</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>费用</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>费用类型</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>组</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>小时</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>小时数类型</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>问题</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>迭代</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>工作角色</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>日志条目</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>里程碑</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑路径</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>注释</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>注释标签</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>项目组合</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>项目群</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>项目用户</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>保留时间* </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>风险</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>风险类型</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>步骤审批者</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任务</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>团队</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>模板</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>模板任务</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>时间表</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>更新</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**每个对象可用的对象类型 [!DNL Workfront] 搜索模块**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL搜索]</th> 
   <th>[!UICONTROL读取相关记录]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>批准流程</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>分配</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>开票记录</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>记帐费率</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文档</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文件文件夹</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文档版本</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>费用</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>费用类型</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>组</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>小时</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>小时数类型</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>问题</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>迭代</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>工作角色</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>日志条目</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑路径</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>注释</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>注释标签</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>项目组合</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>项目群</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>项目用户</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>保留时间* </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>风险</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>风险类型</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>步骤审批者</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任务</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>团队</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>模板</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>模板任务</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>时间表</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>用户委托</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

我们建议您仔细检查，以确保按预期方式运行。

+++

## 中的事件订阅过滤器 [!DNL Workfront] > [!UICONTROL 观看事件] 模块

>[!NOTE]
>
>我们强烈建议在 [!UICONTROL 观看事件] 模块。

的 [!DNL Workfront] [!UICONTROL 观看事件] 模块会根据webhook触发方案，该webhook会在 [!DNL Workfront] API。 事件订阅是一组数据，用于确定将哪些事件发送到Webhook。 例如，如果您将 [!UICONTROL 观看事件] 模块，则事件订阅只发送与问题相关的事件。

通过使用事件订阅过滤器，Fusion用户可以创建更适合其用例的事件订阅。 例如，您可以在 [!DNL Workfront] API将特定项目中的问题仅发送到WebHook，以确保 [!UICONTROL 观看事件] 模块将仅触发该项目中的问题。 创建更窄触发器的功能，可通过减少不相关触发器的数量来改进方案设计。

这与在 [!DNL Workfront Fusion] 情景。 如果没有事件订阅过滤器，您的WebHook将接收与您选择的对象类型相关的所有事件。 这些事件中的大多数都与情景无关，必须先过滤掉，然后情景才能继续。

>[!NOTE]
>
>无法编辑现有 [!DNL Workfront] 网络挂钩。 为 [!DNL Workfront] 事件订阅，删除当前webhook并创建新webhook。

>[!INFO]
>
>**示例：** 请考虑一种方案，该方案会处理分配给特定用户Ana的新问题。
>
>### 使用事件订阅过滤器过滤事件（推荐）
>
>使用事件过滤器，您可以设置Webhook以在创建问题时将问题分配给Ana时触发方案。 Ana的用户ID为b378489d8f7cd3cee0539260720a84b7。
>
>![](assets/event-filter-watch-events-350x277.png)
>
>如果一天内创建了100个问题，但其中只有两个问题被分配给Ana，则此方案将执行两次。
>
>### 在方案中过滤事件（不推荐）
>
>要过滤事件以便仅处理分配给Ana的问题，您可以在 [!UICONTROL 观看事件] 模块。
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>如果一天内创建了100个问题，但其中只有两个问题被分配给Ana，则此方案将执行100次。 其中98项执行将在筛选器处停止，但触发器模块仍在使用数据并在所有执行中执行操作。

有关事件订阅的更多信息，请参阅 [常见问题解答 — 事件订阅](../../wf-api/general/event-subs-faq.md).

有关Web挂接的更多信息，请参阅 [中的即时触发器(Webhook) [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

有关情景中过滤器的更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).
