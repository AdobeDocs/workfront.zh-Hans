---
product-area: documents
navigation-topic: manage-documents
title: 管理文档版本
description: 您可以在Workfront中管理文档的多个版本。
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: a9dbfe21337be9cd9929f4e982e4979265ca14e1
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 0%

---

# 管理文档版本

<!-- Audited: 5/2025 -->

您可以在Workfront中管理文档的多个版本。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>新文档：参与者或更高版本<p>
   <p>或</p>
   <p>当前：请求或更高版本 </p>


</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看对文档的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看对文档的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

* 本文假定文档有多个版本。

  如果需要有关将文档的新版本上载到Workfront的信息，请参阅[上载文档的新版本](../../documents/managing-documents/upload-new-document-version.md)。

## 查看文档所有版本的列表

{{step1-to-documents}}

1. 在&#x200B;**文档**&#x200B;页面上，选择列表中的文档。

1. 在页面的右上角，单击&#x200B;**打开摘要**&#x200B;图标![打开摘要图标](assets/qs-summary-in-new-toolbar-small.png)。 **文档摘要**&#x200B;侧面板打开。

1. 向下滚动到&#x200B;**版本**&#x200B;部分以查看所有文档版本。

## 查看和管理以前文档版本的详细信息

{{step1-to-documents}}

1. 将鼠标悬停在文档上，然后单击&#x200B;**文档详细信息**。

1. 在&#x200B;**文档详细信息**&#x200B;页面顶部附近，单击该名称旁边的下拉菜单，然后单击要查看和管理的版本的名称。

   “文档详细信息”页面上的![版本下拉列表](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   除了查看版本详细信息外，您还可以对版本进行更改，例如其名称、元数据和验证设置（如果它是文档验证）。

## 下载单个文档版本

{{step1-to-documents}}

1. 在&#x200B;**文档**&#x200B;页面上，选择列表中的文档。

1. 在页面的右上角，单击&#x200B;**打开摘要**&#x200B;图标![打开摘要图标](assets/qs-summary-in-new-toolbar-small.png)。 **文档摘要**&#x200B;侧面板打开。

1. 在&#x200B;**版本**&#x200B;部分中，单击版本右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-icon.png)，然后在显示的下拉列表中单击&#x200B;**下载**。

   ![下载单个文档](assets/more-versions-350x143.png)

## 下载文档的所有版本

{{step1-to-documents}}

1. 在&#x200B;**文档**&#x200B;页面上，选择列表中的文档。

1. 在页面的右上角，单击&#x200B;**打开摘要**&#x200B;图标![打开摘要图标](assets/qs-summary-in-new-toolbar-small.png)。 **文档摘要**&#x200B;侧面板打开。

1. 向下滚动到&#x200B;**版本**&#x200B;部分，然后单击&#x200B;**全部下载**。

## 删除文档版本

如果错误地上载了文档的某个版本，或者不再需要某个版本，则可以删除该版本并维护原始文档。

>[!IMPORTANT]
>
>您无法恢复单独删除的文档版本。

当您考虑删除文档版本时，请牢记以下几点：

* 一次只能删除一个版本。 如果删除了某个版本，则此操作会显示在文档的“更新”部分中。
* 如果在删除版本后上载新版本，则新版本将接收下一个序列号。 例如，如果文档有3个版本，而您删除了版本3，则上传的下一个文档将是版本4。
* 删除版本后，对版本所做的系统更新和注释会保留在Workfront中。

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

要删除文档版本，请执行以下操作：

{{step1-to-documents}}

1. 在&#x200B;**文档**&#x200B;页面上，从列表中选择文档。

1. 在页面的右上角，单击&#x200B;**打开摘要**&#x200B;图标![打开摘要图标](assets/qs-summary-in-new-toolbar-small.png)。 **文档摘要**&#x200B;侧面板打开。

1. 向下滚动到&#x200B;**版本**&#x200B;部分以查看所有文档版本。
1. 在&#x200B;**版本**&#x200B;部分中，单击版本右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-icon.png)，然后在显示的下拉列表中单击&#x200B;**删除**。

   >[!NOTE]
   >
   >* **删除**&#x200B;选项仅在至少有2个版本时才可见。
   >* 如果文档链接到外部源，则该链接会被删除，并且无法再通过Workfront访问文档。

   ![删除文档版本](assets/more-versions-350x143.png)
