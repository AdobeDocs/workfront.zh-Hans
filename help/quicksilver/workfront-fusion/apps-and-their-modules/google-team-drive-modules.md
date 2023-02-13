---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Google Team Drive模块
description: 的 [!DNL Adobe Workfront Fusion Google Team Drive] 模块可让您监视、上传、更新、复制、删除或检索文件，以及在 [!DNL Google Shared] 开车。
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 0%

---

# [!DNL Google Team Drive] 模块

的 [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] 模块可让您监视、上传、更新、复制、删除或检索文件，以及在 [!DNL Google Shared Drive].

为了使用 [!DNL Google Team Drive] with [!DNL Adobe Workfront Fusion]，则需要具有 [!DNL G Suite] 帐户。 如果您没有，则可以创建 [!DNL G Suite] 帐户 [[!DNL G Suite] 注册网站](https://gsuite.google.com/signup/businessstarter/welcome).

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Google Team Drive]，并将其连接到多个第三方应用程序和服务。

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

使用 [!DNL Google Team Drive] 模块，您必须 [!DNL Google Team Drive].

## [!DNL Google Team Drive] 模块及其字段

配置 [!DNL Google Team Drive] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Google Team Drive] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

中显示的模块对话框字段 **粗体** (在 [!DNL Workfront Fusion] 方案， **not** )是必填项。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 触发器

#### [!UICONTROL 监视文件]

在指定的文件夹中添加和/或修改新文件时，返回文件详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Team Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> 选择要监视的共享驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>选择共享驱动器中的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL要监视的文件]</td> 
   <td> <p> 选择要监视的文件类型。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL转换 [!DNL Google Documents] 要格式化的文件] </td> 
   <td> <p>选择您希望监视的格式 [!DNL Google Documents] 文件转换为。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL转换 [!DNL Google Sheets] 要格式化的文件] </td> 
   <td> <p>选择您希望监视的格式 [!DNL Google Sheets] 文件转换为。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL转换 [!DNL Google Slides] 要格式化的文件] </td> 
   <td> <p>选择您希望监视的格式 [!DNL Google Slides] 文件转换为。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL转换 [!DNL Google Drawings] 要格式化的文件] </td> 
   <td> <p>选择您希望监视的格式 [!DNL Google Drawings] 文件转换为。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p> 选择是要监视新文件和已修改文件的文件夹，还是仅监视新文件的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL已下载文件的最大数量]</td> 
   <td> <p> 设置最大文件数 [!DNL Workfront Fusion] 将在一个执行周期中返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 上传文件]](#upload-a-file)
* [[!UICONTROL 更新文件]](#update-a-file)
* [[!UICONTROL 复制文件]](#copy-a-file)
* [[!UICONTROL 删除文件]](#delete-a-file)
* [[!UICONTROL 将文件移到垃圾桶]](#move-a-file-to-trash)
* [[!UICONTROL 获取文件]](#get-a-file)
* [[!UICONTROL 获取文件列表]](#get-a-file-list)
* [[!UICONTROL 创建文件夹]](#create-a-folder)

#### [!UICONTROL 上传文件]

将文件上载到指定的共享驱动器。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Team Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive] </td> 
   <td> <p>选择要将文件上传到的共享驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>选择共享驱动器中的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL源文件]</p> </td> 
   <td> <p>指定要上传到共享驱动器的文件。</p> <p>映射要从上一个模块上传的文件(例如，[!UICONTROL HTTP] &gt;[!UICONTROL获取文件]或[!UICONTROLDropbox] &gt;[!UICONTROL获取文件)]，或手动输入文件名和文件数据。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL标题]</td> 
   <td> <p> 输入将在共享文件夹中显示的文件的标题。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL转换文件]</td> 
   <td> <p> 启用此选项可将文件转换为共享文件夹中相应的Google格式。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新文件]

用于更改文件名和/或文件内容。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Team Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> 选择包含要更新的文件的共享驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>选择共享驱动器中的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件ID]</td> 
   <td> <p> 输入（映射）要更新的文件的ID。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL源文件]</p> </td> 
   <td>从前一个模块中选择源文件，或映射源文件的名称和数据。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL标题] </td> 
   <td> <p>输入更新文件的新标题。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL转换文件]</td> 
   <td> <p> 启用此选项可将文件转换为 [!DNL Google] 格式。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 复制文件]

将指定的文件复制到所选文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Team Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> 选择包含要复制的文件的共享驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>选择要将文件复制到的目标文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件ID]</td> 
   <td> <p> 输入（映射）要复制的文件的ID。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL复制文件的名称]</p> </td> 
   <td> <p>如果希望在目标位置中更改新文件名，请输入新文件名。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除文件]

删除指定的文件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Team Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件ID]</td> 
   <td> <p> 输入或映射要删除的文件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将文件移到垃圾桶]

将指定的文件移到垃圾桶。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Team Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件ID]</td> 
   <td> <p> 输入或映射要移动到垃圾桶的文件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件]

检索有关指定文件的详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Team Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL转换 [!DNL Google Documents] 要格式化的文件] </td> 
   <td> <p>选择所需的格式 [!DNL Google Documents] 文件转换为。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL转换 [!DNL Google Sheets] 要格式化的文件] </td> 
   <td> <p>选择所需的格式 [!DNL Google Sheets] 文件转换为。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL转换 [!DNL Google Slides] 要格式化的文件] </td> 
   <td> <p>选择所需的格式 [!DNL Google Slides] 文件转换为。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL转换 [!DNL Google Drawings] 要格式化的文件] </td> 
   <td> <p>选择所需的格式 [!DNL Google Drawings] 文件转换为。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件ID]</td> 
   <td> <p> 输入或映射要检索的文件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件列表]

根据搜索词检索文件和/或文件夹详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Team Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> 选择要从中列出文件的共享驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>选择要从中列出文件的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL搜索] </td> 
   <td> <p>选择要执行的搜索类型 — 请参阅下文。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL查询]</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>[!UICONTROL在文件名内搜索]</p> <p style="font-weight: normal;">在选择[!UICONTROL搜索确切搜索词Search]选项时输入文件名（包括文件扩展名），或在选择[!UICONTROL搜索包含搜索词]选项的名称时输入名称的部分。</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL全文搜索]</p> <p>输入搜索词以搜索文件名、描述和内容。</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL自定义搜索查询]</p> <p>输入 [!DNL Google] 搜索查询词。 有关更多详细信息，请参阅 [!DNL Google]'s <a href="https://developers.google.com/drive/api/v2/ref-search-terms">搜索查询文档</a>. 示例: <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL检索]</td> 
   <td>选择是要检索文件、文件夹，还是同时检索两者。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回结果的最大数]</td> 
   <td> <p> 设置文件或文件夹的最大数量 [!DNL Workfront Fusion] 将在一个执行周期中返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建文件夹]

创建新文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Team Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team Drive]</td> 
   <td> <p> 选择要创建文件夹的共享驱动器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>选择要在中创建文件夹的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL新文件夹的名称]</td> 
   <td> <p> 输入新文件夹的名称。</p> </td> 
  </tr> 
 </tbody> 
</table>
