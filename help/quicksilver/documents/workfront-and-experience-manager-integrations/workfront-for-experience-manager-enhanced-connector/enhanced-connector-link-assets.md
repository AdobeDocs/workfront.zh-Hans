---
title: 使用增强的连接器链接资产和文件夹
description: 您可以将资产或文件夹从Experience Manager Assets链接到支持文档的任何Workfront对象。
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# 使用增强的连接器链接资产和文件夹

您可以将资产或文件夹从Experience Manager Assets链接到支持文档的任何Workfront对象。 从Experience Manager Assets发送的资产不计入Workfront中的整个文档存储。 从Workfront上传并发送到Experience Manager Assets的文档确实会计入整体存储。

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
   <td> <p>查看文档的访问权限或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须

* 安装Workfront for Experience Manager增强连接器

## 从Experience Manager Assets链接资产

您可以将资产从Experience Manager Assets链接到Workfront。 关联资产后，您可以

* [为Experience Manager Assets校样链接的资产](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md)
* [上传文档的新版本](../../../documents/managing-documents/upload-new-document-version.md)

要将资产链接到Experience Manager Assets，请执行以下操作：

1. 转到 **文档** 中要添加文档的区域。
1. 单击 **新增**，然后选择管理员设置的Experience Manager Assets集成。

   >[!NOTE]
   >
   >可以为此集成选择任何名称，因此不能特别提及Experience Manager Assets。

1. 选择所需的资产。

   ![](assets/select-an-asset.png)

1. 单击 **链接**.

## 从Experience Manager Assets链接文件夹

查看文件夹内单个资产的权限取决于Experience Manager Assets权限。

要将文件夹链接到Experience Manager Assets，请执行以下操作：

1. 转到 **文档** 中要添加文档的区域。
1. 单击 **新增**，然后选择管理员设置的Experience Manager Assets集成。

   >[!NOTE]
   >
   >可以为此集成选择任何名称，因此不能特别提及Experience Manager Assets。

1. 选择所需的文件夹。

   ![](assets/select-a-folder.png)

1. 单击 **链接**.

## 从Experience Manager Assets链接新版本

您可以从Experience Manager Assets中提取新资产，并将其作为Workfront中的新版本添加到现有资产中。 如果文档已链接，并且在Experience Manager Assets中添加了新版本，则新版本会在Workfront中自动显示。

>[!TIP]
>
>如果您转到 **文档详细信息** > **版本**.

要从Experience Manager Assets链接新版本，请执行以下操作：

1. 转到 **文档** 中要添加文档的区域。
1. 选择要替换为新版本的资产。 无法在链接的文件夹中创建资产的新版本。
1. 单击 **新增**，然后选择管理员设置的Experience Manager Assets集成。

   >[!NOTE]
   >
   >可以为此集成选择任何名称，因此不能特别提及Experience Manager Assets。

1. 选择所需的资产。

   ![](assets/select-an-asset.png)

1. 单击 **链接**.
