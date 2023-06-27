---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Box模块
description: 在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用Box的工作流，并将其连接到多个第三方应用程序和服务。 监视指定的文件夹，以检查文件更改、修改和删除现有文件，或将新文件上传到文件夹。
author: Becky
feature: Workfront Fusion
exl-id: 965ce570-40bf-474d-b318-0d2de8be6b9d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1070'
ht-degree: 0%

---

# Box模块

在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL Box]，并将其连接到多个第三方应用程序和服务。 监视指定的文件夹，以检查文件更改、修改和删除现有文件，或将新文件上传到文件夹。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). 有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用 [!DNL Box] 模块，您必须具有 [!DNL Box] 帐户。

## [!DNL Box] 模块及其字段

配置时 [!DNL Box] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Box] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 触发器

* [[!UICONTROL 新建事件]](#new-event)
* [[!UICONTROL 关注文件]](#watch-files)

#### [!UICONTROL 新建事件]

此即时触发器模块会在添加、移动、复制、删除、锁定或解锁文件时启动方案。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook]</td> 
   <td> <p>选择要用于监视传出消息的webhook。 要添加webhook，请单击 <strong>[！UICONTROL添加]</strong> 并输入webhook的名称和连接。</p> <p> 有关将您的[！UICONTROL Box]帐户连接到[！UICONTROL Workfront Fusion]的说明，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到[！UICONTROL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[！UICONTROL Adobe Workfront Fusion]中创建方案</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL返回的最大事件数]</p> </td> 
   <td> <p>输入您希望模块在每个方案执行周期内返回的最大事件数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 关注文件]

此触发器模块会在添加新文件或更新受监视文件夹中的现有文件时启动一个方案。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>有关连接 [!DNL Box] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  <tr> 
   <td role="rowheader">观看</td> 
   <td> <p>选择要监视的文件类型。</p> 
    <ul> 
     <li> <p><strong>仅新文件</strong> </p> <p>添加新文件后，将开始此方案。</p> </li> 
     <li> <p><strong>新文件和所有更改</strong> </p> <p>当添加文件，或修改文件内容或文件属性（如其名称）时，即会启动该方案。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>最大下载文件数</p> </td> 
   <td> <p>输入您希望模块在每个方案执行周期内返回的最大文件数。</p> </td> 
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

指定文件。 您还可以为文件提供新文件名。

该模块返回文件的ID和任何关联的字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Box] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择一个源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>如果此模块不成功，请考虑以下事项：
>
>* 文件大小可能超过您的最大文件大小限制 [!DNL Box] 计划，或者您可能已使用所有 [!DNL Box] 帐户的存储配额。 要获得更多存储空间，请从删除现有文件 [!DNL Box] 或升级 [!DNL Box] 帐户。
>* [!DNL Box] 不会将多个同名文件上传到单个文件夹。 如果目标文件夹包含的文件与正在上传的文件同名，则场景运行将终止，并出现错误。 要避免此情况，请重命名文件。 如果要更新文件，请使用 **[!UICONTROL 更新文件]** 模块。

#### [!UICONTROL 更新文件]

此操作模块更新文件。

指定文件的ID。

该模块返回文件的ID和任何关联的字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Box] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件ID]</td> 
   <td>输入或映射您希望模块更新的文件的唯一ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL源文件]</td> 
   <td> <p>从上一个模块中选择一个源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除文件]

此操作模块删除文件。

指定文件的ID。

该模块返回文件的ID和任何关联的字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Box] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件ID]</td> 
   <td>输入或映射您希望模块更新的文件的唯一ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件]

此操作模块下载文件。

指定文件的ID。

该模块返回文件的ID和任何关联的字段，以及连接访问的任何自定义字段和值。 您可以将此信息映射到场景中的后续模块。

>[!NOTE]
>
>此模块在向后续模块提供文件时非常有用。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Box] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
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
