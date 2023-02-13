---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 从Experience Manager Assets或Assets Essentials链接资产和文件夹
description: 您可以将资产或文件夹从Experience Manager Assets或Assets Essentials链接到任何支持文档的Adobe Workfront对象。 从Assets Essentials发送的资产不计入Workfront中的整个文档存储。 从Workfront上传并发送到Assets Essentials的文档确实会计入整体存储。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 8ecbca4d5d09b1f696f489148e960e0eeba2119e
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# 从Experience Manager Assets或Assets Essentials链接资产和文件夹

您可以将资产或文件夹从Experience Manager Assets或Assets Essentials链接到任何支持文档的Adobe Workfront对象。 从Assets Essentials发送的资产不计入Workfront中的整个文档存储。 从Workfront上传并发送到Assets Essentials的文档确实会计入整体存储。

当您将资产从Workfront发送到Experience Manager Assets或Assets Essentials时，首先会映射元数据字段。 如果Workfront管理员已启用对象元数据同步，则在任一应用程序中更改字段时，这些字段将保持为最新。

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
   <td role="rowheader">产品</td> 
   <td>您必须具有Experience Manageras a Cloud Service或Assets Essentials，并且必须以Admin Console用户身份添加到产品中。</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager权限</td> 
    <td>您必须具有对文件夹的写入权限。</td> 
   </tr>
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看访问权限或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

开始之前，

* 您的Workfront管理员必须配置Experience Manager集成。 有关更多信息，请参阅 [配置Experience Manager Assetsas a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 或 [配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## 从Experience Manager Assets或Assets Essentials链接资产

您可以将资产从Experience Manager Assets或Assets Essentials链接到Workfront。 关联资产后，您可以

* [为Experience Manager Assets或Assets Essentials校样链接的资产](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [上传文档的新版本](../../documents/managing-documents/upload-new-document-version.md)

1. 转到 **文档** 中要添加文档的区域。
1. 选择 **新增**，然后选择管理员设置的Experience Manager集成。

   >[!NOTE]
   >
   >Workfront管理员可以为此集成选择任何名称，因此不能特别提及“资产”或“Assets Essentials”。

1. 选择所需的资产。

   ![](assets/select-an-asset.png)

1. 单击 **选择**.

## 链接Experience Manager Assets或Assets Essentials中的文件夹

查看文件夹内单个资产的权限取决于Experience Manager Assets或Assets Essentials权限。

1. 转到 **文档** 中要找到文件夹的区域。
1. 选择 **新增**，然后选择管理员设置的Experience Manager集成。

   >[!NOTE]
   >
   >Workfront管理员可以为此集成选择任何名称，因此可能不会特别提及Assets或Assets Essentials。

1. 选择所需的文件夹。

   ![](assets/select-a-folder.png)

1. 单击 **选择**.

## 从Experience Manager Assets或Assets Essentials链接新版本

您可以从Assets Essentials中提取新资产，并将其作为新版本添加到现有资产中。 如果文档已链接，并且在Assets Essentials中添加了新版本，则新版本会在Workfront中自动显示。

要从Assets Essentials链接新版本，请执行以下操作：

1. 转到 **文档** 中要添加文档的区域。
1. 选择要替换为新版本的资产。 无法在链接的文件夹中创建资产的新版本。
1. 选择 **新增** > **版本**，然后选择管理员设置的Experience Manager集成。

   >[!NOTE]
   >
   >Workfront管理员可以为此集成选择任何名称，因此可能不会特别提及Assets或Assets Essentials。

1. 选择所需的资产。

   ![](assets/select-an-asset.png)

1. 单击 **选择**.

>[!TIP]
>
>如果您转到 **文档详细信息** > **版本**.
