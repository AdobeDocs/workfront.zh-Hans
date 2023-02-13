---
product-area: documents
navigation-topic: manage-documents
title: 管理文档版本
description: 您可以在Workfront中管理文档的多个版本。
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# 管理文档版本

您可以在Workfront中管理文档的多个版本。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看文档访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看对文档的访问</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

* 本文假定文档具有多个版本。

   如果您需要有关将文档的新版本上传到Workfront的信息，请参阅 [上传文档的新版本](../../documents/managing-documents/upload-new-document-version.md).

## 查看文档所有版本的列表

1. 在“摘要”中，滚动到视图 **所有版本** 中。 您可以在此处查看文档的所有版本。

## 查看和管理以前文档版本的详细信息

1. 在“文档详细信息”页面顶部附近，单击该名称旁边的下拉菜单，然后单击要查看和管理的版本的名称。

   ![](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   除了查看版本的详细信息之外，您还可以更改版本，如其名称、元数据和校对设置（如果是文档校样）。

## 下载单个文档版本

1. 在摘要中， **版本**，单击更多菜单 ![](assets/more-icon.png) 在版本的右侧，单击 **下载** 中。

   ![](assets/more-versions-350x143.png)

## 下载文档的所有版本

1. 单击 **文档详细信息**，然后选择 **所有版本** 中。

1. 单击 **全部下载** 列表顶部。

## 删除文档版本

如果您错误地上传文档的某个版本，或者不再需要某个版本，则可以删除该版本并维护原始文档。

>[!IMPORTANT]
>
>无法恢复单独删除的文档版本。

在考虑删除文档版本时，请牢记以下几点：

* 一次只能删除一个版本。 如果删除了某个版本，则此操作会显示在 **更新** 在文档中。
* 如果您在删除某个版本后上传了新版本，则新版本会收到下一个序列号。 例如，如果文档有3个版本，并且您删除了版本3，则下一个上传的文档将是版本4。
* 删除版本后，对版本进行的系统更新和评论会保留在Workfront中。

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

要删除文档版本，请执行以下操作：

1. 转到包含文档的项目、任务或问题，然后选择 **文档**.查找所需文档。
1. 在 **版本** ，单击版本，然后单击 **删除** 中。 的 **删除** 仅当至少有两个版本时，才会显示选项。

   如果文档已链接到外部源，则该链接将被删除，并且该文档将不再通过Workfront访问。

   ![](assets/more-versions-350x143.png)
