---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: 创建链接了Experience Manager Assets或Assets Essentials的文件夹
description: 在Workfront中，您可以创建与Experience Manager Assets或Assets Essentials链接的文件夹。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# 创建链接了Experience Manager Assets或Assets Essentials的文件夹

在Workfront中，您可以创建与Experience Manager Assets或Assets Essentials链接的文件夹。 由于文件夹已关联，因此添加到该文件夹的任何资产都将自动同时显示在Workfront和Experience Manager中。 如果资产位于链接的文件夹中，则无需手动发送该资产。


## 访问要求

您必须具备以下条件：

<table>
  <tr>
   <td><strong>Adobe Workfront计划*</strong>
   </td>
   <td>任意
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
   <td>您必须具有Experience Manager Assetsas a Cloud Service或Assets Essentials，并且必须作为用户添加到产品中。
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager权限</strong>
   </td>
   <td>您必须对Experience Manager集成中的目标文件夹具有写入权限。
   </td>
  </tr>
  <tr>
   <td><strong>访问级别配置</strong>
   </td>
   <td>您必须是Workfront管理员。 有关Workfront管理员的信息，请参阅 <strong>授予用户完全管理访问权限</strong>.
   </td>
  </tr>
</table>


*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。


## 先决条件

开始之前，

* 您的Workfront管理员必须配置Experience Manager集成。 有关更多信息，请参阅 [配置Experience Manager Assetsas a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 或 [配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## 创建链接的文件夹

链接的文件夹是在Workfront管理员设置集成时指定的位置创建的。 每个集成只能有一个链接文件夹的位置。

链接文件夹的名称会根据与关联的Portfolio、项目、项目名称自动创建，且无法更改。 如果项目与Portfolio或项目群没有关联，则链接的文件夹将显示项目名称和创建日期。

要创建链接的文件夹，请执行以下操作：



1. 转到所需文件夹的项目。
1. 选择 **新增**，然后转到管理员设置的Experience Manager集成。
   >[!NOTE]
   >
   >Workfront管理员可以为此集成选择任何名称，因此可能不会特别提及Experience Manager Assets或Assets Essentials。

1. 选择 **创建链接的文件夹**. 系统会根据集成设置时指定的位置，自动在Experience Manager中创建文件夹。
   ![创建链接的文件夹](assets/linked-folder.png)
