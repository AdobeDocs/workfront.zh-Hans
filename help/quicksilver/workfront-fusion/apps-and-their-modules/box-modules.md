---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: 盒式模块
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: 965ce570-40bf-474d-b318-0d2de8be6b9d
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1117'
ht-degree: 0%

---

# 盒式模块

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [Box模块](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/box-modules.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

在[!DNL Adobe Workfront Fusion]方案中，您可以自动使用[!DNL Box]的工作流，并将其连接到多个第三方应用程序和服务。 监视指定的文件夹，以检查文件更改、修改和删除现有文件，或将新文件上传到文件夹。

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

要使用[!DNL Box]模块，您必须具有[!DNL Box]帐户。

## 框API信息

Box连接器使用下列方法：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基本URL</td> 
   <td> https://api.box.com/2.0
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API版本</td> 
   <td> v2.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API标记</td> 
   <td>v3.0.3</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Box]模块及其字段

配置[!DNL Box]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL Box]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)

### 触发器

* [[!UICONTROL 新事件]](#new-event)
* [[!UICONTROL 监视文件]](#watch-files)

#### [!UICONTROL 新事件]

此即时触发器模块会在添加、移动、复制、删除、锁定或解锁文件时启动方案。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook]</td> 
   <td> <p>选择要用于监视传出消息的webhook。 要添加webhook，请单击<strong>[！UICONTROL添加]</strong>并输入webhook的名称和连接。</p> <p> 有关将[！UICONTROL Box]帐户连接到[！UICONTROL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[！UICONTROL Adobe Workfront Fusion]</a>中创建方案中的文章<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL返回的最大事件数]</p> </td> 
   <td> <p>输入您希望模块在每个方案执行周期中返回的最大事件数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 监视文件]

在监视的文件夹中添加新文件或更新现有文件时，此触发器模块将启动一个方案。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>有关将[!DNL Box]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  <tr> 
   <td role="rowheader">观看</td> 
   <td> <p>选择要监视的文件类型。</p> 
    <ul> 
     <li> <p><strong>仅新文件</strong> </p> <p>添加新文件后，将开始此方案。</p> </li> 
     <li> <p><strong>新文件和所有更改</strong> </p> <p>当添加文件，或修改文件内容或文件属性（如文件名称）时，将开始使用此方案。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>最大下载文件数</p> </td> 
   <td> <p>输入您希望模块在每个方案执行周期中返回的最大文件数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 上传]文件](#upload-a-file)
* [[!UICONTROL 更新文件]](#update-a-file)
* [[!UICONTROL 删除文件]](#delete-a-file)
* [[!UICONTROL 获取文件]](#get-a-file)

#### [!UICONTROL 上载文件]

此操作模块上传文件。

指定文件。 您还可以为文件提供新的文件名。

模块会返回文件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Box]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source file]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>如果此模块不成功，请考虑以下事项：
>
>* 文件大小可能超过[!DNL Box]计划的最大文件大小限制，或者您可能已使用所有[!DNL Box]帐户的存储配额。 若要获得更多存储空间，请从[!DNL Box]中删除现有文件或升级您的[!DNL Box]帐户。
>* [!DNL Box]不会将多个同名文件上载到单个文件夹。 如果目标文件夹包含的文件与要上传的文件同名，则场景运行将终止，并出现错误。 要避免此情况，请重命名文件。 如果要更新文件，请使用&#x200B;**[!UICONTROL 更新文件]**&#x200B;模块。

#### [!UICONTROL 更新文件]

此操作模块可更新文件。

指定文件的ID。

模块会返回文件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Box]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件ID]</td> 
   <td>输入或映射您希望模块更新的文件的唯一ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source file]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除文件]

此操作模块删除文件。

指定文件的ID。

模块会返回文件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Box]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件ID]</td> 
   <td>输入或映射您希望模块更新的文件的唯一ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件]

此操作模块将下载文件。

指定文件的ID。

模块会返回文件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

>[!NOTE]
>
>此模块在向后续模块提供文件时非常有用。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Box]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!DNL Adobe Workfront Fusion]的连接 — 基本说明</a>。</p> </td> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件ID]</td> 
   <td>输入或映射您希望模块更新的文件的唯一ID。</td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Possible problems</h2>
-->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This is drafted out because we don't have a download module for Box yet</p>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Watch files trigger module doesn't download a file contained in the folder.</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">There are several situations when downloading a file fails:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The current file lock setting does not allow the file to be downloaded or the downloading of the file is disabled. In this case, the file is ignored.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the scenario started, the file was being uploaded to the server and was not ready to be downloaded. The scenario run gets stopped and Workfront Fusion tries downloading the file again during the next execution of the scenario.</li>
  -->
