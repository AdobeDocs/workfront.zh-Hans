---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: 创建与Experience Manager Assets或Assets Essentials链接的文件夹
description: 在Workfront中，您可以创建与Experience Manager Assets或Assets Essentials链接的文件夹。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: 84760d5fe301bd0a44879490fb030bd29821bd41
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# 创建与Experience Manager Assets或Assets Essentials链接的文件夹

在Workfront中，您可以创建与Experience Manager Assets或Assets Essentials链接的文件夹。 由于该文件夹已链接，因此添加到该文件夹的任何资源都将自动显示在Workfront和Experience Manger中。 如果资产位于链接的文件夹中，则无需手动发送。

如果从Experience Manager Assets或Assets Essentials内的链接文件夹中删除或移动资源，Workfront会在项目>文档区域中保留该资源的副本。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件：

<table>
  <tr>
   <td><strong>Adobe Workfront计划*</strong>
   </td>
   <td>任何
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront许可证*</strong>
   </td>
   <td>计划
   </td>
  </tr>
  <tr>
   <td><strong>产品</strong>
   </td>
   <td>您必须具有Experience Manager Assetsas a Cloud Service或Assets Essentials，并且您必须作为用户添加到产品中。
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager权限</strong>
   </td>
   <td>您必须具有Experience Manger集成中目标文件夹的写入权限。
   </td>
  </tr>
  <tr>
   <td><strong>访问级别配置</strong>
   </td>
   <td>您必须是Workfront管理员才能配置Experience Manager集成。 配置该计划后，拥有计划许可证的用户可以在单个项目上设置链接文件夹。
   </td>
  </tr>
</table>


*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

+++

## 先决条件

开始之前，

* 您的Workfront管理员必须配置Experience Manager集成。 有关详细信息，请参阅[配置Experience Manager Assetsas a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)或[配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)。


## 创建链接文件夹

会在Workfront管理员设置集成时指定的位置创建链接的文件夹。 每个集成只能有一个文件夹位置用于链接的文件夹。

链接文件夹的名称会根据与其关联的Portfolio、项目群、项目自动创建，且无法更改。 如果项目未与Portfolio或项目群关联，则链接的文件夹将显示项目名称和创建日期。

要创建链接文件夹，请执行以下操作：

1. 转到要在其中放置文件夹的项目。
1. 选择&#x200B;**新增**，然后转到管理员设置的Experience Manager集成。

   >[!NOTE]
   >
   >Workfront管理员可以选择此集成的任何名称，因此可能没有特别提及Experience Manager Assets或Assets Essentials。

1. 选择&#x200B;**创建链接文件夹**。 系统会根据设置集成时指定的位置，在Experience Manager中自动创建文件夹。
   ![创建链接文件夹](assets/linked-folder.png)
