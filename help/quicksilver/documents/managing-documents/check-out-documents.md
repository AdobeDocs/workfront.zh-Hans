---
product-area: documents
navigation-topic: manage-documents
title: 签出文档
description: 您可以签出文档以防止其他用户删除它或上载它的新版本。 一次只能有一个用户签出文档。 您可以签出上传到Adobe Workfront的任何文档以及链接到第三方文档提供商(Box、Dropbox、Google Drive、Webdam、Workfront DAM、SharePoint或任何其他自定义提供商)的文档。
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: 85a2f154b3b561cdf53c68d50e66b8945f9f9823
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 0%

---

# 签出文档

您可以签出文档以防止其他用户删除它或上载它的新版本。 一次只能有一个用户签出文档。 您可以签出上传到Adobe Workfront的任何文档以及链接到第三方文档提供商(Box、Dropbox、Google Drive、Webdam、Workfront DAM、SharePoint或任何其他自定义提供商)的文档。 

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>审核或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对文档的访问</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

+++

## 允许对已签出文档执行的操作

对文档具有管理访问权限的用户可以执行以下操作：

* 编辑文档（文档名称、描述、自定义数据）
* 移动文档
* 共享文档
* 预览文档
* 下载文档

  >[!TIP]
  >
  > 虽然当文档被其他用户检出时，用户可以下载文档，但我们建议用户等到文档重新检入后再下载。 当文档被检出时，它通常表示文档上的工作仍在进行中。 等到文档签回下载时，可以确保用户拥有最新版本。

* 批准文档或对文档应用批准。
* 在校对查看器中查看文档

  有关校对的详细信息，请参阅[校对](../../review-and-approve-work/proofing/proofing.md)

## 签出文档

如果您对文档具有管理权限，则可以将其检出以禁止对文档执行某些操作。 

1. 转到存储文档的区域，然后选择文档。 

   有关添加文档的信息，请参阅[将文档从您的文件系统添加到Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)。

1. 单击&#x200B;**签出**&#x200B;图标![签出图标](assets/check-out-25x23.png)。

1. 文档名称的右侧将显示一个锁定图标![锁定图标](assets/lock-icon-locked-qs.png)。 注销Workfront后，文档将保持签出状态。
1. 只有签出文档的用户或Workfront管理员才能签入文档。

## 管理已签出的文档

有关已签出文档，请考虑以下事项：

* 在删除存储已检出文档的对象之前，必须先将该文档检回。 
* 如果Workfront管理员删除了一个签出其非所有文档的用户，则Workfront会自动签入该文档。
* 如果Workfront管理员删除签出其拥有的文档的用户，并且该文档被上传到对象上，则该文档保持签出状态。 只有Workfront管理员才能将其签回。
* 如果Workfront管理员删除了签出其拥有的文档的用户，并且文档仅在“文档”区域（而不是对象上）上传，则该文档将随该用户一起删除。

  有关删除用户的信息，请参阅[删除用户](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md)。

* 如果Workfront管理员停用用户，则他们已签出的任何文档都会保持签出状态。 只有Workfront管理员才能重新签入这些帐户。 

## 检入文档

您必须重新签入文档，然后才能上传新版本或删除该版本。 

要检入文档：

1. 转到存储文档的区域，然后选择文档。 

   文档名称的右侧将显示一个锁定图标![锁定图标](assets/lock-icon-locked-qs.png)。

1. 单击&#x200B;**签入**&#x200B;图标![签入图标](assets/check-in-25x22.png)。
