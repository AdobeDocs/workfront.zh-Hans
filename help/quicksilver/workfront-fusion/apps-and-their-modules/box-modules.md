---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: 框模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用Box的工作流，并将其连接到多个第三方应用程序和服务。 监视指定文件夹以检查文件更改、修改和删除现有文件，或将新文件上传到文件夹。
author: Becky
feature: Workfront Fusion
exl-id: 965ce570-40bf-474d-b318-0d2de8be6b9d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 0%

---

# 框模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Box]，并将其连接到多个第三方应用程序和服务。 监视指定文件夹以检查文件更改、修改和删除现有文件，或将新文件上传到文件夹。

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

使用 [!DNL Box] 模块，您必须 [!DNL Box] 帐户。

## [!DNL Box] 模块及其字段

配置 [!DNL Box] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Box] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 触发器

* [[!UICONTROL 新事件]](#new-event)
* [[!UICONTROL 监视文件]](#watch-files)

#### [!UICONTROL 新事件]

此即时触发模块会在添加、移动、复制、删除、锁定或解锁文件时启动一个方案。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>选择要用于监视传出消息的WebHook。 要添加网页挂接，请单击 <strong>[!UICONTROL Add]</strong> 并输入webhook的名称和连接。</p> <p> 有关将您的[!UICONTROL Box]帐户连接到[!UICONTROL Workfront Fusion]的说明，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到[!UICONTROL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!UICONTROL Adobe Workfront Fusion]中创建方案</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL返回事件的最大数]</p> </td> 
   <td> <p>输入您希望模块在每个方案执行周期期间返回的事件数上限。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 监视文件]

当添加新文件或在正在监视的文件夹中更新现有文件时，此触发器模块会启动一个方案。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>有关连接 [!DNL Box] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  <tr> 
   <td role="rowheader">Watch</td> 
   <td> <p>选择要监视的文件类型。</p> 
    <ul> 
     <li> <p><strong>仅新文件</strong> </p> <p>添加新文件后，方案将开始。</p> </li> 
     <li> <p><strong>新文件和所有更改</strong> </p> <p>在添加文件或修改文件内容或文件属性（如其名称）时，会开始这种情况。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>已下载文件的最大数量</p> </td> 
   <td> <p>输入在每个方案执行周期中希望模块返回的最大文件数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 上传] 文件](#upload-a-file)
* [[!UICONTROL 更新文件]](#update-a-file)
* [[!UICONTROL 删除文件]](#delete-a-file)
* [[!UICONTROL 获取文件]](#get-a-file)

#### [!UICONTROL 上传文件]

此操作模块上传文件。

指定文件。 您还可以为文件提供新的文件名。

模块会返回文件的ID和任何关联的字段，以及连接访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Box] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>如果此模块不成功，请考虑以下事项：
>
>* 文件大小可能超过 [!DNL Box] 计划，或者你用了 [!DNL Box] 帐户的存储配额。 要获取更多存储空间，请从 [!DNL Box] 升级 [!DNL Box] 帐户。
>* [!DNL Box] 不会将多个同名文件上载到单个文件夹。 如果目标文件夹包含的文件与上传的文件同名，则运行方案将终止，并出现错误。 要避免出现此情况，请重命名文件。 如果要更新文件，请使用 **[!UICONTROL 更新文件]** 模块。


#### [!UICONTROL 更新文件]

此操作模块会更新文件。

您指定文件的ID。

模块会返回文件的ID和任何关联的字段，以及连接访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Box] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件ID]</td> 
   <td>输入或映射要更新模块的文件的唯一ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除文件]

此操作模块会删除文件。

您指定文件的ID。

模块会返回文件的ID和任何关联的字段，以及连接访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Box] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件ID]</td> 
   <td>输入或映射要更新模块的文件的唯一ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件]

此操作模块下载文件。

您指定文件的ID。

模块会返回文件的ID和任何关联的字段，以及连接访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

>[!NOTE]
>
>此模块可用于向后续模块提供文件。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Box] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件ID]</td> 
   <td>输入或映射要更新模块的文件的唯一ID。</td> 
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
