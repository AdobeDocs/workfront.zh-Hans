---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 将文档发送到Experience Manager Assets或Assets Essentials
description: 您可以将文档从Workfront发送到Experience Manager Assets或Assets Essentials。 从Workfront上传并发送到Assets Essentials的文档仍会计入您的总体文档存储中。 从Assets Essentials链接的Assets不计入总体存储空间。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '919'
ht-degree: 0%

---

# 将文档发送到Experience Manager Assets或Assets Essentials

您可以将文档从Workfront发送到Experience Manager Assets或Assets Essentials。 从Workfront上传并发送到Assets Essentials的文档仍会计入您的总体文档存储中。 从Assets Essentials链接的Assets不计入总体存储空间。

通过此集成发送到Experience Manager的Assets具有&#x200B;**5 GB**&#x200B;的大小限制。

在“预览”环境中，通过此集成发送到Experience Manager的Assets具有&#x200B;**30 GB**&#x200B;的大小限制。

在将资源从Workfront发送到Experience Manager Assets或Assets Essentials时，首先映射元数据字段。 配置为映射父对象的任何元数据也会发送。 有关配置元数据映射的详细信息，请参阅[配置Experience Manager Assets as a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)或[配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)。

>[!INFO]
>
>**示例**&#x200B;首次发送附加到任务的资源时，任务元数据将映射到Experience Manager Assets或Assets Essentials，以及父对象（如项目、项目组合和项目群）中的任何映射元数据。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能完成本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">Adobe Workfront计划</a>*</td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">旧版许可证概述</a>*</td> 
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您必须安装了Experience Manager as a Cloud Service或Assets Essentials，并且您必须作为用户添加到Admin Console的产品中。
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看文档访问权限或更高版本</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

+++

## 先决条件

开始之前，

* 您的Workfront管理员必须配置Experience Manager集成。 有关详细信息，请参阅[配置Experience Manager Assets as a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)或[配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)。


## 从Workfront发送文档

当用户将文档从Workfront发送到Experience Manager Assets或Assets Essentials时，映射的元数据将沿文档传输。 发送文档后，在Workfront中对文档元数据所做的更改不会反映在Assets或Assets Essentials中。 如果Workfront中的映射字段发生更改，您必须将包含更新后元数据的文档的新版本发送到Assets或Assets Essentials。 要设置或编辑元数据，请参阅[配置Experience Manager Assets as a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)或[配置Experience Manager Assets Essentials集成](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)。

要发送文档，请执行以下操作：

1. 转到Workfront中的&#x200B;**文档**&#x200B;区域，然后选择要发送的文档。
1. 单击&#x200B;**发送至**，然后选择管理员设置的Experience Manager集成。

   >[!NOTE]
   >
   >Workfront管理员可以选择此集成的任何名称，因此可能没有特别提及Assets或Assets Essentials。

   ![发送至](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 选择要将资源放置到的位置，然后单击&#x200B;**选择文件夹**。
1. 找到所需目标后，单击&#x200B;**保存**。

## 发送新版本

您可以向先前上载到Workfront的文档中添加新版本。 有关详细信息，请参阅[上载文档的新版本](../../documents/managing-documents/upload-new-document-version.md)。 上传最新版本后，可将其发送到Assets Essentials。 如果Workfront中的映射字段已更改，则新版本会在发送时更新Assets Essentials中的元数据。

>[!IMPORTANT]
>
>在将新版本上传到Workfront之前，我们建议重命名文件。 如果上传的文件名与以前版本完全相同，则只能从Workfront下载最新版本。 无论文件名如何，均可从Experience Manager Assets或Assets Essentials下载所有版本。

发送最新版本：

1. 转到Workfront中的&#x200B;**文档**&#x200B;区域，然后找到该文档。
1. 选择&#x200B;**发送至**，然后选择管理员设置的Experience Manager集成。

   >[!NOTE]
   >
   >Workfront管理员可以选择此集成的任何名称，因此可能没有特别提及Assets或Assets Essentials。

   ![发送至](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 单击&#x200B;**保存**。 新版本将保存在与先前版本相同的位置。

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

