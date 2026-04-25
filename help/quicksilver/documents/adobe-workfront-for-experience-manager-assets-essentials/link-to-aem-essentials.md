---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 从Experience Manager Assets Essentials链接资源和文件夹
description: 您可以从Experience Manager Assets Essentials将资源或文件夹链接到任何支持文档的Adobe Workfront对象。 从Assets Essentials发送的Assets不计入Workfront中的整体文档存储。 从Workfront上传并发送到Assets Essentials的文档确实会计入总体存储中。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 0b93f6f6-cf4b-4077-a464-be7f19f7cd25
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 4%

---

# 从Experience Manager Assets Essentials链接资源和文件夹

您可以从Experience Manager Assets Essentials将资源或文件夹链接到任何支持文档的Adobe Workfront对象。

要使用Content Advisor从Experience Manager Assets链接资源和文件夹，请参阅[使用由Experience Manager Assets提供支持的Content Advisor链接资源和文件夹](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md)。

如果您位于企业存储中，请参阅[将Adobe Experience Manager与Frame.io集成一起使用](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md)。


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

开始之前：

* 您的Workfront管理员必须配置Experience Manager集成。 有关详细信息，请参阅[配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)。

## 从Experience Manager Assets Essentials链接资源

1. 转到Workfront中要添加文档的&#x200B;**文档**&#x200B;区域。
1. 选择&#x200B;**新增**，然后选择管理员设置的Experience Manager集成。

   >[!NOTE]
   >
   >Workfront管理员可以选择此集成的任何名称，因此可能没有特别提及Experience Manager Assets Essentials。

1. 选择所需的资源。

   ![选择资源](assets/select-an-asset.png)

1. 单击&#x200B;**选择**。

## 从Experience Manager Assets Essentials链接新版本

您可以从Experience Manager Assets Essentials中提取新资源，并将其作为新版本添加到现有资源。 如果文档已链接，并且在Experience Manager Assets Essentials中添加了新版本，则新版本会自动显示在Workfront中。

要链接新版本，请执行以下操作：

1. 转到Workfront中要添加文档的&#x200B;**文档**&#x200B;区域。
1. 选择要替换为新版本的资产。 您无法在链接的文件夹中创建资产的新版本。
1. 选择&#x200B;**新增** > **版本**，然后选择管理员设置的Experience Manager集成。

   >[!NOTE]
   >
   >Workfront管理员可以选择此集成的任何名称，因此可能没有特别提及Experience Manager Assets Essentials。

1. 选择要链接的资源。

1. 单击&#x200B;**选择**。

## 从Experience Manager Assets Essentials链接文件夹

查看文件夹内各个资产的权限取决于Experience Manager Assets Essentials权限。

1. 转到Workfront中要放置文件夹的&#x200B;**文档**&#x200B;区域。
1. 选择&#x200B;**新增**，然后选择管理员设置的Experience Manager集成。

   >[!NOTE]
   >
   >Workfront管理员可以选择此集成的任何名称，因此可能没有特别提及Experience Manager Assets Essentials。

1. 选择所需的文件夹。

   ![选择文件夹](assets/select-a-folder.png)

1. 单击&#x200B;**选择**。

## 注意事项

* 内容审查程序功能不适用于Assets Essentials。 要使用“内容顾问”链接资源和文件夹，请参阅[将资源和文件夹与Experience Manager Assets支持的内容顾问链接](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md)。

* 从Assets Essentials发送的Assets不计入Workfront中的整体文档存储。 从Workfront上传并发送到Assets Essentials的文档确实会计入总体存储中。

* 在将资源从Workfront发送到Experience Manager Assets Essentials时，首先映射元数据字段。 如果您的Workfront管理员启用了对象元数据同步，则在任一应用程序中更改了某些字段后，这些字段将保持最新状态。
