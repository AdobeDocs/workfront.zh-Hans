---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Google驱动器模块
description: 此 [!DNL Adobe Workfront Fusion Google Drive] 通过模块，您可以监视、搜索、创建、更新、删除和管理文件、文件夹或共享驱动器。 [!DNL Google Drive].
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2956'
ht-degree: 0%

---

# [!DNL Google Drive] 模块

此 [!DNL Adobe Workfront Fusion] [!DNL Google Drive] 通过模块，您可以监视、搜索、创建、更新、删除和管理文件、文件夹或共享驱动器。 [!DNL Google Drive].

在 [!DNL Adobe Workfront Fusion] 方案，您可以将 [!DNL Google Drive] 帐户到多个第三方应用程序和服务。

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



## 正在连接 [!DNL Google Drive] 到 [!DNL Workfront Fusion]

如果您是 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 您需要在其上创建OAuth客户端的用户 [此 [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 为了获得 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密码].

有关如何创建OAuth客户端(和获取 [!UICONTROL 客户端ID] 和 [!UICONTROL 客户端密码])，请参见 [Connect [!DNL Adobe Workfront Fusion] 到 [!DNL Google Services] 使用自定义OAuth客户端](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

有关连接 [!DNL Google Drive] 目标帐户 [!UICONTROL Workfront Fusion]，请参见 [创建连接 [!UICONTROL Adobe Workfront Fusion]  — 基本说明](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Google Drive] 模块及其字段

配置时 [!DNL Google Drive] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Google Drive] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)



* [触发器](#triggers)
* [操作](#actions)

### 触发器

* [[!UICONTROL 监视文件夹中的文件]](#watch-files-in-folder)
* [[!UICONTROL 观看所有文件]](#watch-all-files)
* [[!UICONTROL 观看共享文件]](#watch-shared-files)
* [[!UICONTROL 关注评论]](#watch-comments)

#### [!UICONTROL 监视文件夹中的文件]

在指定的文件夹中添加或修改文件时检索文件详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[！UICONTROL连接] </td>
   <td> <p>有关连接 [!DNL Google Drive] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在连接 [!DNL Google Drive] 到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr>
    <td>[！UICONTROL选择要监视的文件夹]</td>
    <td >选择驱动器上要监视文件的文件夹。</td>
  </tr> 
  <tr> 
    <td>[！UICONTROL要监视哪些文件]</td>
   <td> <p>选择要监视的文件类型。</p> 
    <ul> 
     <li>[！UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[！UICONTROL转换 [!DNL Google Documents] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Documents] 到。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL转换 [!DNL Google Spreadsheets] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Spreadsheets] 到。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL转换 [!DNL Google Slides] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Slides] 到。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL转换 [!DNL Google Drawings] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Drawings] 到。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL监视]</td>
    <td>选择是要监视新文件和所有更改，还是只监视新文件。</td>
  </tr> 
  <tr> 
    <td>[！UICONTROL最大下载文件数]</td>
    <td>设置满足以下条件的最大结果数 [!DNL Workfront Fusion] 将在一个周期内下载（每个方案运行的重复次数）。</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看所有文件]

在以下情况下检索文件详细信息： [!DNL Google Drive] 添加或修改。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在连接 [!DNL Google Drive] 到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL要监视哪些文件]</td> 
   <td> <p>选择要监视的文件类型。</p> 
    <ul> 
     <li>[！UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[！UICONTROL转换 [!DNL Google Documents] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Documents] 到。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL转换 [!DNL Google Spreadsheets] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Spreadsheets] 到。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL转换 [!DNL Google Slides] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Slides] 到。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL转换 [!DNL Google Drawings] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Drawings] 到。</td>
  </tr>  
  <tr> 
   <td>[！UICONTROL监视]</td> 
   <td>选择是要监视新文件和所有更改，还是只监视新文件。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最大下载文件数]</td> 
   <td>设置满足以下条件的最大结果数 [!DNL Workfront Fusion] 将在一个周期内下载（每个方案运行的重复次数）。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 观看共享文件]

在将新文件共享给您或更新现有共享文件时触发。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在连接 [!DNL Google Drive] 到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL选择要监视的文件夹]</td> 
   <td>选择要监视文件的共享文件夹。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL要监视哪些文件]</td> 
   <td> <p>选择要监视的文件类型。</p> 
    <ul> 
     <li>[！UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[！UICONTROL转换 [!DNL Google Documents] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Documents] 到。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL转换 [!DNL Google Spreadsheets] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Spreadsheets] 到。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL转换 [!DNL Google Slides] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Slides] 到。</td>
  </tr> 
  <tr>
    <td>[！UICONTROL转换 [!DNL Google Drawings] 要格式化的文件]</td>
    <td>选择要转换的文件格式 [!DNL Google Drawings] 到。</td>
  </tr> 
  <tr> 
   <td>[！UICONTROL监视]</td> 
   <td>选择是要监视新文件和所有更改，还是只监视新文件。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最大下载文件数]</td> 
   <td>设置满足以下条件的最大结果数 [!DNL Workfront Fusion] 将在一个周期内下载（每个方案运行的重复次数）。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 关注评论]

在选定文件上添加或修改评论时触发。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在连接 [!DNL Google Drive] 到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件]</td> 
   <td>选择要监视其注释的文件。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL监视]</td> 
   <td>选择是要监视所有更改，还是只监视新注释</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL返回评论的最大数量]</td> 
   <td>设置符合以下条件的评论的最大数量： [!DNL Workfront Fusion] 将在一个周期内返回（每个方案运行的重复次数）。</td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 上传文件]](#upload-a-file)
* [[!UICONTROL 更新文件]](#update-a-file)
* [[!UICONTROL 复制文件]](#copy-a-file)
* [[!UICONTROL 删除文件]](#delete-a-file)
* [[!UICONTROL 将文件/文件夹移动到垃圾桶]](#move-a-filefolder-to-trash)
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
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在连接 [!DNL Google Drive] 到[！UICONTROL Workfront Fusion]</a></p> </td> 
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
   <td>[！UICONTROL目标文件夹]</td> 
   <td>选择要将文件上传到的文件夹。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL源文件]</td> 
   <td>选择是要使用从上一个模块传入的文件，还是要手动映射文件。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件名]</td> 
   <td>选择文件名。 如果在[！UICONTROL源文件]字段中选择“[！UICONTROL映射]”，则此选项可用。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL数据]</td> 
   <td>选择要上载的数据文件。 如果在[！UICONTROL源文件]字段中选择“[！UICONTROL映射]”，则此选项可用。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL标题]</td> 
   <td>输入新文件的标题。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL转换文件]</td> 
   <td>启用此选项后，模块可以将文件转换为相应的 [!DNL Google] 格式。</td> 
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
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在连接 [!DNL Google Drive] 到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目标]</td> 
   <td> <p>选择要将文件上传到的目标。</p> 
    <ul> 
     <li>[！UICONTROL我的驱动器]</li> 
     <li>[！UICONTROL与我共享]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL移动到文件夹]</td> 
   <td>如果要将文件移动到其他文件夹，请选择要将文件移动到其中的文件夹。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件ID]</td> 
   <td>映射要更新的文件的ID。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL标题]</td> 
   <td>输入更新文件的标题。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL更改文件内容]</td> 
   <td>选择是否要替换文件的内容。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL源文件]</td> 
   <td>选择是要使用从上一个模块传入的文件，还是要手动映射文件。 如果您在上一个字段中选择了更改文件的内容，则此字段可用。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件名]</td> 
   <td>选择文件名。 如果在[！UICONTROL源文件]字段中选择“[！UICONTROL映射]”，则此选项可用。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL数据]</td> 
   <td>选择要上载的数据文件。 如果在[！UICONTROL源文件]字段中选择“[！UICONTROL映射]”，则此选项可用。</td> 
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
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在连接 [!DNL Google Drive] 到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目标]</td> 
   <td> <p>选择要将文件上传到的目标。</p> 
    <ul> 
     <li>[！UICONTROL我的驱动器]</li> 
     <li>[！UICONTROL与我共享]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目标文件夹]</td> 
   <td>选择要复制的文件所在的文件夹/</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件ID]</td> 
   <td>映射要更新的文件的ID。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL副本的名称]</td> 
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
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在连接 [!DNL Google Drive] 到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件ID]</td> 
   <td>映射要删除的文件的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将文件/文件夹移动到垃圾桶]

将文件或文件夹移至垃圾桶。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在连接 [!DNL Google Drive] 到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件ID]</td> 
   <td>将您要移动的文件的ID映射到垃圾桶。</td> 
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
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在连接 [!DNL Google Drive] 到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL转换 [!DNL Google Documents] 要格式化的文件]</td> 
   <td>选择要转换的文件格式 [!DNL Google Documents] 到。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL转换 [!DNL Google Spreadsheets] 要格式化的文件]</td> 
   <td>选择要转换的文件格式 [!DNL Google Spreadsheets] 到。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL转换 [!DNL Google Slides] 要格式化的文件]</td> 
   <td>选择要转换的文件格式 [!DNL Google Slides] 到。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL转换 [!DNL Google Drawings] 要格式化的文件]</td> 
   <td>选择要转换的文件格式 [!DNL Google Drawings] 到。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件ID]</td> 
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
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在连接 [!DNL Google Drive] 到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目标]</td> 
   <td> <p>选择要搜索的目标。</p> 
    <ul> 
     <li>[！UICONTROL我的驱动器]</li> 
     <li>[！UICONTROL与我共享]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL列出文件夹]</td> 
   <td>导航到要搜索文件或文件夹的文件夹。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Retrieve]</td> 
   <td> <p> 选择是要搜索文件、文件夹，还是同时搜索两者。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL搜索]</p> </td> 
   <td> <p>选择要执行的搜索类型。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL在文件/文件夹名称中搜索]</strong> </p> 
      <ul> 
       <li> <p><strong>[！UICONTROL查询]</strong> </p> <p>输入要搜索的文件名或完整文件名（包括后缀）的一部分。</p> </li> 
       <li> <p><strong>[！UICONTROL搜索选项]</strong> </p> <p>选择是要搜索确切的搜索词，还是要搜索包含该搜索词的名称。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL Fulltext]搜索</strong> </p> 
      <ul> 
       <li> <p><strong>[！UICONTROL查询]</strong> </p> <p>输入要在中搜索的任何搜索词 [!DNL Google Drive].</p> </li> 
      </ul> </li> 
     <li> <p><strong>输入自定义搜索查询</strong> </p> 
      <ul> 
       <li> <p><strong>[！UICONTROL查询]</strong> </p> <p>输入自定义搜索查询。 有关更多详细信息，请参阅本文的[！UICONTROL搜索文件]部分。</p> </li> 
       <li> <p><strong>将上面选择的文件夹添加到查询中</strong> </p> <p>搜索父项收藏集中的文件夹。 这会查找直接位于上面所选文件夹中的所有文件和文件夹。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL返回结果的最大数目]</td> 
   <td>设置文件或文件夹的最大数量 [!DNL Workfront Fusion] 将在一个执行周期内返回。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL即使模块未返回任何结果，仍继续执行路由]</td> 
   <td>启用此选项可确保模块未返回任何结果时不会停止该方案。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建文件夹]

在指定位置创建文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在连接 [!DNL Google Drive] 到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目标]</td> 
   <td> <p>选择要将文件上传到的目标。</p> 
    <ul> 
     <li>[！UICONTROL我的驱动器]</li> 
     <li>[！UICONTROL与我共享]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL新文件夹位置]</td> 
   <td>导航到要创建新文件夹的位置。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL新文件夹的名称]</td> 
   <td>输入正在创建的文件夹的名称。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL共享文件夹]</td> 
   <td>如果要与具有[！UICONTROL共享]链接的任何用户共享文件夹，请选择此选项。 否则，共享链接仅供所有者使用。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取共享链接]

在Google驱动器中检索文件的共享链接。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Drive] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">正在连接 [!DNL Google Drive] 到[！UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件ID]</td> 
   <td>映射要获取共享链接的文件的ID。</td> 
  </tr> 
 </tbody> 
</table>

## 故障排除

### 无法上传或更新文件

上传或更新文件失败时有几种情况：

* 上传的文件太大，超过了允许的最大文件大小限制 [!DNL Google Drive] 计划或您已超出 [!DNL Google Drive] 存储限制。 您可以升级存储计划，也可以从 [!DNL Google Drive] 服务。
* 要将文件上传到的所选文件夹不再存在。 场景将停止，然后需要再次选择目标文件夹。

## 搜索文件

在List files in a folder模块中，您可以使用自己的查询，该查询由以下部分组成：

* **[!UICONTROL 字段]**  — 所搜索文件的属性，例如，属性 `name` 文件中的。

* **[!UICONTROL 运算符]**  — 对数据执行以提供匹配的测试，例如， `contains`.

* **[!UICONTROL 值]**  — 测试的属性的内容，例如文件名 `My cool document`.

将子句与连接项组合 `and` 或 `or`，并使用否定查询 `not`.

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
   <td>布尔型 </td> 
   <td><code>=</code>， <code>!=</code></td> 
   <td> <p> 文件是否在垃圾桶中。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL starred]</code></td> 
   <td>布尔型 </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p>文件是否被启动。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL parents]</code></td> 
   <td>收藏集 </td> 
   <td><code>in </code> </td> 
   <td> <p>[！UICONTROL parents]集合是否包含指定的ID。</p> </td> 
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
   <td>布尔型 </td> 
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

请考虑以下有关这些字段中的运算符的信息：

* 此 `contains` 运算符仅执行前缀匹配 `title`.

  例如，标题“HelloWorld”与 `title contains 'Hello'` 但不适用于 `title contains 'World'`.

* 此 `contains` 运算符仅对的整个字符串令牌执行匹配 `fullText`.

  例如，如果文档的全文仅包含字符串“HelloWorld”，则查询为 `fullText contains 'HelloWorld'` 返回一个结果。 查询，例如 `fullText contains 'Hello'` 将不会在此场景中返回结果。

* 此 `contains` 如果运算符用双引号括起来，则它匹配一个准确的字母数字短语。

  例如，如果 `fullText` 文档的URL包含字符串“Hello there world”，然后是查询 `fullText contains '"Hello there"'` 返回一个结果，但查询 `fullText contains '"Hello world"'` 不会。

  此外，因为搜索是字母数字的，如果 `fullText` 文档的URL中包含字符串“Hello_world”，然后是查询 `fullText contains '"Hello world"'` 返回一个结果。

* 字段 `type` 日期之间不可比较，只能比较固定日期。

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
   <td> <p>用单引号括起来。 使用以下方式转义查询中的单引号 <code>\'</code>，例如，<code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>布尔型 </td> 
   <td> <p><code>true </code>或 <code>false</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>日期 </td> 
   <td> <p>RFC 3339格式，默认时区为UTC，例如， <code>2012-06-04T12:00:00-08:00</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 运算符

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>操作员 </th> 
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
   <td> <p> 字符串或布尔值的内容等于另一个字符串或布尔值。</p> </td> 
  </tr> 
  <tr> 
   <td><code>!=</code> </td> 
   <td> <p> 字符串或布尔值的内容不等于另一个字符串或布尔值。</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;</code> </td> 
   <td> <p> 日期早于另一个日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;=</code> </td> 
   <td> <p> 日期早于或等于另一个日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>></code> </td> 
   <td> <p> 日期晚于另一个日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>>=</code> </td> 
   <td> <p> 日期晚于或等于另一个日期。</p> </td> 
  </tr> 
  <tr> 
   <td><code>in </code> </td> 
   <td> <p>元素包含在收藏集中。</p> </td> 
  </tr> 
  <tr> 
   <td><code>and </code> </td> 
   <td> <p>返回匹配两个子句的文件。</p> </td> 
  </tr> 
  <tr> 
   <td><code>or </code> </td> 
   <td> <p>返回与任一子句匹配的文件。</p> </td> 
  </tr> 
  <tr> 
   <td><code>not </code> </td> 
   <td> <p>使搜索子句无效。</p> </td> 
  </tr> 
  <tr> 
   <td><code>has </code> </td> 
   <td> <p>收藏集包含与参数匹配的元素。</p> </td> 
  </tr> 
 </tbody> 
</table>

对于复合子句，可以使用括号将子句组合在一起。 例如：
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` 此搜索会返回其上次修改是在2012年6月4日之后且图像或视频MIME类型的所有文件。 因为 `and` 和 `or` 从左到右评估运算符，不使用圆括号，上述示例将仅返回在2012年6月4日之后修改的图像，但会返回所有视频，甚至是2012年6月4日之前的视频。

### 示例

此页面上的所有示例都显示了未编码的 `<q>q</q>` 参数，其中 `title = 'hello'` 编码为 `title+%3d+%27hello%27`. 客户端库会自动处理此编码。

* 搜索名为“hello”的文件
  <pre>title = 'hello'</pre>
* 使用文件夹特定的MIME类型搜索文件夹
  <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* 搜索不是文件夹的文件
  <pre>mimeType！= 'application/vnd.google-apps.folder'</pre>
* 搜索名称中包含单词“hello”和“goodbye”的文件
  <pre>标题包含'hello'，[！UICONTROL名称]包含'goodbye'</pre>
* 搜索名称中不包含单词“hello”的文件
  <pre>标题不包含'hello'</pre>
* 搜索内容中包含“hello”一词的文件
  <pre>全文包含'hello'</pre>
* 搜索内容中不包含单词“hello”的文件
  <pre>非fullText包含“hello”</pre>
* 搜索内容中包含精确短语“hello world”的文件
  <pre>全文包含“ hello world”“全文包含“ hello_world””</pre>
* 搜索其查询包含“\”字符（例如，“\authors”）的文件
  <pre>全文包含'\\authors'</pre>
* 搜索可由用户“test@example.org”写入的文件
  <pre>中的“test@example.org” [!DNL writers]</pre>
* 搜索ID `1234567` 在 `parents` 收藏集。 这会查找直接位于ID为 `1234567`.
  <pre>[！UICONTROL父级]中的'1234567'</pre>
* 搜索别名ID `appDataFolder` 在 `parents` 收藏集。 这会查找位于下的所有文件和文件夹 [应用程序数据文件夹](https://developers.google.com/drive/api/v2/appdata).
  <pre>父级中的“appDataFolder”</pre>
* 搜索可由用户“test@example.org”和“test2@example.org”写入的文件
  <pre>作家中的“test@example.org”，作家中的“test2@example.org”</pre>
* 搜索包含垃圾桶中“important”文本的文件
  <pre>fullText包含“important”，并且已置入垃圾桶= true</pre>
* 搜索在2012年6月4日后修改的文件
  <pre>修改日期&gt; '2012-06-04T12:00:00' //默认时区是UTC</pre><pre>修改日期&gt; '2012-06-04T12:00:00-08:00`</pre>
* 搜索与授权用户共享的文件，其名称中包含“hello”
  <pre>sharedWithMe和标题包含“hello”</pre>
* 使用搜索文件 [自定义文件属性](https://developers.google.com/drive/api/v2/properties) 已命名 `additionalID` 具有值 `8e8aceg2af2ge72e78`.
  <pre>属性具有{ key='additionalID'和value='8e8aceg2af2ge72e78'和visibility='PRIVATE' }</pre>

本指南的来源为 [[!DNL Google Drive] 文档](https://developers.google.com/drive/api/v2/search-shareddrives).
