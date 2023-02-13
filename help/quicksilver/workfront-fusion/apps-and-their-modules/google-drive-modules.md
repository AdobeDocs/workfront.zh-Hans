---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Google驱动器模块
description: 的 [!DNL Adobe Workfront Fusion Google Drive] 模块可让您监视、搜索、创建、更新、删除和管理文件、文件夹或共享驱动器 [!DNL Google Drive].
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2908'
ht-degree: 0%

---

# [!DNL Google Drive] 模块

的 [!DNL Adobe Workfront Fusion] [!DNL Google Drive] 模块可让您监视、搜索、创建、更新、删除和管理文件、文件夹或共享驱动器 [!DNL Google Drive].

在 [!DNL Adobe Workfront Fusion] 方案中，您可以连接 [!DNL Google Drive] 帐户到多个第三方应用程序和服务。

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



## 连接 [!DNL Google Drive] to [!DNL Workfront Fusion]

如果您 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 用户，您需要在 [the [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 为了获得 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密钥].

有关如何创建OAuth客户端(并获取 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密钥])，请参阅 [连接 [!DNL Adobe Workfront Fusion] to [!DNL Google Services] 使用自定义OAuth客户端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

有关连接 [!DNL Google Drive] 帐户 [!UICONTROL Workfront Fusion]，请参阅 [创建连接 [!UICONTROL Adobe Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Google Drive] 模块及其字段

配置 [!DNL Google Drive] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Google Drive] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)



* [触发器](#triggers)
* [操作](#actions)

### 触发器

* [[!UICONTROL 文件夹中的监视文件]](#watch-files-in-folder)
* [[!UICONTROL 观看所有文件]](#watch-all-files)
* [[!UICONTROL 观看共享文件]](#watch-shared-files)
* [[!UICONTROL 观看评论]](#watch-comments)

#### [!UICONTROL 文件夹中的监视文件]

在指定的文件夹中添加或修改文件时检索文件详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL连接] </td>
   <td> <p>有关连接 [!DNL Google Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">连接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL选择要监视的文件夹]</td>
    <td >选择驱动器上要在其中监视文件的文件夹。</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL要监视的文件]</td>
   <td> <p>选择要监视的文件类型。</p> 
    <ul> 
     <li>[!UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL转换 [!DNL Google Documents] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Documents] 。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL转换 [!DNL Google Spreadsheets] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Spreadsheets] 。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL转换 [!DNL Google Slides] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Slides] 。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL转换 [!DNL Google Drawings] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Drawings] 。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Watch]</td>
    <td>选择是要监视新文件和所有更改，还是仅监视新文件。</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL已下载文件的最大数量]</td>
    <td>设置 [!DNL Workfront Fusion] 将在一个周期内下载（每个方案运行的重复次数）。</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看所有文件]

在 [!DNL Google Drive] 添加或修改。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">连接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL要监视的文件]</td> 
   <td> <p>选择要监视的文件类型。</p> 
    <ul> 
     <li>[!UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL转换 [!DNL Google Documents] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Documents] 。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL转换 [!DNL Google Spreadsheets] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Spreadsheets] 。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL转换 [!DNL Google Slides] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Slides] 。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL转换 [!DNL Google Drawings] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Drawings] 。</td>
  </tr>  
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>选择是要监视新文件和所有更改，还是仅监视新文件。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL已下载文件的最大数量]</td> 
   <td>设置 [!DNL Workfront Fusion] 将在一个周期内下载（每个方案运行的重复次数）。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看共享文件]

将新文件共享给您或更新现有共享文件时触发。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">连接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL选择要监视的文件夹]</td> 
   <td>选择要在中监视文件的共享文件夹。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL要监视的文件]</td> 
   <td> <p>选择要监视的文件类型。</p> 
    <ul> 
     <li>[!UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL转换 [!DNL Google Documents] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Documents] 。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL转换 [!DNL Google Spreadsheets] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Spreadsheets] 。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL转换 [!DNL Google Slides] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Slides] 。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL转换 [!DNL Google Drawings] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Drawings] 。</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>选择是要监视新文件和所有更改，还是仅监视新文件。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL已下载文件的最大数量]</td> 
   <td>设置 [!DNL Workfront Fusion] 将在一个周期内下载（每个方案运行的重复次数）。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看评论]

在选定文件上添加或修改注释时触发。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">连接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件]</td> 
   <td>选择要监视的注释文件。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>选择您是要监视所有更改还是仅监视新注释</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回评论的最大数量]</td> 
   <td>设置 [!DNL Workfront Fusion] 将在一个周期中返回（每个方案运行的重复次数）。</td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 上传文件]](#upload-a-file)
* [[!UICONTROL 更新文件]](#update-a-file)
* [[!UICONTROL 复制文件]](#copy-a-file)
* [[!UICONTROL 删除文件]](#delete-a-file)
* [[!UICONTROL 将文件/文件夹移到垃圾桶]](#move-a-filefolder-to-trash)
* [[!UICONTROL 获取文件]](#get-a-file)
* [[!UICONTROL 搜索文件/文件夹]](#search-for-filesfolders)
* [[!UICONTROL 创建文件夹]](#create-a-folder)
* [[!UICONTROL 获取共享链接]](#get-a-share-link)

#### [!UICONTROL 上传文件]

将文件上传到 [!DNL Google Drive].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">连接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Destination]</td> 
   <td> <p>选择要将文件上传到的目标。</p> 
    <ul> 
     <li>[!DNL My Drive]</li> 
     <li>[!DNL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Target文件夹]</td> 
   <td>选择要将文件上传到的文件夹。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL源文件]</td> 
   <td>选择是要使用从前一个模块传入的文件，还是要手动映射文件。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件名]</td> 
   <td>选择文件名。 如果在[!UICONTROL源文件]字段中选择“[!UICONTROL Map]”，则此选项将可用。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL数据]</td> 
   <td>选择要上传的数据文件。 如果在[!UICONTROL源文件]字段中选择“[!UICONTROL Map]”，则此选项将可用。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL标题]</td> 
   <td>输入新文件的标题。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL转换文件]</td> 
   <td>启用此选项后，模块可将文件转换为 [!DNL Google] 格式。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新文件]

更新文件的元数据或内容。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">连接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL目标]</td> 
   <td> <p>选择要将文件上传到的目标。</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL与我共享]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL移动到文件夹]</td> 
   <td>如果要将文件移动到其他文件夹，请选择要将文件移动到的文件夹。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件ID]</td> 
   <td>映射要更新的文件的ID。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL标题]</td> 
   <td>输入更新文件的标题。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL更改文件内容]</td> 
   <td>选择是否要替换文件的内容。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL源文件]</td> 
   <td>选择是要使用从前一个模块传入的文件，还是要手动映射文件。 如果您选择更改前一个字段中的文件内容，则此字段将可用。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件名]</td> 
   <td>选择文件名。 如果在[!UICONTROL源文件]字段中选择“[!UICONTROL Map]”，则此选项将可用。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL数据]</td> 
   <td>选择要上传的数据文件。 如果在[!UICONTROL源文件]字段中选择“[!UICONTROL Map]”，则此选项将可用。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 复制文件]

将文件复制到新位置。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">连接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL目标]</td> 
   <td> <p>选择要将文件上传到的目标。</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL与我共享]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Target文件夹]</td> 
   <td>选择要复制的文件所在的文件夹/</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件ID]</td> 
   <td>映射要更新的文件的ID。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL副本的名称]</td> 
   <td>输入新文件的标题。 如果您不想更改原始文件名，请将此字段留空。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除文件]

永久删除文件或文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">连接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件ID]</td> 
   <td>映射要删除的文件的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将文件/文件夹移到垃圾桶]

将文件或文件夹移到垃圾桶。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">连接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件ID]</td> 
   <td>将要移动到垃圾桶的文件的ID映射。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件]

检索具有指定ID的文件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">连接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL转换 [!DNL Google Documents] 要格式化的文件]</td> 
   <td>选择要转换的文件格式 [!DNL Google Documents] 。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL转换 [!DNL Google Spreadsheets] 要格式化的文件]</td> 
   <td>选择要转换的文件格式 [!DNL Google Spreadsheets] 。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL转换 [!DNL Google Slides] 要格式化的文件]</td> 
   <td>选择要转换的文件格式 [!DNL Google Slides] 。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL转换 [!DNL Google Drawings] 要格式化的文件]</td> 
   <td>选择要转换的文件格式 [!DNL Google Drawings] 。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件ID]</td> 
   <td>映射要检索的文件的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索文件/文件夹]

根据搜索条件搜索文件或文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">连接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL目标]</td> 
   <td> <p>选择要搜索的目标。</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL与我共享]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL列出文件夹]</td> 
   <td>导航到要搜索文件或文件夹的文件夹。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL检索]</td> 
   <td> <p> 选择是要搜索文件、文件夹，还是同时搜索两者。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL搜索]</p> </td> 
   <td> <p>选择要执行的搜索类型。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL在文件/文件夹名称内搜索]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL查询]</strong> </p> <p>输入要搜索的部分文件名或完整文件名（包括后缀）。</p> </li> 
       <li> <p><strong>[!UICONTROL搜索选项]</strong> </p> <p>选择是要搜索确切的搜索词，还是要搜索包含搜索词的名称。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL全文]搜索</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL查询]</strong> </p> <p>输入您想要在您的 [!DNL Google Drive].</p> </li> 
      </ul> </li> 
     <li> <p><strong>输入自定义搜索查询</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL查询]</strong> </p> <p>输入自定义搜索查询。 有关更多详细信息，请参阅本文的[!UICONTROL搜索文件]部分。</p> </li> 
       <li> <p><strong>将上面选择的文件夹添加到查询中</strong> </p> <p>在父收藏集中搜索文件夹。 这将查找直接位于上述选定文件夹中的所有文件和文件夹。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回结果的最大数]</td> 
   <td>设置文件或文件夹的最大数量 [!DNL Workfront Fusion] 将在一个执行周期中返回。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL即使模块未返回任何结果，仍继续执行路由]</td> 
   <td>启用此选项可确保在模块未返回任何结果时不停止方案。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建文件夹]

在指定位置中创建文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">连接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL目标]</td> 
   <td> <p>选择要将文件上传到的目标。</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL与我共享]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL新文件夹位置]</td> 
   <td>导航到要创建新文件夹的位置。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL新文件夹的名称]</td> 
   <td>输入要创建的文件夹的名称。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL共享文件夹]</td> 
   <td>如果要通过[!UICONTROL Share]链接与任何人共享文件夹，请选择此选项。 否则，共享链接仅供所有者使用。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取共享链接]

检索Google驱动器中文件的共享链接。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">连接 [!DNL Google Drive] 到[!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件ID]</td> 
   <td>映射要获取其共享链接的文件ID。</td> 
  </tr> 
 </tbody> 
</table>

## 疑难解答

### 无法上载或更新文件

上传或更新文件失败时，可能会出现以下几种情况：

* 上传的文件太大，超出了您允许的最大文件大小限制 [!DNL Google Drive] 计划或超出 [!DNL Google Drive] 存储限制。 您可以升级存储计划或从 [!DNL Google Drive] 服务。
* 要将文件上传到的选定文件夹不再存在。 方案停止，然后需要再次选择目标文件夹。

## 搜索文件

在文件夹的模块List文件中，您可以使用自己的查询，该查询包含以下部分：

* **[!UICONTROL 字段]**  — 正在搜索的文件的属性，例如属性 `name` 文件。

* **[!UICONTROL 运算符]**  — 对数据执行的测试以提供匹配，例如 `contains`.

* **[!UICONTROL 值]**  — 测试的属性的内容，例如文件名 `My cool document`.

将子句与连词组合 `and` 或 `or`，和对查询否定 `not`.

* [字段](#fields)
* [值类型](#value-types)
* [运算符](#operators)
* [示例](#examples)

### 字段

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>字段 </th> 
   <th>值类型 </th> 
   <th>运算符</th> 
   <th> <p> 描述</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>[!UICONTROL title]</code></td> 
   <td>字符串</td> 
   <td><code>contains</code><sup>1</sup>, <code>=</code>, <code>!=</code></td> 
   <td> <p> 文件的名称。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL fullText]</code> </td> 
   <td>字符串 </td> 
   <td><code>contains</code><sup>2, 3</sup> </td> 
   <td> <p> 文件的全文，包括名称、描述、内容和可索引文本。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL mimeType]</code> </td> 
   <td> 字符串</td> 
   <td><code>contains</code>, <code>=</code>, <code>!=</code></td> 
   <td> <p> 文件的MIME类型。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL modifiedDate]</code> </td> 
   <td> 日期<sup>4</sup></td> 
   <td><code> &lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> 上次修改文件的日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL lastViewedByMeDate]</code> </td> 
   <td> 日期<sup>4</sup></td> 
   <td><code>&lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> 用户上次查看文件的日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL trashed]</code></td> 
   <td>布尔 </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> 文件是否在垃圾桶中。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL starred]</code></td> 
   <td>布尔 </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p>文件是否有星号。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL parents]</code></td> 
   <td>收藏集 </td> 
   <td><code>in </code> </td> 
   <td> <p>[!UICONTROL父代]集合是否包含指定的ID。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL owners]</code></td> 
   <td>收藏集 </td> 
   <td><code>in </code> </td> 
   <td> <p>拥有文件的用户。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL writers]</code></td> 
   <td>收藏集 </td> 
   <td><code>in </code> </td> 
   <td> <p>有权修改文件的用户。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL readers] </code> </td> 
   <td>收藏集 </td> 
   <td><code>in </code> </td> 
   <td> <p>有权读取文件的用户。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL sharedWithMe]</code> </td> 
   <td>布尔 </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> 用户“与我共享”收藏集中的文件。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL properties] </code> </td> 
   <td>收藏集</td> 
   <td><code>has </code> </td> 
   <td> <p> 公共自定义文件属性。</p> </td> 
  </tr> 
 </tbody> 
</table>

请考虑以下有关这些字段中运算符的信息：

* 的 `contains` 运算符仅执行前缀匹配 `title`.

   例如，标题“HelloWorld”与 `title contains 'Hello'` 但不是 `title contains 'World'`.

* 的 `contains` 运算符仅对整个字符串令牌执行匹配 `fullText`.

   例如，如果文档的全文仅包含查询字符串“HelloWorld” `fullText contains 'HelloWorld'` 返回结果。 查询，例如 `fullText contains 'Hello'` 不会在此情景中返回结果。

* 的 `contains` 运算符与精确的字母数字短语匹配（如果它被双引号括住）。

   例如，如果 `fullText` 文档中包含字符串“Hello ther world”，然后是查询 `fullText contains '"Hello there"'` 返回结果，但查询 `fullText contains '"Hello world"'` 不会。

   此外，由于搜索是字母数字，因此如果 `fullText` 文档包含字符串“Hello_world”，然后包含查询 `fullText contains '"Hello world"'` 返回结果。

* 字段 `type` 日期当前不能相互比较，只能与固定日期比较。

### 值类型

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>值类型</th> 
   <th> <p> 注释</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>字符串 </td> 
   <td> <p>带单引号'。 对查询中的单引号进行转义 <code>\'</code>，例如，<code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>布尔值 </td> 
   <td> <p><code>true </code>或 <code>false</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>日期 </td> 
   <td> <p>RFC 3339格式，默认时区为UTC，例如 <code>2012-06-04T12:00:00-08:00</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 运算符

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>运算符 </th> 
   <th> <p>注释</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>contains</code></td> 
   <td> <p>一个字符串的内容存在于另一个字符串中。</p> </td> 
  </tr> 
  <tr> 
   <td><code>=</code> </td> 
   <td> <p> 字符串或布尔值的内容等于另一个。</p> </td> 
  </tr> 
  <tr> 
   <td><code>!=</code> </td> 
   <td> <p> 字符串或布尔值的内容不等于另一个。</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;</code> </td> 
   <td> <p> 日期早于其他日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;=</code> </td> 
   <td> <p> 日期早于或等于其他日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>></code> </td> 
   <td> <p> 日期晚于其他日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>>=</code> </td> 
   <td> <p> 日期晚于或等于其他日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>in </code> </td> 
   <td> <p>元素包含在集合中。</p> </td> 
  </tr> 
  <tr> 
   <td><code>and </code> </td> 
   <td> <p>返回与两个子句都匹配的文件。</p> </td> 
  </tr> 
  <tr> 
   <td><code>or </code> </td> 
   <td> <p>返回与任一子句匹配的文件。</p> </td> 
  </tr> 
  <tr> 
   <td><code>not </code> </td> 
   <td> <p>否定搜索子句。</p> </td> 
  </tr> 
  <tr> 
   <td><code>has </code> </td> 
   <td> <p>集合包含与参数匹配的元素。</p> </td> 
  </tr> 
 </tbody> 
</table>

对于复合子句，可以使用圆括号将子句分组在一起。 例如：
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` 此搜索会返回MIME类型为其上次修改时间为2012年6月4日之后的所有图像或视频文件。 因为 `and` 和 `or` 运算符从左到右进行评估（不带圆括号），上例将仅返回在2012年6月4日之后修改的图像，但将返回所有视频，即使是在2012年6月4日之前也是如此。

### 示例

本页上的所有示例都显示未编码的 `<q>q</q>` 参数，其中 `title = 'hello'` 编码为 `title+%3d+%27hello%27`. 客户端库会自动处理此编码。

* 搜索名为“hello”的文件

   <pre>title = 'hello'</pre>
* 使用特定于文件夹的MIME类型搜索文件夹

   <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* 搜索非文件夹的文件

   <pre>mimeType != 'application/vnd.google-apps.folder'</pre>
* 搜索名称包含“hello”和“goodbye”字样的文件

   <pre>标题包含“hello”，而[!UICONTROL name]包含“goodbye”</pre>
* 搜索名称中不包含“hello”字样的文件

   <pre>不包含“hello”的标题</pre>
* 搜索内容中包含“hello”一词的文件

   <pre>fullText包含“hello”</pre>
* 搜索内容中不包含“hello”一词的文件

   <pre>not fullText包含“hello”</pre>
* 搜索内容中包含精确短语“hello world”的文件

   <pre>fullText包含“hello world”的fullText包含“hello_world”</pre>
* 搜索包含“\”字符的查询（例如“\authors”）的文件

   <pre>fullText包含“\\authors”</pre>
* 搜索用户“test@example.org”可写的文件

   <pre>“test@example.org”在 [!DNL writers]</pre>
* 搜索ID `1234567` 在 `parents` 收藏集。 这会查找ID为的文件夹中直接存在的所有文件和文件夹 `1234567`.

   <pre>[!UICONTROL父母]中的“1234567”</pre>
* 搜索别名ID `appDataFolder` 在 `parents` 收藏集。 这会查找位于 [应用程序数据文件夹](https://developers.google.com/drive/api/v2/appdata).

   <pre>父项中的“appDataFolder”</pre>
* 搜索用户“test@example.org”和“test2@example.org”可写的文件

   <pre>作家的“test@example.org”和作家的“test2@example.org”</pre>
* 搜索垃圾桶中包含“重要”文本的文件

   <pre>fullText包含“important”，并且trashed = true</pre>
* 搜索在2012年6月4日之后修改的文件

   <pre>modifiedDate &gt; '2012-06-04T12:00:00' //默认时区为UTC</pre><pre>modifiedDate &gt; '2012-06-04T12:00:00-08:00'</pre>
* 搜索名称中带有“hello”的授权用户共享的文件

   <pre>sharedWithMe和title包含“hello”</pre>
* 搜索带有 [自定义文件属性](https://developers.google.com/drive/api/v2/properties) 已命名 `additionalID` 值 `8e8aceg2af2ge72e78`.

   <pre>属性具有{ key='additionalID' and value='8e8aceg2af2ge72e78' and visibility='PRIVATE' }</pre>

本指南的来源是 [[!DNL Google Drive] 文档](https://developers.google.com/drive/api/v2/search-shareddrives).
