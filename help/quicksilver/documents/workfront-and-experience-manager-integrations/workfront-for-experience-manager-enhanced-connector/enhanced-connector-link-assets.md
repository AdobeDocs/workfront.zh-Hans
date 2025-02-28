---
title: 使用增强型连接器链接资源和文件夹
description: 您可以从Experience Manager Assets将资源或文件夹链接到任何支持文档的Workfront对象。
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: 85a2f154b3b561cdf53c68d50e66b8945f9f9823
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 1%

---


# 使用增强型连接器链接资源和文件夹

您可以从Experience Manager Assets将资源或文件夹链接到任何支持文档的Workfront对象。 从Experience Manager Assets发送的Assets不计入Workfront中的整体文档存储。 从Workfront上传并发送到Experience Manager Assets的文档确实会计入总体存储中。


>[!NOTE]
>
>在Workfront中无法预览通过增强型连接器链接的Excel文件。 您必须下载文件才能访问它。

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
   <td> <p>当前：请求或更高版本</p> 
   或
   <p>新文档：参与者或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看文档访问权限或更高版本</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。
+++

## 先决条件

在开始之前，您必须

* 安装Workfront for Experience Manager增强型连接器

## 从Experience Manager Assets链接资源

您可以将资源从Experience Manager Assets链接到Workfront。 链接资产后，您可以

* [校对Experience Manager Assets的链接资源](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md)
* [上载文档的新版本](../../../documents/managing-documents/upload-new-document-version.md)

要将资源链接到Experience Manager Assets，请执行以下操作：

1. 转到Workfront中要添加文档的&#x200B;**文档**&#x200B;区域。
1. 单击&#x200B;**新增**，然后选择管理员设置的Experience Manager Assets集成。

   >[!NOTE]
   >
   >可以为此集成选择任何名称，因此它可能没有特别提及Experience Manager Assets。

1. 选择所需的资源。

   ![选择资源](assets/select-an-asset.png)

1. 单击&#x200B;**链接**。

## 从Experience Manager Assets链接文件夹

查看文件夹中各个资产的权限取决于Experience Manager Assets权限。

要将文件夹链接到Experience Manager Assets，请执行以下操作：

1. 转到Workfront中要添加文档的&#x200B;**文档**&#x200B;区域。
1. 单击&#x200B;**新增**，然后选择管理员设置的Experience Manager Assets集成。

   >[!NOTE]
   >
   >可以为此集成选择任何名称，因此它可能没有特别提及Experience Manager Assets。

1. 选择所需的文件夹。

   ![选择文件夹](assets/select-a-folder.png)

1. 单击&#x200B;**链接**。

## 从Experience Manager Assets链接新版本

您可以从Experience Manager Assets中提取新资源，并将其作为Workfront中的新版本添加到现有资源。 如果文档已链接，并且在Experience Manager Assets中添加了新版本，则新版本会自动显示在Workfront中。

>[!TIP]
>
>如果您转到&#x200B;**文档详细信息** > **版本**，则可以查看资产的所有版本。

要链接来自Experience Manager Assets的新版本，请执行以下操作：

1. 转到Workfront中要添加文档的&#x200B;**文档**&#x200B;区域。
1. 选择要替换为新版本的资产。 您无法在链接的文件夹中创建资产的新版本。
1. 单击&#x200B;**新增**，然后选择管理员设置的Experience Manager Assets集成。

   >[!NOTE]
   >
   >可以为此集成选择任何名称，因此它可能没有特别提及Experience Manager Assets。

1. 选择所需的资源。

   ![选择资源](assets/select-an-asset.png)

1. 单击&#x200B;**链接**。
