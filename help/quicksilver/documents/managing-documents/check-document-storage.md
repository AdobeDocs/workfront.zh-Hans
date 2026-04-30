---
product-area: documents
navigation-topic: manage-documents
title: 检查文档存储限制
description: 作为Adobe Workfront管理员，您可以在“客户信息”页面上查看文档存储使用情况和配额。 存储的显示方式取决于您的组织使用的是旧版Workfront存储还是Adobe企业级存储。
author: Courtney
feature: Digital Content and Documents
exl-id: f5d1963e-b205-44b9-b2b6-b7de465c6977
last-update: 2026-04-29T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: e25be455e16beee813e612b983bca1302f129e6f
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 2%

---

# 检查文档存储限制

{{highlighted-preview}}

尽管用户可以上传到Workfront实例的单个文件的类型和大小没有限制，但您的Workfront计划包含总存储配额。 作为Workfront管理员，您可以从“客户信息”页面上的“设置”区域监控使用情况和配额。

存储的显示方式取决于您的组织使用的是旧版Workfront存储还是Adobe企业级存储：

* 如果您使用旧版Workfront存储，请参阅本文中的[旧版Workfront存储](#legacy-workfront-storage)。
* 如果您使用Adobe企业存储，请参阅本文中的[Adobe企业存储](#adobe-enterprise-storage)。

  有关企业存储的更多信息，请参阅[Adobe企业存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Workfront计划</td> 
   <td> <p>使用旧版存储管理文档的任意Workfront软件包</p>
      <p>用于使用Adobe企业存储管理文档的任意工作流包</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>您必须是Workfront管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 旧版Workfront存储

如果您的组织使用旧版Workfront存储，则“客户信息”页面会显示直接上传到Workfront的文档的单个存储配额。

要检查旧版Workfront文档存储，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**系统** > **客户信息**。
1. 在&#x200B;**基本信息**&#x200B;部分中，找到&#x200B;**存储配额**。 在这里，您可以查看您当前使用的存储空间量以及Workfront计划包括的存储空间总量。

存储配额每天刷新一次，以显示最新计数。

>[!NOTE]
>
>此限制不适用于您从任何其他第三方服务提供商（SharePoint、Google Drive、Webdam、Box、Dropbox或任何其他文档资产管理提供商）链接到Workfront的文档。

<div class="preview">

## Adobe企业存储

如果您的组织使用Adobe企业存储，则“客户信息”会显示存储概述，其中将旧版Workfront存储、Adobe企业存储和Frame.io的使用情况划分为不同的部分。 当使用量超过您的配额时，Workfront还会对上传应用软上限，以便用户仍然可以上传文档。

### 在客户信息中查看存储使用情况

要检查Adobe企业文档存储，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**系统** > **客户信息**。
1. 转到&#x200B;**存储概述**&#x200B;部分。
1. 查看Adobe企业存储的使用情况。
   <!--Both Workfront and Frame.io usage are broken down separately, but roll up to the total usage for Adobe enterprise storage.-->

客户信息中的![Adobe企业存储使用情况](assets/storage-usage.png)

使用情况数字会定期刷新，以便您查看最新计数。

### 管理员的电子邮件通知

当使用量超过存储配额的75% 、 85%或100%时， Workfront会向系统管理员发送电子邮件通知。

</div>