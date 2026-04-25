---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 将文档发送到Experience Manager Assets或Assets Essentials
description: 您可以将文档从Workfront发送到Experience Manager Assets或Assets Essentials。 从Workfront上传并发送到Assets Essentials的文档仍会计入您的总体文档存储中。 从Assets Essentials链接的Assets不计入总体存储空间。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 2%

---

# 将文档发送到Experience Manager Assets或Assets Essentials

您可以将文档从Workfront发送到Experience Manager Assets或Assets Essentials。 从Workfront上传并发送到Assets Essentials的文档仍会计入您的总体文档存储中。 从Assets Essentials链接的Assets不计入总体存储空间。

通过此集成发送到Experience Manager的Assets具有&#x200B;**5 GB**&#x200B;的大小限制。

在“预览”环境中，通过此集成发送到Experience Manager的Assets具有&#x200B;**30 GB**&#x200B;的大小限制。

>[!NOTE]
>
>新文档区域不提供此功能。<br>
>如果您的组织使用企业存储，则当您访问Workfront中的文档时，将会看到“新建文档”区域。 从该位置，您可以将资源发送到Experience Manager Assets。 有关详细信息，请参阅[将Adobe Experience Manager与Frame.io集成一起使用](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md)。

## 元数据

在将资源从Workfront发送到Experience Manager Assets或Assets Essentials时，首先映射元数据字段。 配置为映射父对象的任何元数据也会发送。 有关配置元数据映射的详细信息，请参阅[配置Experience Manager Assets as a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)或[配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)。

>[!INFO]
>
>**示例**&#x200B;首次发送附加到任务的资源时，任务元数据将映射到Experience Manager Assets或Assets Essentials，以及父对象（如项目、项目组合和项目群）中的任何映射元数据。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p> “任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 许可证</td> 
   <td> 
   <p>参与者或更高版本</p> 
   <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他产品</td> 
   <td>您必须安装了Experience Manager as a Cloud Service或Assets Essentials，并且您必须作为用户添加到Admin Console的产品中。</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager权限</td> 
    <td>您必须具有此文件夹的写入权限。</td> 
   </tr>
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看访问权限或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

Before you begin,

* 您的Workfront管理员必须配置Experience Manager集成。 有关详细信息，请参阅[配置Experience Manager Assets as a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)或[配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)。


## Send a Document from Workfront

When a user sends a document from Workfront to Experience Manager Assets or Assets Essentials, mapped metadata transfers along the document. After the document is sent, changes made to the document&#39;s metadata in Workfront are not reflected in Assets or Assets Essentials. If a mapped field in Workfront is changed, you must send a new version of the document with the updated metadata to Assets or Assets Essentials. To set up or edit metadata, see [Configure the Experience Manager Assets as a Cloud Service integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) or [Configure the Experience Manager Assets Essentials integration](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

To send a document:

1. Go to the **Documents** area in Workfront, and select the document you want to send.
1. Click **Send to**, then choose the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it may not specifically mention Assets or Assets Essentials.

   ![Send to](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Choose where you want the asset to go, then click **Select Folder**.
1. When you find your desired destination, click **Save**.

## Send a new version

You can add a new version to a document you have previously uploaded to Workfront. For more information, see [Upload a new version of a document](../../documents/managing-documents/upload-new-document-version.md). After the latest version is uploaded, you can send it to Assets Essentials. If a mapped field in Workfront has changed, the new version updates the metadata in Assets Essentials when it sends.

>[!IMPORTANT]
>
>Before you upload a new version to Workfront, we recommend renaming the file. 如果上传的文件名与以前版本完全相同，则只能从Workfront下载最新版本。 无论文件名如何，均可从Experience Manager Assets或Assets Essentials下载所有版本。

发送最新版本：

1. 转到Workfront中的&#x200B;**文档**&#x200B;区域，然后找到该文档。
1. 选择&#x200B;**发送至**，然后选择管理员设置的Experience Manager集成。

   >[!NOTE]
   >
   >Workfront管理员可以选择此集成的任何名称，因此可能没有特别提及Assets或Assets Essentials。

   ![发送至](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 单击 **Save**。 新版本将保存在与先前版本相同的位置。

## 在Experience Manager Assets中将文档移动到链接的文件夹

>[!NOTE]
>
>此功能仅适用于Experience Manager Assets as a Cloud Service。 它不适用于Experience Manager Assets Essentials。

如果文档和链接文件夹位于同一文档列表（如项目的文档区域）中，则可以将文档移至Experience Manager Assets中的链接文件夹。

1. 找到要移动的文档。
1. 将文档拖放到要将它移动到的链接Experience Manager Assets文件夹中。

文档正在移动时，文档选项不可用。 将文档移至Experience Manager Assets后，在Workfront的文档列表中不再可见。

>[!NOTE]
>
> 您在文档移动时对文档所做的任何操作或编辑都不会显示在Experience Manager Assets的文档中，因此将丢失。

