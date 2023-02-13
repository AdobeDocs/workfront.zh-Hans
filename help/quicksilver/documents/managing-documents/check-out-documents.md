---
product-area: documents
navigation-topic: manage-documents
title: 签出文档
description: 您可以签出文档，以阻止其他用户删除文档或上传新版本的文档。 一次只能有一个用户签出文档。 您可以签出上传到Adobe Workfront的任何文档以及链接到第三方文档提供程序的文档(Box、Dropbox、Google Drive、Webdam、Workfront DAM、SharePoint或任何其他自定义提供程序)。
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 签出文档

您可以签出文档，以阻止其他用户删除文档或上传新版本的文档。 一次只能有一个用户签出文档。 您可以签出上传到Adobe Workfront的任何文档以及链接到第三方文档提供程序的文档(Box、Dropbox、Google Drive、Webdam、Workfront DAM、SharePoint或任何其他自定义提供程序)。 

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对文档的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 签出文档时允许的操作

对文档具有管理访问权限的用户可以执行以下操作：

* 编辑文档（文档名称、说明、自定义数据）
* 移动文档
* 共享文档
* 预览文档
* 下载文档

   >[!TIP]
   >
   > 虽然用户在文档被其他用户签出时可以下载该文档，但我们建议用户在下载该文档之前先等待文档被签回。 当文档被检出时，它通常表示仍在对文档完成工作。 等待文档签回以下载，可确保用户具有最新版本。

* 批准文档或对文档应用批准。
* 在校对查看器中查看文档

   有关校对的更多信息，请参阅 [校对](../../review-and-approve-work/proofing/proofing.md)

## 签出文档

如果您对文档具有管理权限，则可以将其签出以禁止对文档执行某些操作。 

1. 转到文档的存储区域，然后选择该文档。 

   有关添加文档的信息，请参阅 [从文件系统将文档添加到Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

1. 单击 **结帐** 图标 ![](assets/check-out-25x23.png).

1. 锁图标 ![](assets/lock-icon-locked-qs.png) 显示在文档名称的右侧。 从Workfront注销后，文档将保持签出状态。
1. 只有签出文档的用户或Workfront管理员才能签入文档。

## 管理签出文档

请考虑以下有关已签出文档的事项：

* 在可以删除存储已签出文档的对象之前，必须先将文档签回。 
* 如果Workfront管理员删除了某个用户签出了他们不拥有的文档，则Workfront会自动签入该文档。
* 如果Workfront管理员删除了其拥有的文档的用户，并且该文档已上传到对象上，则该文档将保持签出状态。 只有Workfront管理员才能将其签回。
* 如果Workfront管理员删除了某个用户签出了他们拥有的文档，并且该文档仅在“文档”区域（而不是对象上）上传，则该文档将随用户一起删除。

   有关删除用户的信息，请参阅 [删除用户](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* 如果Workfront管理员停用用户，则他们签出的任何文档都将保持签出状态。 只有Workfront管理员才能重新签入。 

## 在

必须先将文档签回，然后才能上载新版本或删除它。 

要签入文档，请执行以下操作：

1. 转到文档的存储区域并选择文档。 

   锁图标 ![](assets/lock-icon-locked-qs.png) 显示在文档名称的右侧。

1. 单击 **签入** 图标 ![](assets/check-in-25x22.png).
