---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 将文档发送到Experience Manager Assets或Assets Essentials
description: 您可以将文档从Workfront发送到Experience Manager Assets或Assets Essentials。 从Workfront上传并发送到Assets Essentials的文档仍会计入整个文档存储中。 从Assets Essentials链接的资产不计入整体存储。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# 将文档发送到Experience Manager Assets或Assets Essentials


您可以将文档从Workfront发送到Experience Manager Assets或Assets Essentials。 从Workfront上传并发送到Assets Essentials的文档仍会计入整个文档存储中。 从Assets Essentials链接的资产不计入整体存储。

当您将资产从Workfront发送到Experience Manager Assets或Assets Essentials时，首先会映射元数据字段。 配置为映射父对象的任何元数据也会发送。 有关配置元数据映射的更多信息，请参阅 [配置Experience Manager Assetsas a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 或 [配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**示例** 首次发送附加到任务的资产时，任务元数据会映射到Experience Manager Assets或Assets Essentials，以及父对象（如项目、项目组合和项目群）中映射的任何元数据。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront计划</a>*</td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">旧版许可证概述</a>*</td> 
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您必须具有Experience Manageras a Cloud Service或Assets Essentials，并且必须以Admin Console用户身份添加到产品中。
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看对文档的访问权限或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

开始之前，

* 您的Workfront管理员必须配置Experience Manager集成。 有关更多信息，请参阅 [配置Experience Manager Assetsas a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 或 [配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## 从Workfront发送文档

当用户将文档从Workfront发送到Experience Manager Assets或Assets Essentials时，映射的元数据会随文档进行传输。 发送文档后，对Workfront中文档元数据所做的更改不会反映在Assets或Assets Essentials中。 如果更改了Workfront中的映射字段，则必须将包含更新元数据的文档新版本发送到Assets或Assets Essentials。 要设置或编辑元数据，请参阅 [配置Experience Manager Assetsas a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 或 [配置Experience Manager Assets Essentials集成](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

要发送文档，请执行以下操作：

1. 转到 **文档** ，然后选择要发送的文档。
1. 单击 **发送到**，然后选择管理员设置的Experience Manager集成。

   >[!NOTE]
   >
   >Workfront管理员可以为此集成选择任何名称，因此不能特别提及“资产”或“Assets Essentials”。

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 选择资产的去向，然后单击 **选择文件夹**.
1. 找到所需目标后，单击 **保存**.

## 发送新版本

您可以向之前上传到Workfront的文档添加新版本。 有关更多信息，请参阅 [上传文档的新版本](../../documents/managing-documents/upload-new-document-version.md). 上传最新版本后，您可以将其发送到Assets Essentials。 如果Workfront中的映射字段发生更改，则新版本会在发送时更新Assets Essentials中的元数据。

>[!IMPORTANT]
>
>在将新版本上传到Workfront之前，我们建议重命名文件。 如果您上传的新版本与之前的版本具有完全相同的文件名，则只能从Workfront下载最新版本。 无论文件名如何，都可以从Experience Manager Assets或Assets Essentials下载所有版本。

要发送最新版本，请执行以下操作：

1. 转到 **文档** ，并找到文档。
1. 选择 **发送到**，然后选择管理员设置的Experience Manager集成。

   >[!NOTE]
   >
   >Workfront管理员可以为此集成选择任何名称，因此可能不会特别提及Assets或Assets Essentials。

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 单击&#x200B;**保存**。新版本保存在与先前版本相同的位置。
