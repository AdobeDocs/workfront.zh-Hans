---
product-area: documents
navigation-topic: add-documents-to-workfront
title: 将文档从您的文件系统添加到Adobe Workfront
description: 您可以在Adobe Workfront中将文档添加到多个区域中的项目、任务或问题。
author: Courtney, Alina
feature: Digital Content and Documents
exl-id: 0a5f82b2-f86e-4ffa-b3a6-18221dd0e158
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7fc5fe2f2692841a8663740441f70be0c82c4073
workflow-type: tm+mt
source-wordcount: '1317'
ht-degree: 2%

---

# 将文档从您的文件系统添加到Adobe Workfront

Adobe Workfront当前具有以下两种类型的文档存储：

* 旧版Workfront存储
* Adobe云存储

有关这些存储类型的更多信息，请参阅[Adobe云存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

>[!NOTE]
>
>有些客户同时具有这两种类型的文档存储，而有些客户只有Workfront或Adobe存储。

将文档添加到Workfront会因贵组织使用的文档区域版本而异。

* [在旧版文档区域添加来自文件系统的文档](#add-documents-from-your-file-system-in-the-legacy-documents-area)
* [在新的“文档”区域将文档添加到Workfront](#add-documents-to-workfront-in-the-new-documents-area)

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>使用旧版Workfront存储管理文档的任何Workfront软件包</p>
<p>用于使用Adobe云存储管理文档的任意工作流包</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 许可证</td> 
   <td> 
   <p>参与者或更高版本</p> 
   <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>旧版Workfront Storage：编辑对文档的访问权限</p> 
   <p>Adobe云存储：默认情况下会启用对文档的编辑访问权限，无法对其进行更改</p>
   </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在旧版文档区域添加来自文件系统的文档

如果您的组织使用的是旧版Workfront存储，则在访问Workfront中的文档时，您将看到旧版文档区域。

有关Workfront存储的更多信息，请参阅[Adobe云存储与旧版Workfront存储之间的区别](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)。

您可以在Workfront中将文档添加到以下区域：

* 主菜单中的文档区域
* Workfront对象（项目、任务、问题、模板、模板任务、项目组合、项目群）的“文档”区域
* Workfront展示板上的连接卡

您还可以上传文档的新版本，并将链接添加到来自第三方云供应商（如Google Drive、Dropbox和Microsoft OneDrive）的文档。

有关添加文档新版本的信息，请参阅[上载文档的新版本](../../documents/managing-documents/upload-new-document-version.md)。

有关添加来自第三方云供应商的文档的信息，请参阅[链接来自外部应用程序的文档](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

您可以上传到Workfront的文件类型和大小没有限制。 但是，为了成功，上传必须在5分钟内完成，并且您必须具有足够的可用存储空间。

如果需要有关将文档的新版本上载到Workfront的信息，请参阅[上载文档的新版本](../../documents/managing-documents/upload-new-document-version.md)。


### 在旧版文档区域将文档添加到Workfront

您可以从工作站上的文件系统向Workfront添加新文档。 您还可以链接来自第三方应用程序（如Google Drive和SharePoint）的文档。

>[!IMPORTANT]
>
>* 您一次最多可以上传150个文档。
>* 文件大小没有限制。
>* 文档下载限制为4GB。

要添加文档，请执行以下操作：

1. 转到要添加新文档的Workfront对象。
1. 单击&#x200B;**文档**&#x200B;选项卡，然后单击&#x200B;**添加新文档**&#x200B;下拉菜单。

   ![添加新文档](assets/add-new-doc.png)

1. 根据要添加的文档类型，执行以下任一操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">从工作站上的文件系统上传文档</td> 
      <td> 
       <ol> 
        <li value="1">从<strong>添加新</strong>下拉菜单中，选择<strong>文档。</strong></li> 
        <li value="2"> <p>浏览并选择要从工作站上的文件系统添加的文档。<br></p> <p>选择其他文件时，按住Shift键可选择多个文档。</p> </li> 
        <li value="3">单击<strong>打开</strong>。</li> 
       </ol> 
       <p><b>注意</b>：您还可以将文件直接从文件管理器拖放到文档列表中。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">从第三方应用程序（如Google Drive或SharePoint）上传文档</td> 
      <td> 
       <ol> 
        <li value="1"> <p>从<strong>添加新</strong>下拉菜单中，选择<strong>从&lt;name_of_third-party_application&gt;</strong>。</p> <p>例如，要从Google驱动器上传文档，请单击<strong>从Google驱动器</strong>。</p> </li> 
        <li value="2"> <p>按照提示在第三方应用程序中选择文档。<br></p> <p>有关链接文档的更多信息，请参阅<a href="../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md" class="MCXref xref">链接来自外部应用程序的文档</a>。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">从其他Workfront用户请求文档</td> 
      <td> 
       <ol> 
        <li value="1">从<strong>添加新</strong>下拉菜单中，选择<strong>请求文档</strong>。</li> 
        <li value="2">在<strong>您是从</strong>中请求文档的用户框中，键入您向其请求文档的用户名。</li> 
        <li value="3">在<strong>告知您请求的内容</strong>框中，键入文档的名称。</li> 
        <li value="4"> <p>单击<strong>发送请求</strong>。</p> <p>您的请求将显示在“文档”选项卡上。</p> <p>有关请求文档的更多信息，请参阅<a href="../../documents/adding-documents-to-workfront/request-a-document.md" class="MCXref xref">请求文档</a>。</p> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

   文档将添加到所选对象的“文档”部分。

## 在新的“文档”区域将文档添加到Workfront

您可以使用Adobe云存储模型将文档添加到对象。 有关Adobe云存储的更多信息，请参阅[Adobe云存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

新文档区域当前不支持的功能：

* 将文档上传到主菜单的文档区域
* 添加指向第三方云供应商（如Google Drive、Dropbox和Microsoft OneDrive）文档的链接。
* 请求文档
* 将链接复制到文件夹
* 签出文档
* 从剪贴板粘贴图像
* 添加智能文件夹

### 在新的“文档”区域将文档添加到Workfront

如果您的组织使用Adobe云存储，则在访问Workfront中的文档时，您将看到新的文档区域。 有关Adobe云存储的更多信息，请参阅[Adobe云存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

要添加文档，请执行以下操作：

1. 转到要添加新文档的Workfront对象。
1. 单击左侧面板中的&#x200B;**文档**&#x200B;部分。
1. 单击页面右侧的&#x200B;**新建**&#x200B;或将文件拖放到显示的拖放区域中。 您可以一次添加多个文档。

   ![添加新文档](assets/add-new-doc-new-doc.png)

如果需要有关将文档的新版本上载到Workfront的信息，请参阅[上载文档的新版本](../../documents/managing-documents/upload-new-document-version.md)。

系统会自动在“文档”部分中创建与上载文档的目标对象同名的文件夹，并将文档添加到该文件夹。

## Adobe云存储的文档安全

Workfront通过以下方式防止病毒和其他恶意内容通过文档进入站点：

**Workfront如何检测损坏的文件**

使用Adobe云存储模型会自动为对象启用文档扫描。

上传时，将扫描500 MB以下的所有文件。 不会扫描超过500 MB的文件。 如果Workfront检测到损坏的文档，则会自动将其删除。

**文件名限制**

由于此集成是使用Adobe云存储构建的，因此在管理项目和文档时，应注意一些强制性的结构和命名约定。

* 对象名称必须是唯一的，并且不能重复
* Adobe云存储要求层次结构树中具有相同父级的对等对象具有唯一名称
* 如果文档属于同一项目，则不能具有相同的名称
* 文档名称不能包含以下任何特殊字符： `\ / : * ? " | < >`
* 文档名称限制为最多255个字符

考虑到这些限制，Workfront会根据需要自动重命名对象或文档，以防止冲突。


## 旧版Workfront存储的文档安全

Workfront通过以下方式防止病毒和其他恶意内容通过文档进入站点：

**Workfront如何检测损坏的文件**

仅应请求为贵组织启用文档扫描。

如果启用了文档扫描，则在上传时扫描小于25 MB的文件。 不会扫描超过25 MB的文件。

如果Workfront检测到损坏的文档，则会显示一条消息，指示文件已损坏。 此外，当Workfront检测到潜在的恶意内容并计划删除文件时，您会收到电子邮件通知。

损坏的文件会在检测到后的24小时内删除，除非您手动删除它们。 如果删除损坏的文件，Workfront会将此操作作为更新进行跟踪。 如果您允许Workfront删除它，则不会记录任何更新。

**文件名限制**

上载到Workfront的文件不能包含文件名中的某些字符。 如果文件在文件名中包含以下任何字符，则在上载文件时，将从文件名中删除这些字符： `! # % * \ | ' " / ? < > { } [ ]`。
