---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: 使用增强的连接器发送文档
description: 您可以将文档从Workfront发送到Experience Manager Assets。 从Workfront上传并发送到Experience Manager Assets的文档仍会计入整个文档存储中。 从Experience Manager Assets链接的资产不计入整体存储。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 1%

---

# 使用增强的连接器发送文档

您可以将文档从Workfront发送到Experience Manager Assets。 从Workfront上传并发送到Experience Manager Assets的文档仍会计入整个文档存储中。 从Experience Manager Assets链接的资产不计入整体存储。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看对文档的访问权限或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须

* 安装Workfront for Experience Manager增强连接器。

## 将文档发送到Experience Manager Assets

当用户将文档从Workfront发送到Experience Manager Assets时，映射的元数据会随文档进行传输。 如果已配置，则每次进行更改时，元数据都会连续同步。

要发送文档，请执行以下操作：

1. 转到 **文档** ，然后选择要发送的文档。
1. 单击 **发送到**，然后选择管理员设置的Experience Manager Assets集成。

   >[!NOTE]
   >
   >可以为此集成选择任何名称，因此不能特别提及Experience Manager Assets。

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 选择资产的去向，然后单击 **选择文件夹**.
1. 找到所需目标后，单击 **保存**.

## 将新版本发送到Experience Manager Assets

您可以向之前上传到Workfront的文档添加新版本。 有关更多信息，请参阅 [上传文档的新版本](../../../documents/managing-documents/upload-new-document-version.md). 上传最新版本后，您可以将其发送到Experience Manager Assets。 如果Workfront中的映射字段发生更改，则新版本会在发送时更新Experience Manager Assets中的元数据。

要发送最新版本，请执行以下操作：

1. 转到 **文档** ，并找到文档。
1. 单击 **发送到**，然后选择管理员设置的Experience Manager Assets集成。

   >[!NOTE]
   >
   >可以为此集成选择任何名称，因此不能特别提及Experience Manager Assets。

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 单击&#x200B;**保存**。新版本保存在与先前版本相同的位置。
