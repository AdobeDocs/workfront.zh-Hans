---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Dropbox模块
description: 在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用Dropbox的工作流，并将其连接到多个第三方应用程序和服务。这样，您就可以自动执行Dropbox中的各种活动，如监视、搜索、检索、列出、创建和编辑文件和文件夹。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: a35631d7-40ac-4e7f-9a37-ad3879c0b6a2
source-git-commit: 86be8b6e1c21f3fd5f5b66afa3bf930d6bafbd63
workflow-type: tm+mt
source-wordcount: '3208'
ht-degree: 0%

---

# [!DNL Dropbox] 模块

在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用 [!UICONTROL Dropbox] 或 [!DNL Dropbox Business]，并将其连接到多个第三方应用程序和服务。这使您能够自动执行各种活动，例如监控、搜索、检索、列出、创建和编辑您的中的文件和文件夹 [!UICONTROL Dropbox].

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
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关的信息 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

* 使用 [!DNL Dropbox] 模块，您必须拥有 [!DNL Dropbox] 帐户。

>[!IMPORTANT]
>
>Dropbox必须批准用户数超过50的应用程序。
>
>有关更多信息，请在Dropbox开发人员指南中搜索“生产批准”。


## 创建与的连接 [!DNL Dropbox]

要为创建连接，请执行以下操作 [!DNL Dropbox] 模块：

1. 单击 **[!UICONTROL 添加]** ，位于“Connection（连接）”框旁。

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
          <p>输入此连接的名称。</p>
        </td>
        <tr>
        <td role="rowheader">[！UICONTROL环境]</td>
        <td>选择此连接是用于生产环境还是非生产环境。</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL类型]</td>
        <td>选择您是要连接到服务帐户还是个人帐户。</td>
        </tr>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL客户端ID]</td>
        <td>输入您的[！UICONTROLDropbox] [！UICONTROL客户端ID]。 </tr>
        <tr>
        <td role="rowheader">[！UICONTROL客户端密钥]</td>
        <td>输入您的 [!DNL Dropbox] [！UICONTROL客户端密钥]。 </td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL帐户类型]</td>
        <td>选择您是要连接到个人Dropbox帐户还是企业(Dropbox企业)帐户。</td>
        </tr>
      </tbody>
    </table>

1. 单击 **[!UICONTROL 继续]** 以保存连接并返回到模块。## [!DNL Dropbox] 模块及其字段

## [!DNL Dropbox] 模块及其字段

配置时 [!DNL Dropbox] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Dropbox] 字段可能会显示，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器模块](#trigger-modules)
* [获取模块 [!DNL Dropbox] 文件和文件夹](#modules-for-getting-dropbox-files-and-folders)
* [用于创建和编辑的模块 [!DNL Dropbox] 文件和文件夹](#modules-for-creating-and-editing-dropbox-files-and-folders)
* [其他模块](#other-modules)

### 触发器模块

#### [!UICONTROL 监视文件]

修改指定文件夹中的文件时，此触发器类型模块会返回文件详细信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关连接 [!DNL Dropbox] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-dropbox" class="MCXref xref">创建与的连接 [!DNL Dropbox]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择要监视更改的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Watch also subfolders]</td> 
   <td> <p> 启用此选项还可以监视所选文件夹中用于修改文件的子文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制] </td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 获取模块 [!DNL Dropbox] 文件和文件夹

* [[!UICONTROL 搜索文件/文件夹]](#search-filesfolders)
* [[!UICONTROL 下载文件]](#download-a-file)
* [[!UICONTROL 获取文件夹元数据]](#get-a-folder-metadata)
* [[!UICONTROL 列出文件夹中的所有文件/子文件夹]](#list-all-filessubfolders-in-a-folder)
* [[!UICONTROL 列出文件修订]](#list-file-revisions)

#### [!UICONTROL 搜索文件/文件夹]

此搜索模块查找对象中的记录 [!DNL Dropbox] 匹配您指定的搜索查询的规则。

您可以在场景的后续模块中映射此信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关连接 [!DNL Dropbox] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-dropbox" class="MCXref xref">创建与的连接 [!DNL Dropbox]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜索] </td> 
   <td> <p>输入搜索词。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择要搜索的文件夹。 此模块搜索整个 [!DNL Dropbox] 如果不选择文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>文件状态</td> 
   <td> <p> 选择文件状态，将搜索限制为选定的文件状态。</p> </td> 
  </tr> 
  <tr> 
   <td>文件类别</td> 
   <td> <p> 选择文件类别，将搜索限制在选定的类别内。</p> </td> 
  </tr> 
  <tr> 
   <td>文件扩展名</td> 
   <td> <p> 选择要搜索的文件扩展名。</p> </td> 
  </tr> 
  <tr> 
   <td>限制 </td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下载文件]

此操作模块从文件夹下载文件。

指定文件及其位置。

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
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关连接 [!DNL Dropbox] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-dropbox" class="MCXref xref">创建与的连接 [!DNL Dropbox]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>选择文件的方法</td> 
   <td> <p> 选择是要映射文件路径还是手动选择文件。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文件路径/文件</p> </td> 
   <td> <p style="font-weight: bold;">文件路径</p> <p>输入或映射目标路径到文件。</p> <p style="font-weight: bold;">文件</p> <p>从菜单中选择文件。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件夹元数据]

此操作模块可检索共享文件夹的详细信息。

指定文件夹的ID。

该模块会返回文件夹ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关连接 [!DNL Dropbox] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-dropbox" class="MCXref xref">创建与的连接 [!DNL Dropbox]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>共享文件夹ID</td> 
   <td> <p> 输入或映射要检索其详细信息的文件夹的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出文件夹中的所有文件/子文件夹]

此操作模块列出特定文件夹中的文件或文件夹。

指定文件夹的ID。

该模块返回文件或文件夹的ID以及任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关连接 [!DNL Dropbox] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-dropbox" class="MCXref xref">创建与的连接 [!DNL Dropbox]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>列表 </td> 
   <td> <p>选择是要检索文件或文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>仅显示可下载的文件</td> 
   <td> <p> 启用此选项可仅返回可下载的文件。 某些类型的文件(如Google文档)不可下载。</p> </td> 
  </tr> 
  <tr> 
   <td>文件夹 </td> 
   <td> <p>输入或映射要从中检索文件或文件夹的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>限制 </td> 
   <td> <p>输入或映射每个方案执行周期中您希望模块列出的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出文件修订]

此操作模块可检索特定文件的所有文件修订版本（版本历史记录）。\
指定文件的ID。

该模块会返回与记录关联的任何标准字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关连接 [!DNL Dropbox] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-dropbox" class="MCXref xref">创建与的连接 [!DNL Dropbox]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>选择文件的方法</td> 
   <td> <p> 选择是要映射文件路径还是手动选择文件。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文件路径/文件</p> </td> 
   <td> <p style="font-weight: bold;">文件路径</p> <p>输入或映射目标路径到文件。</p> <p style="font-weight: bold;">文件</p> <p>从菜单中选择文件。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>限制</p> </td> 
   <td> <p>输入或映射每个方案执行周期中您希望模块列出的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 用于创建和编辑的模块 [!DNL Dropbox] 文件和文件夹

* [[!UICONTROL 上传] 文件](#upload-a-file)
* [[!UICONTROL 创建文件夹]](#create-a-folder)
* [[!UICONTROL 创建/覆盖文本文件]](#createoverwrite-a-text-file)
* [[!UICONTROL 创建/更新共享链接]](#createupdate-a-share-link)
* [[!UICONTROL 恢复文件]](#restore-a-file)
* [[!UICONTROL 移动文件/文件夹]](#move-a-filefolder)
* [[!UICONTROL 重命名文件/文件夹]](#rename-a-filefolder)
* [[!UICONTROL 删除文件/文件夹]](#delete-a-filefolder)

#### [!UICONTROL 上传文件]

此操作模块将文件上传到文件夹。

您可以指定信息，例如文件的位置、要上传的文件以及文件的可选新名称。

模块会返回文件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关连接 [!DNL Dropbox] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-dropbox" class="MCXref xref">创建与的连接 [!DNL Dropbox]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹]</td> 
   <td> <p> 选择您的文件夹 [!DNL Dropbox] 文件要上传到的位置。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL源文件]</p> </td> 
   <td> <p>输入或映射要添加到的文件 [!DNL Dropbox] 以上选择的文件夹。</p> <p style="font-weight: bold;">[！UICONTROL文件名]</p> <p>输入或映射文件名，包括文件扩展名。</p> <p style="font-weight: bold;">[！UICONTROL文件数据]</p> <p>输入或映射文件数据(来自前一模块，如[！UICONTROL Google Drive] &gt;[！UICONTROL Get a File])。</p> <p>注意：上传文件的最大大小为150 MB。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL覆盖现有文件]</td> 
   <td> <p> 启用此选项可使用新文件替换现有文件。 如果将此选项保留为禁用，则将重命名上传的文件。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建文件夹]

此操作模块将创建新文件夹。

指定文件夹的路径和名称。

该模块会返回文件夹ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关连接 [!DNL Dropbox] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-dropbox" class="MCXref xref">创建与的连接 [!DNL Dropbox]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹名称] </td> 
   <td> <p>输入新文件夹的名称。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL文件夹]</p> </td> 
   <td> <p>输入或映射要创建新文件夹的路径。</p> <p>注意：   <p>如果您使用 [!DNL Dropbox Business] 帐户（包含团队空格），您必须删除斜杠 <code>/</code>，或者不要单击 <strong>[！UICONTROL单击此处]选择文件夹</strong> 以在根目录中创建团队文件夹。</p> <p>如果未删除斜杠，则出现错误 <code>[409] path/malformed_path/..</code> 会返回。</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自动重命名]</td> 
   <td> <p> 启用此选项可重命名新文件夹（如果目标位置中已存在同名文件夹）。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建/覆盖文本文件]

此操作模块创建DOC文件或覆盖现有文件的内容。

指定源文件和文件夹。

该模块会返回文件夹ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关连接 [!DNL Dropbox] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-dropbox" class="MCXref xref">创建与的连接 [!DNL Dropbox]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL选择至]</td> 
   <td> <p> 选择是要创建或覆盖DOC文件。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择要创建文件的目标位置。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL源文件]</p> </td> 
   <td> <p>输入或映射要添加到的文件 [!DNL Dropbox] 文件夹。</p> <p style="font-weight: bold;">文件名</p> <p>输入新DOC文件的文件名（不带扩展名）。</p> <p style="font-weight: bold;">文件内容</p> <p>输入DOC文件的文本内容。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建/更新共享链接]

此操作模块创建指向文件的公共链接。

指定文件以及有关链接的信息。

模块会返回链接的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关连接 [!DNL Dropbox] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-dropbox" class="MCXref xref">创建与的连接 [!DNL Dropbox]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL选择文件的方法]</td> 
   <td> <p> 选择是要映射还是输入文件路径，或者手动选择文件。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL文件路径/文件]</p> </td> 
   <td> <p style="font-weight: bold;">[！UICONTROL文件路径]</p> <p>输入或映射目标路径到文件。</p> <p style="font-weight: bold;">[！UICONTROL文件]</p> <p>从菜单中选择文件。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL请求的可见性]</p> </td> 
   <td> <p>选择链接是公共链接、团队链接还是密码受限链接。</p> <p>注意： [！UICONTROL仅团队]和[！UICONTROL通过密码访问]选项仅适用于具有以下权限的用户： [!DNL Dropbox Pro] 或更高版本。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL链接的到期日期]</td> 
   <td> <p> 输入链接到期且无法再访问的日期和时间。 如果此字段留空，链接将不会过期。 有关支持的日期和时间格式的列表，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">键入强制 [!DNL Adobe Workfront Fusion]</a>.</p> <p>注意： [！UICONTROL Team only]和[！UICONTROL Access with password]选项仅适用于具有[！UICONTROL Pro]或更高版本的Dropbox。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Link的访问级别]</p> </td> 
   <td> <p>设置链接收件人的权限。</p> <p><strong>[！UICONTROL查看器]</strong> 使用该链接的用户可以查看和评论内容。</p> <p><strong>[！UICONTROL编辑器]</strong> 使用该链接的用户可以编辑、查看和评论内容。</p> <p><strong>[！UICONTROL Max]</strong> 使用该链接的用户将获得您可以设置该链接的最大访问级别。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 恢复文件]

此操作模块恢复文件的先前版本。

指定所需的文件和修订版本号。

模块会返回版本ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关连接 [!DNL Dropbox] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-dropbox" class="MCXref xref">创建与的连接 [!DNL Dropbox]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL选择文件的方法]</td> 
   <td> <p> 选择是要映射还是输入文件路径，或者手动选择文件。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL文件路径] / [！UICONTROL文件]</p> </td> 
   <td> <p><strong>[！UICONTROL文件路径]</strong> </p> <p>输入或映射目标路径到文件。</p> <p><strong>[！UICONTROL文件]</strong> </p> <p>从菜单中选择文件。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL修订版]</p> </td> 
   <td> <p>输入或映射要恢复的修订版本的修订号。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移动文件/文件夹]

此操作模块会将文件或文件夹移动到其他位置。

您可以指定文件或文件夹，以及移动它的方法和位置。

该模块会返回文件或文件夹的ID以及任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关连接 [!DNL Dropbox] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-dropbox" class="MCXref xref">创建与的连接 [!DNL Dropbox]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL选择文件的方法] </td> 
   <td> <p>选择是要映射还是输入文件路径，或者手动选择文件。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL文件/文件夹路径] / [！UICONTROL文件/文件夹]</p> </td> 
   <td> <p style="font-weight: bold;">[！UICONTROL文件/文件夹路径]</p> <p>输入目标路径或将目标路径映射到文件或文件夹。</p> <p style="font-weight: bold;">[！UICONTROL文件/文件夹]</p> <p>从菜单中选择文件或文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL到文件夹]</p> </td> 
   <td> <p>输入或映射文件或文件夹的目标位置。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL新名称]</p> </td> 
   <td> <p>在新位置输入文件或文件夹的新名称。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL自动重命名]</p> </td> 
   <td> <p>启用此选项以确保如果存在同名的文件或文件夹，模块会重命名新的文件或文件夹，方法是在文件或文件夹名称后添加([！UICONTROL NUMBER])。 否则，将覆盖目标位置中的文件或文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL允许所有权转让]</p> </td> 
   <td> <p>启用此选项可允许所有者移动，即使这会导致所移动内容的所有权转移。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 重命名文件/文件夹]

此操作模块将重命名文件或文件夹。

指定文件或文件夹以及新名称。

该模块会返回文件或文件夹的ID以及任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关连接 [!DNL Dropbox] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-dropbox" class="MCXref xref">创建与的连接 [!DNL Dropbox]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>选择文件的方法</td> 
   <td> <p> 选择是要映射还是输入文件路径，或者手动选择文件。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文件/文件夹路径/文件/文件夹</p> </td> 
   <td> <p style="font-weight: bold;">文件/文件夹路径</p> <p>输入目标路径或将目标路径映射到文件或文件夹。</p> <p style="font-weight: bold;">文件/文件夹</p> <p>从菜单中选择文件或文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>重命名 </td> 
   <td> <p>输入文件的[！UICONTROL目标名称]，包括文件扩展名。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除文件/文件夹]

此操作模块删除文件或文件夹。

指定文件或文件夹。

该模块返回记录ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关连接 [!DNL Dropbox] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-dropbox" class="MCXref xref">创建与的连接 [!DNL Dropbox]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL选择文件的方法]</td> 
   <td> <p> 选择是要映射还是输入文件路径，或者手动选择文件。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL文件路径] / [！UICONTROL文件]</p> </td> 
   <td> <p style="font-weight: bold;">[！UICONTROL文件路径]</p> <p>输入或映射目标路径到文件。</p> <p style="font-weight: bold;">[！UICONTROL文件]</p> <p>从菜单中选择文件。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他模块

#### [!UICONTROL 进行API调用]

通过此操作模块，您可以对 [!DNL Dropbox] API。 这样，您就可以创建另一个无法实现的数据流自动化 [!DNL Dropbox] 模块。

配置此模块时，会显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关连接 [!DNL Dropbox] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="#create-a-connection-to-dropbox" class="MCXref xref">创建与的连接 [!DNL Dropbox]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>输入相对路径输入相对路径 <code>https://api.dropboxapi.com</code>. 例如， <code>/2/files/list_folder</code></p> <p>注：有关可用端点的列表，请参阅 <a href="https://www.dropbox.com/developers/documentation/http/documentation">DropboxAPI v2文档</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL方法]</p> </td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Headers] </td> 
   <td> <p>输入所需的请求标头。 [!DNL Workfront Fusion] 自动添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL查询字符串]</td> 
   <td> <p> 输入请求查询字符串。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Body] </td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：   <p>使用条件语句(例如 <code>if</code> 在JSON中，将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**示例：** 以下API调用返回来自的前10个文件 [!DNL /Text files] 中的文件夹 [!DNL Dropbox] 帐户：
>
>URL： `/2/files/list_folder`
>
>正文：
> 
>`{`
>
>`"path": "/Text files",`
>
>`"limit": 10,`
>
>`"recursive": false,`
>
>`"include_deleted": false`
>
>`}`
>
>搜索匹配项可在模块的“输出”中找到，位于 [!UICONTROL 捆绑] > [!UICONTROL 正文] >条目。
>
>在我们的示例中，返回了10张票证：

## 常见问题

* [无法上传或更新文件](#unable-to-upload-or-update-a-file)
* [无法呈现通过共享链接引用的图像](#image-referenced-via-a-shared-link-does-not-render)

### 无法上传或更新文件

上传或更新文件失败时，可能会出现以下几种情况：

* 上传的文件太大，超过了允许的最大文件大小。 [!DNL Dropbox] 计划，或者你用了 [!DNL Dropbox] 帐户的存储配额。 您必须从 [!DNL Dropbox] 帐户或升级计划。
* 先前选择的文件夹（文件将上载到该文件夹）不再存在。 场景将停止，您必须再次选择目标文件夹。

### 无法呈现通过共享链接引用的图像

返回的URL [!UICONTROL Dropbox] >[!UICONTROL 创建共享链接] 不会直接链接到图像，而是链接到 [!DNL Dropbox] 页面。 要强制下载图像，请替换尾随的 `?dl=0` 替换为 `?dl=1`. 要强制呈现图像(例如，在Web浏览器或Facebook Messenger中)，请在 `&raw=1` 到URL。

如果您需要获取您网站或其他网站的图像的直接或原始链接 [!DNL Workfront Fusion] 模块时，必须按以下方式修改初始共享URL：

原始URL：

`https://www.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png?dl=0`

1. 替换 `www` 替换为 `dl`.
1. 移除 `?dl=0`.

最终URL：

`https://dl.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png`

要自动修改URL，您可以使用 `replace()` 函数两次：

* 将www替换为dl

  ![](assets/www-to-dl-350x32.png)

* 要删除？dl=0

  ![](assets/remove-dl0-350x33.png)

要一次性完成此操作，请组合以下函数：

![](assets/replace-both-350x47.png)

您也可以复制该模板并将其粘贴到字段中。 替换 `1.url` 包含URL。

```
{{replace(replace(1.url; "?dl=0"; ""); "www"; "dl")}}
```
