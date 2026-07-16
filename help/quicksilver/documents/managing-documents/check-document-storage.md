---
product-area: documents
navigation-topic: manage-documents
title: 检查文档存储限制
description: 作为Adobe Workfront管理员，您可以在“客户信息”页面上查看文档存储使用情况和配额。 存储的显示方式取决于您的组织是使用旧版Workfront存储还是Adobe云存储。
author: Courtney
feature: Digital Content and Documents
exl-id: f5d1963e-b205-44b9-b2b6-b7de465c6977
last-update: 2026-04-29T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/vOjgBLxX5rFIGHBCHB2a6Q3Bs3KE5x-opXUMvANjI1E
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 09dff59503604894e61f2a62af7ae1c2e8a39068
workflow-type: tm+mt
source-wordcount: 491
ht-degree: 3%

---

# 检查文档存储限制

尽管用户可以上传到Workfront实例的单个文件的类型和大小没有限制，但您的Workfront计划包含总存储配额。 作为Workfront管理员，您可以从“客户信息”页面上的“设置”区域监控使用情况和配额。

存储的显示方式取决于您的组织是使用旧版Workfront存储还是Adobe云存储：

* 如果您使用旧版Workfront存储，请参阅本文中的[旧版Workfront存储](#legacy-workfront-storage)。
* 如果您使用Adobe云存储，请参阅本文中的[Adobe云存储](#adobe-cloud-storage)。

  有关Adobe云存储的更多信息，请参阅[Adobe云存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Workfront计划</td> 
   <td> <p>使用旧版存储管理文档的任意Workfront软件包</p>
      <p>用于使用Adobe云存储管理文档的任意工作流包</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>您必须是Workfront管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 旧版 Workfront 存储

如果您的组织使用旧版Workfront存储，则“客户信息”页面会显示直接上传到Workfront的文档的单个存储配额。

要检查旧版Workfront文档存储，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**系统** > **客户信息**。
1. 在&#x200B;**基本信息**&#x200B;部分中，找到&#x200B;**存储配额**。 在这里，您可以查看您当前使用的存储空间量以及Workfront计划包括的存储空间总量。

存储配额每天刷新一次，以显示最新计数。

>[!NOTE]
>
>此限制不适用于您从任何其他第三方服务提供商（SharePoint、Google Drive、Webdam、Box、Dropbox或任何其他文档资产管理提供商）链接到Workfront的文档。

## Adobe 云存储


如果您的组织使用Adobe云存储，您的存储配额将报告为单个池分配，该分配将通过Workfront许可证预配的存储与通过Frame.io Enterprise加载项预配的任何存储组合在一起。 存储使用量没有硬性限制；即使使用量超过您的配额，用户也可以继续上传文档。

### 在客户信息中查看存储使用情况

要检查Adobe云存储中的文档，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**系统** > **客户信息**。
1. 转到&#x200B;**存储概述**&#x200B;部分。
1. 检查您的使用情况。 “存储概述”显示您的池存储配额，并将使用情况分为：

   * Workfront旧版项目和Adobe cloud storage项目会显示在蓝色栏中。
   * 框架独立项目显示在绿色栏中。 这些项目独立于Workfront，并且仅在您拥有Frame.io Enterprise许可证时才可用。


客户信息中的![Adobe云存储使用情况](assets/storage-usage.png)

使用情况数字会定期刷新，以便您查看最新计数。

### 管理员的电子邮件通知

当使用量超过存储配额的75% 、 90%或100%时， Workfront会向系统管理员发送电子邮件通知。
