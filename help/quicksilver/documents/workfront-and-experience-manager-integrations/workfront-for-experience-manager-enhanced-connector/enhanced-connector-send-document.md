---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: 使用增强型连接器发送文档
description: 您可以将文档从Workfront发送到Experience Manager Assets。 从Workfront上传并发送到Experience Manager Assets的文档仍会计入您的总体文档存储中。 从Experience Manager Assets链接的Assets不计入总体存储空间。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: 3f9a824780f2ded914d461a473aef3b6ecfa8701
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 1%

---

# 使用增强型连接器发送文档

您可以将文档从Workfront发送到Experience Manager Assets。 从Workfront上传并发送到Experience Manager Assets的文档仍会计入您的总体文档存储中。 从Experience Manager Assets链接的Assets不计入总体存储空间。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>参与者或更高版本</p>
   <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他产品</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问权限</p> s="MCXref xref"&gt;创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看文档访问权限或更高版本</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 先决条件

在开始之前，您必须

* 安装Workfront for Experience Manager增强型连接器。

## 将文档发送到Experience Manager Assets

当用户将文档从Workfront发送到Experience Manager Assets时，映射的元数据将沿着文档传输。 如果已配置，则每次进行更改时，元数据都会连续同步。

要发送文档，请执行以下操作：

1. 转到Workfront中的&#x200B;**文档**&#x200B;区域，然后选择要发送的文档。
1. 单击&#x200B;**发送至**，然后选择管理员设置的Experience Manager Assets集成。

   >[!NOTE]
   >
   >可以为此集成选择任何名称，因此它可能没有特别提及Experience Manager Assets。

   ![发送至](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 选择要将资源放置到的位置，然后单击&#x200B;**选择文件夹**。
1. 找到所需目标后，单击&#x200B;**保存**。

## 向Experience Manager Assets发送新版本

您可以向先前上载到Workfront的文档中添加新版本。 有关详细信息，请参阅[上载文档的新版本](../../../documents/managing-documents/upload-new-document-version.md)。 上传最新版本后，可将其发送到Experience Manager Assets。 如果Workfront中的映射字段已更改，则新版本会在发送时更新Experience Manager Assets中的元数据。

发送最新版本：

1. 转到Workfront中的&#x200B;**文档**&#x200B;区域，然后找到该文档。
1. 单击&#x200B;**发送至**，然后选择管理员设置的Experience Manager Assets集成。

   >[!NOTE]
   >
   >可以为此集成选择任何名称，因此它可能没有特别提及Experience Manager Assets。

   ![发送至](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 单击 **Save**。新版本将保存在与先前版本相同的位置。
